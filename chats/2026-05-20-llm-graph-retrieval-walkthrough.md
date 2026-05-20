---
date: 2026-05-20
title: Graph visualization + how an LLM reads/queries the Operating Cortex (walkthrough)
tags: [meta, memory-system, retrieval, ops, documentation, graph]
outcomes-touched: []
artifacts:
  created:
    - kompete-research/chats/2026-05-20-llm-graph-retrieval-walkthrough.md  # this file
  updated: []
  referenced:
    - kompete-research/graph.md
    - kompete-research/chats/README.md
    - kompete-research/decision-log.md
    - kompete-research/chats/2026-05-20-cortex-extensions-hook-and-graph.md (the morning session)
related-chats: [2026-05-20-cortex-extensions-hook-and-graph, 2026-05-19-operating-cortex-system]
chat-source: claude-code-cli
status: live
---

# LLM graph retrieval walkthrough

## Context

After building the cortex extensions (chat-logger + Stop hook + graph-builder + graph.md) in the morning session, two follow-up exchanges grounded the system in practical mechanics: (1) what does the graph actually *look like* and (2) how does an LLM (or any future model/agent) *query* it. Both were durable enough to capture as a self-contained reference, since the retrieval-pattern walkthrough codifies *how* the Operating Cortex is actually used — which wasn't fully written down until this conversation.

## Work done

### Exchange A — "Show me the graph visually"

Produced four views of the current 4-chat / 9-decision corpus:
1. **ASCII chronological spine** — chats in time order with their decisions branching out; chat #2 (strategy doc) confirmed as the load-bearing hub
2. **Cleaner Mermaid source** — paste-into-mermaid.live-ready, color-coded (chats blue, decisions green, open decisions yellow-dashed)
3. **Concept centrality scan** — tag frequency, showing `gtm`, `positioning`, `meta`, `moat`, `pricing`, `foundations` as the most-connected hubs at this stage
4. **Y1 OKR coverage** — all 7 KRs touched in exactly one chat (the strategy doc) — flagged as the diagnostic that needs to *change* by mid-June to confirm we're working on outcomes vs just researching around them

Key observations surfaced by the visualization:
- The corpus has a clean *spine* (foundations → strategy → cortex → cortex-extensions) — easy to maintain at this scale
- D#7 (pricing) is the single open decision; it blocks KR6 (commercial) — the highest-leverage queued task
- No chat has touched `klue` directly yet — only via D#3's tag — so the "Why won't Klue copy us?" pressure-test will create the first explicit Klue-tagged chat

### Exchange B — "How does an LLM read/query this?"

Explicit walkthrough of what the "graph" actually is and how retrieval works in practice. Six retrieval patterns demoed with **live grep commands** showing real outputs:

| Pattern | Question | Recipe |
|---|---|---|
| **A. Single-concept lookup** | "What did we say about pricing?" | `grep -l "^tags:.*pricing" chats/*.md` → read matches |
| **B. Decision provenance** | "Why are we positioning as deal intelligence?" | `grep -i "<topic>" decision-log.md` → follow chat-source + artifact links |
| **C. Outcome / KR tracking** | "How are we tracking on KR1 — pilots?" | `grep -l "outcomes-touched:.*kr1-pilots" chats/*.md` → read in date order |
| **D. Multi-hop traversal** | "Everything connecting Klue and pricing" | grep both tags independently, then walk via decision-log for indirect connections |
| **E. Session resume** | "Where were we?" | MEMORY.md + ls -t chats/ \| head -3 + graph.md §8 |
| **F. State aggregation** | "What's open?" | grep decision-log for "Open" + aggregate chats' "Open questions" sections |

The honest framing emphasized: **this isn't a real graph DB** — it's structured markdown + grep traversal. The "graph" emerges when an LLM walks the frontmatter relationships. That distinction matters for two reasons:
- It explains why this works at our scale (4 chats reads instantly into context)
- It defines when it breaks (~500 chats → port frontmatter to Postgres or Neo4j; data model is already graph-native, only engine swaps)

The traversal primitives an LLM needs: **Read + Grep + Glob + Bash**. Nothing else. Any model with file-tool access — Claude, GPT, Gemini, local Llama — can use this corpus the same way. That's the portability property.

### Verified: the system works end-to-end

The live grep demos returned correct results:
- Pattern A returned 2 chats tagged pricing (foundations-research, strategy-doc) — as expected
- Pattern B returned D#5 and D#6 with clean chat-source links — as expected
- Pattern C revealed KR1 has been *defined* but no work has *moved* it yet — useful diagnostic
- Pattern D showed Klue and pricing are connected via D#3 ↔ strategy-doc ↔ D#7 — exactly the 2-hop traversal a real graph DB would surface with Cypher

The structure is doing what it was designed to do.

## Decisions

None — this session clarified *how* the existing system (D#8, D#9) is actually used. No new strategic choices. The retrieval patterns themselves are now documented in this chat for any future LLM that needs to learn them.

## Artifacts

- **Created:** this chat entry (durable reference for the 6 retrieval patterns)
- **Referenced:** graph.md (the visualization), chats/README.md (the convention), decision-log.md (for live grep demos), the morning's chat entry

## Open questions / next steps

- **Consider expanding `chats/README.md`** to include the 6 retrieval patterns as a "How to query this" section. Right now the README has the protocol but not the query recipes — adding them would help any future LLM bootstrap faster. Not urgent.
- **Regenerate `graph.md`** next session via the graph-builder subagent to include today's two chats. (Skipped now; the user is shutting down. Next session's first graph-builder run will pick it up.)
- **Self-validating moment queued:** next Claude session should open with "where were we?" and verify Pattern E works end-to-end across a laptop restart.

## Notes

**The implicit confirmation in this session:** the Stop hook is active (registered in `.claude/settings.local.json`), with the test marker cleared. It should have fired on each assistant Stop event during this conversation. If the user has been seeing the soft-reminder text appear in the transcript (or not), that's the validation we needed about whether the hook is correctly wired without being intrusive.

**The most durable thing in this chat:** the 6 retrieval patterns. They're not just teaching content — they're the *operational protocol* for any LLM working in this corpus. Worth re-reading anytime someone (or some model) onboards to Kompete and asks "how do I find what's been decided about X?"

**On the meta question of "what makes this portable across LLMs":** the entire system is self-describing. A future LLM with zero prior context can discover everything from one entry point (MEMORY.md → chats/README.md → graph.md → individual chats). No tribal knowledge, no founder dependency. That portability is what makes the markdown-based design preferable to a proprietary graph DB at this stage — even if it's "less powerful" in pure querying terms.
