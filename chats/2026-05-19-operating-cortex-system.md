---
date: 2026-05-19
title: Designed & built the Operating Cortex — chats/ + decision-log + tag-based retrieval
tags: [meta, memory-system, retrieval, ops, system-design, decision]
outcomes-touched: []
artifacts:
  created:
    - kompete-research/chats/README.md
    - kompete-research/decision-log.md
    - kompete-research/chats/2026-05-18-product-foundations-research.md
    - kompete-research/chats/2026-05-18-strategy-and-principles-doc.md
    - kompete-research/chats/2026-05-19-operating-cortex-system.md  # this file
  updated:
    - memory/MEMORY.md
  referenced:
    - kompete-research/strategy-and-principles.md
    - kompete-research/investor-conversations/zeropearl-vc-jai.md (parallel chat; not migrated)
related-chats: [2026-05-18-product-foundations-research, 2026-05-18-strategy-and-principles-doc]
chat-source: claude-code-cli
status: live
---

# Operating Cortex — system for not losing context across sessions, laptops, and parallel chats

## Context

After two days of foundation research + the operating doc, the volume of working context exceeded what fits in any single Claude session. The user wanted a system so that (a) closing laptop / fresh chat doesn't lose context, (b) parallel chats (e.g., the Zeropearl VC reply chat running separately) feed into the same institutional memory, (c) every discussion can be tagged to outcomes/departments for retrieval, (d) in 1–2 years we can look back at how thinking evolved.

## Work done

Initially proposed a **thread-folder** structure (folder-per-topic: pricing/, fundraising/, product/, etc.). User pushed back: folder categorization forces a primary axis that doesn't match how real conversations work — most touch multiple topics at once. Better: flat timestamped log + tags for retrieval.

Redesigned and built:

### Final structure

```
kompete-research/
├── strategy-and-principles.md         (anchor — already existed)
├── decision-log.md                    (NEW — single file, durable decisions)
└── chats/                             (NEW — flat folder, timestamped entries)
    ├── README.md                       (convention + tag vocabulary)
    ├── 2026-05-18-product-foundations-research.md
    ├── 2026-05-18-strategy-and-principles-doc.md
    └── 2026-05-19-operating-cortex-system.md
```

### Frontmatter schema

Each chat entry has YAML frontmatter with: date, title, tags (free-form list), outcomes-touched (Y1 KRs), artifacts (created/updated/referenced), related-chats, chat-source, status.

### Protocol

- **Session start:** MEMORY.md auto-loads; if topic is referenced, Claude greps `chats/` for prior context.
- **Session end (meaningful work):** Claude writes timestamped file in `chats/`; if durable decision was made, adds row to `decision-log.md`; updates MEMORY.md only if orientation has changed.
- **Parallel chats:** each writes independently to its own timestamped file; same tags surface overlap. Zeropearl chat continues at existing path (`investor-conversations/zeropearl-vc-jai.md`) until that chat opts in.
- **Retrieval:** grep by tag (`tags: pricing`), by date range (ls + sort), by outcome (`outcomes-touched:.*kr3`), or by decision-log row.

### Tag vocabulary (seeded; extends by use)

Domain (pricing, fundraising, gtm, product, hiring, ops, market-intel), Concept (counter-positioning, hook-model, build-trap, atomic-network, mom-test, etc.), Operational (decision, draft, research, synthesis, meta, open-question), Outcome (kr1-pilots through kr7-pmm-time-saved).

### Retro-logged 2026-05-18 work

Created two backdated entries so the system has real content from day one and the next Claude session (post-laptop-restart) can find what we did:
1. `2026-05-18-product-foundations-research.md` — the 13-book read
2. `2026-05-18-strategy-and-principles-doc.md` — the operating doc with 6 sourced decisions

Seeded `decision-log.md` with 8 rows total (7 from the strategy session + 1 for the cortex system itself).

## Decisions

- **decision-log #8** — use flat timestamped `chats/` + tag-based retrieval + single `decision-log.md`, **not** thread folders. User rationale: folders force pre-categorization that doesn't match overlapping reality of real conversations.

## Artifacts

- **Created:** `chats/README.md` (convention), `decision-log.md` (with 8 seeded rows), 3 chat entries (2 retro + this one)
- **Updated:** `MEMORY.md` (pointer to chats/ system)
- **Referenced:** strategy-and-principles.md as the anchor doc that everything traces back to

## Open questions / next steps

- **Weekly journal?** Initially proposed but skipped — start without it; add if `chats/` alone proves insufficient for retrospective scanning. The chats themselves are date-ordered already.
- **Zeropearl migration?** Left in `investor-conversations/` for now — that parallel chat decides if/when to adopt the convention. A future entry can simply tag-reference the existing file.
- **Tag vocabulary convergence** — current list is a seed; we'll codify a canonical set after ~20 entries, once natural patterns emerge.
- **Automation** — at some point worth a hook that auto-creates a chat-entry template at session end. Premature now; revisit at team-of-3+.

## Notes

**The thing the user got right that I almost missed:** real conversations are inherently multi-topic. The Zeropearl chat touches fundraising AND positioning AND pricing AND moat thesis. Forcing it into one folder destroys the cross-cutting nature; tags preserve it.

**The minimum viable system is what we built today**, not a heavier setup. Three files (decision-log, README, this entry) + 2 retro entries. About 90 minutes of work. The hard part wasn't building — it was the user's correction that turned a folder-based design into a tag-based one. That correction probably saves 20+ hours of "moving files around" friction over the next year.

**Test for the system right now:** when you close this laptop and open it tomorrow (or open a fresh Claude chat on another laptop), saying *"where were we?"* should produce: MEMORY.md auto-loads → Claude reads the latest 1–3 chats in `chats/` → resumes with full context. We'll see if that's true on the next session.
