---
date: 2026-05-20
title: Cortex extensions — chat-logger agent, soft-reminder Stop hook, graph-builder agent, initial graph view
tags: [meta, memory-system, retrieval, ops, decision, system-design, agents, hooks]
outcomes-touched: []
artifacts:
  created:
    - ~/.claude/agents/chat-logger.md
    - ~/.claude/agents/graph-builder.md
    - kompete-research/.claude/hooks/chat-logger-reminder.sh
    - kompete-research/graph.md
    - kompete-research/chats/2026-05-20-cortex-extensions-hook-and-graph.md  # this file
  updated:
    - kompete-research/.claude/settings.local.json (added Stop hook registration)
    - kompete-research/chats/README.md (referenced chat-logger agent in protocol)
    - kompete-research/decision-log.md (appended D#9)
    - memory/MEMORY.md (added pointers to agents)
  referenced:
    - kompete-research/strategy-and-principles.md
    - kompete-research/chats/2026-05-19-operating-cortex-system.md (the design)
related-chats: [2026-05-19-operating-cortex-system]
chat-source: claude-code-cli
status: live
---

# Cortex extensions — chat-logger agent, Stop hook, graph-builder + graph view

## Context

User raised two follow-up questions on the day-old Operating Cortex: (1) should we add a graph-style retrieval layer (GraphRAG / Cypher / GraphQL-like) on top of the chats, and (2) how do we ensure every session actually gets logged — manual discipline is fragile.

## Work done

### Graph retrieval question (answered, not built heavily)

Concluded that **the frontmatter we designed yesterday already encodes a graph**. Each chat entry has `tags`, `outcomes-touched`, `artifacts`, `related-chats` — that's an adjacency list. At our current scale (3 chats, 8 decisions), Claude walks it in-context implicitly. We don't need infrastructure (Neo4j, vector DB, GraphRAG framework) — we need a *view* over what's already there.

Three-phase plan documented in the chat:
- **Now (<30 chats):** Claude walks frontmatter implicitly. Plus we can generate a static graph view on demand via a subagent.
- **Soon (~30–100):** static `graph.md` becomes the primary navigation aid; regenerated periodically.
- **Later (200+):** real graph DB; frontmatter ports cleanly when we get there.

### Three artifacts built today

1. **`~/.claude/agents/chat-logger.md`** — Haiku-model subagent that reads the chats/ convention, the strategy doc (for KR slugs), and recent chats; writes a timestamped entry following the README schema; appends to decision-log.md if durable decisions were made; outputs a brief confirmation. Invocable from any future session via the parent's Agent tool (`subagent_type: chat-logger`).

2. **`kompete-research/.claude/hooks/chat-logger-reminder.sh`** — bash hook that fires on `Stop` events. Checks whether files in `kompete-research/` (excluding `chats/`) or `memory/` have been modified more recently than the latest chat-log entry. If yes, prints a one-line reminder for Claude to suggest invoking chat-logger. Rate-limited to once per hour via a `/tmp` marker file. Registered in `.claude/settings.local.json`.

3. **`~/.claude/agents/graph-builder.md`** — Sonnet-model subagent that walks all chat frontmatter + decision-log rows + strategy doc references, materializes a derivable graph view at `kompete-research/graph.md`. Sections: snapshot, Mermaid concept graph, tag cross-reference, outcome→chats index, decision provenance chains, artifact provenance, open questions surfaced, recent activity. Re-runnable on demand.

4. **`kompete-research/graph.md`** — initial graph view of the current 3-chat / 8-decision corpus. Built manually this session (the graph-builder subagent will run it natively starting next session). Already useful for visual scan: shows the corpus has a clear spine (foundations-research → strategy-doc → operating-cortex), with `moat` / `counter-positioning` and the strategy doc as the most-connected nodes.

### Caveat about agents this session

Subagent files created mid-session are not loadable by the current Claude Code session — both `chat-logger` and `graph-builder` will become invocable from the next fresh session onward. For today: this chat entry was written manually following the convention; the graph.md was generated manually following the agent's intended methodology. From tomorrow on, the agents do this work.

## Decisions

- **decision-log #9** — Cortex extensions: soft-reminder Stop hook for chat-logger (chosen over no-hook or auto-trigger); graph-builder as a dedicated Sonnet subagent (chosen over deferring or one-time manual generation); graph.md as a derivable artifact (regenerable on demand, not the source of truth).

## Artifacts

- **Created:** 4 files (chat-logger agent, graph-builder agent, hook script, graph.md) + this chat entry
- **Updated:** project settings.local.json (Stop hook registered), chats/README.md (agent invocation documented), decision-log.md (row #9), MEMORY.md (pointers to new agents)
- **Referenced:** strategy-and-principles.md, the 2026-05-19 design chat

## Open questions / next steps

- **Test the agents from a fresh Claude Code session.** Open a new session, say "where were we?", verify the latest chats load. Then invoke chat-logger on the session's exit and confirm it produces a clean entry. Then invoke graph-builder and confirm it regenerates `graph.md` faithfully.
- **Soft-reminder hook in practice.** It's set to rate-limit to once per hour. If it gets annoying (fires on small edits), we tighten the "meaningful work" detection in the script.
- **Zeropearl migration still optional.** Parallel chat can opt in when convenient. If they don't, that's also fine — their file is referenceable from graph.md notes.
- **Graph view refresh cadence.** Set as "after 5 new chats since last gen." Worth revisiting once we have ~15 chats and see whether scanning the diff is useful.
- **Substantive work queued** (from the strategy doc, unchanged from yesterday): MVP-plan outcome rewrite, Mom-Test audit of 27 interviews, 10 WTP conversations, "Why won't Klue copy us?" one-pager, OST + Product Kata.

## Notes

The session's headline insight isn't any one artifact — it's that **the Operating Cortex now has a closed loop**: rich frontmatter (yesterday) → chat-logger subagent maintains it (today) → soft-reminder hook prevents forgetting (today) → graph-builder materializes a view on demand (today). All five components work together to ensure context survives sessions, laptops, and parallel chats without manual discipline being the only safeguard.

Also worth noting: the user's correction on Day 1 (timestamp+tags, not folders) made all of this much simpler. A folder-categorized system would have made graph-builder substantially harder — you'd have to walk a directory tree to find cross-cutting nodes, vs. just walking a flat list and looking at frontmatter. Pays back already.
