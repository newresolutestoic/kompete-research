---
date: 2026-05-18
title: Drafted strategy-and-principles.md — the operating doc synthesizing 13 books + 27 interviews
tags: [strategy, principles, foundations, synthesis, decision, moat, beachhead, positioning, pricing, gtm, outcomes, meta]
outcomes-touched: [kr1-pilots, kr2-references, kr3-win-rate, kr4-adoption, kr5-trigger-precision, kr6-commercial, kr7-pmm-time-saved]
artifacts:
  created:
    - kompete-research/strategy-and-principles.md
  updated:
    - memory/MEMORY.md
  referenced:
    - memory/product-foundations/ (all 16 files)
    - kompete-research/market-validation/issue-trees/task5-product-form-factor.md
    - kompete-research/synthesis/ci-thesis-analysis.md
    - kompete-research/synthesis/mvp-demo-plan.md
related-chats: [2026-05-18-product-foundations-research]
chat-source: claude-code-cli
status: live
---

# strategy-and-principles.md — the operating doc

## Context

After 13 foundation books surfaced 7 convergent conclusions, the next move was to compress those into one operating document — the artifact every hire reads, every design decision is tested against, and every investor conversation references. The doc had to be specific enough to be useful, brief enough to be read, and durable enough to last years.

## Work done

Drafted `kompete-research/strategy-and-principles.md` — 10 sections:

| § | Content |
|---|---|
| I | Strategy Stack (Perri) — Vision, Strategic Intent, Y1 Product Initiative, current Options & Tests |
| II | The Beachhead (Moore) — precise customer definition + Whole Product non-negotiables |
| III | Positioning Statement (Dunford) — 5-component format + Sales-VP buyer reframe + category posture |
| IV | The Seven First Principles — durable tie-breakers with "what this rules out" clauses |
| V | Moat Thesis (Helmer) — Counter-Positioning primary, Cornered Resource secondary, what we don't claim |
| VI | Year-1 Outcome OKRs — 7 KRs, all outcomes, zero feature counts |
| VII | Operating Disciplines — weekly/monthly cadences from Torres + Perri + Cagan + Fitzpatrick + Eyal |
| VIII | "We Don't Do This" List — 11 explicit no's, each justified by a principle |
| IX | What Changes This Doc — update triggers vs deliberately resistant |
| X | Where this fits — map to other artifacts |

## Decisions

This session produced **6 durable decisions** — all logged in `decision-log.md`:

- **decision-log #1** — adopt the 7 first principles
- **decision-log #2** — Y1 success = 5 pilots + 3 references + ≥10pp win-rate (not "MVP shipped")
- **decision-log #3** — primary moat = Counter-Positioning against Klue/Crayon; secondary = aggregate-intel data network
- **decision-log #4** — beachhead = $10–30M ARR Series B B2B SaaS sales orgs with specific tech-stack + pain criteria
- **decision-log #5** — category = dominate subsegment Y1–2; plant Deal Intelligence category seeds for Y2+
- **decision-log #6** — buyer reframe to Sales VP (not PMM); language reframe to deal intelligence

Plus one **open decision (#7)** — pricing tier hypothesis ($0/$799/$1499/Enterprise) pending WTP-conversation validation.

## Artifacts

- **Created:** `kompete-research/strategy-and-principles.md` (the operating doc; ~4 pages dense)
- **Updated:** `memory/MEMORY.md` — added pointer under new "Operating Documents" section
- **Referenced:** all 16 product-foundations files, Task 5, CI thesis, MVP plan

## Open questions / next steps

The strategy doc itself names 5 immediate downstream consequences. In priority order:

1. **Rewrite `mvp-demo-plan.md`** to outcome-language per §VI of strategy doc (the phase/feature structure is the highest-priority inconsistency)
2. **Mom-Test audit of 27 interviews** to separate concrete past behavior from "would-you-pay" fluff
3. **Run 10 WTP conversations** to validate (and likely raise) the pricing tier hypothesis
4. **Write "Why won't Klue copy us?" one-pager** to pressure-test Counter-Positioning
5. **Build a live Opportunity Solution Tree** + adopt the Product Kata weekly cadence

The strategy doc is the *anchor* — these are the artifacts that need to align with it next.

## Notes

The 7 First Principles were the hardest section to draft. The discipline was: each principle has to (a) be durable for years, (b) actually rule out specific decisions (which is why each one has an explicit "this rules out" clause), and (c) compress a foundation-book lesson into a sentence a hire can recite from memory.

The final 7:
1. The customer outcome is the win condition.
2. If a user has to log in, we failed.
3. Silence between triggers.
4. Deliver the answer, not the data.
5. Attribution is built in, not bolted on.
6. Every customer request becomes a problem before it becomes a backlog item.
7. Would we be embarrassed if the competitor saw exactly what we scraped about them?

These are designed to outlast every other decision in the doc. The vision can be revised; these shouldn't be — unless a foundational mistake is found.
