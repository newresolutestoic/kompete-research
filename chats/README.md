# Kompete — Chats Log

> **What this is:** a flat, timestamped log of every meaningful Claude (or other) conversation that produced an artifact, decision, or substantive analysis for Kompete. Retrieval is by **tag**, not by folder.
>
> **Why this exists:** to make the institutional memory of Kompete *queryable in 1–2 years*. Without it, every chat evaporates when the window closes.

---

## The convention

### 1. One file per meaningful conversation

Filename format: `YYYY-MM-DD-<short-slug>.md`

If multiple conversations happen on the same day, add a time suffix: `YYYY-MM-DD-HHMM-<slug>.md`. Slug is 2–5 words, kebab-case, descriptive.

Examples:
- `2026-05-18-product-foundations-research.md`
- `2026-05-19-operating-cortex-system.md`
- `2026-05-19-1430-pricing-wtp-conversations.md`

### 2. Frontmatter is the retrieval index

Every entry starts with this block:

```yaml
---
date: YYYY-MM-DD
title: <human-readable title>
tags: [tag1, tag2, ...]                  # free-form, multi-tag
outcomes-touched: []                     # Y1 KRs from strategy-and-principles.md, if any
artifacts:
  created: []                            # files created in this chat
  updated: []                            # files updated
  referenced: []                         # files read but not modified
related-chats: []                        # other entries this builds on
chat-source: claude-code-cli | other
status: live | superseded | archived
---
```

Anything that isn't relevant can be omitted or left as `[]`.

### 3. Standard body sections

```markdown
## Context
1–3 sentences: what problem were we working on, why.

## Work done
Bullets: what happened in the chat.

## Decisions
- Each durable decision → mirrored as a row in `../decision-log.md`.
  Reference the decision-log row number.

## Artifacts
- **Created:** [filenames + 1-line description each]
- **Updated:** [filenames]
- **Referenced:** [filenames]

## Open questions / next steps
- What's unresolved or queued for the next session.

## Notes (optional)
- Anything else: reasoning, surprises, things that turned out wrong.
```

### 4. Tag vocabulary (extend over time)

Tags are free-form. These are the ones already in use — add new ones liberally; we'll converge by practice.

**Domain tags:**
- `product` — form factor, MVP, discovery, prototyping
- `gtm`, `positioning`, `messaging`, `category`
- `pricing`, `monetization`, `wtp`, `tiers`
- `fundraising`, `investor`, `narrative`, `deck`
- `pilot-recruiting`, `design-partners`
- `hiring`, `coaching`, `team`
- `ops`, `legal`, `infra`, `finance`
- `market-intel`, `klue`, `crayon`, `ema`, `competitor-watch`
- `discovery`, `interviews`, `mom-test`, `wtp-study`

**Concept tags (from foundations):**
- `counter-positioning`, `moat`, `7-powers`
- `whole-product`, `chasm`, `beachhead`
- `hook-model`, `triggers`, `investment-loop`
- `outcome-vs-output`, `product-kata`, `ost`
- `atomic-network`, `network-effects`, `cold-start`
- `build-trap`, `strategy-stack`
- `mom-test`, `commitment-currency`
- `anchoring`, `decoy`, `endowment`
- `affordance`, `signifier`, `two-gulfs`

**Operational tags:**
- `decision` — produced a durable decision
- `draft` — produced a draft (deck, email, doc)
- `research` — gathered external information
- `synthesis` — cross-cutting analysis
- `meta` — about the system itself, not the business
- `open-question` — unresolved at session end

**Outcome tags (link to Y1 KRs):**
- `kr1-pilots`, `kr2-references`, `kr3-win-rate`
- `kr4-adoption`, `kr5-trigger-precision`
- `kr6-commercial`, `kr7-pmm-time-saved`

---

## The protocol

### When a Claude session starts

1. `MEMORY.md` auto-loads (existing behavior).
2. If you reference a topic, Claude will optionally grep `chats/` for relevant past entries and read them for context.
3. Just opening a fresh chat with "where were we?" → Claude reads the most recent 1–3 entries in `chats/`.

### When a Claude session ends with meaningful work

1. Claude invokes the **`chat-logger` subagent** (defined at `~/.claude/agents/chat-logger.md`) — *or* the user invokes it explicitly by saying "log this," "save session," "log to chats," etc.
2. The agent reads this convention, generates the frontmatter, writes the timestamped entry, appends rows to `decision-log.md` if durable decisions were made, and reports back what it did.
3. The agent updates `MEMORY.md` only if the session materially changes how future sessions should be oriented.

The agent runs on Haiku (cheap, fast, structured-extraction work). Invocation is via the parent session's `Agent` tool with `subagent_type: chat-logger`.

### When you're running parallel chats

Each chat writes to its own timestamped file. Overlapping topics get the same tags; that's fine and expected. The Zeropearl-VC chat continues at its existing path (`investor-conversations/zeropearl-vc-jai.md`) until that parallel chat opts into the new system on its own.

### When you want to retrieve something later

The lookup mental model:
- **"What did we decide about X?"** → grep `tags: X` in `chats/*.md`; OR look at `../decision-log.md`.
- **"What was happening last week / last month?"** → ls `chats/` filtered by date; read in order.
- **"How did our pricing thinking evolve?"** → grep `tags: pricing`; read entries chronologically.
- **"What touched KR3 (win-rate)?"** → grep `outcomes-touched:.*kr3`.

---

## What's NOT in here

`chats/` is for *conversation logs*. It is not where artifacts live.

| Artifact type | Lives in |
|---|---|
| Conversation log | `chats/` (this folder) |
| The operating doc | `strategy-and-principles.md` |
| Durable decisions | `decision-log.md` |
| Customer interviews | `interviews/` |
| Synthesis (issue trees, MECE analyses) | `synthesis/` and `market-validation/issue-trees/` |
| Investor conversations (drafts, reply emails) | `investor-conversations/` |
| Reference reading (books) | `~/.claude/projects/-Users-main-Documents-Kompete/memory/product-foundations/` |
| Auto-loaded index for Claude | `~/.claude/projects/-Users-main-Documents-Kompete/memory/MEMORY.md` |

A chat entry *references* the artifacts it produced/modified via the frontmatter and the Artifacts section. The artifacts themselves stay in their canonical location.

---

## How to look back in 1–2 years

In 18 months you'll want to ask things like:
- *"When did we first realize the Klue counter-positioning thesis was load-bearing?"*
- *"What customer pushback shaped the trigger-precision threshold?"*
- *"Did we ever discuss enterprise expansion before Q3 2026?"*

The answer to each is: grep + read. The tagging discipline today is what makes those answers retrievable then.

---

*Convention version: v1, established 2026-05-19. Revise as it gets used.*
