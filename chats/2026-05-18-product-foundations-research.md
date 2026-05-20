---
date: 2026-05-18
title: Product foundations research — 13 books across product/pricing/GTM/strategy
tags: [foundations, product, pricing, gtm, positioning, moat, discovery, research, synthesis]
outcomes-touched: []
artifacts:
  created:
    - memory/product-foundations/cagan-1-inspired.md
    - memory/product-foundations/cagan-2-empowered.md
    - memory/product-foundations/cagan-3-transformed.md
    - memory/product-foundations/cagan-kompete-synthesis.md
    - memory/product-foundations/hooked-eyal.md
    - memory/product-foundations/design-of-everyday-things-norman.md
    - memory/product-foundations/predictably-irrational-ariely.md
    - memory/product-foundations/cold-start-problem-chen.md
    - memory/product-foundations/mom-test-fitzpatrick.md
    - memory/product-foundations/continuous-discovery-habits-torres.md
    - memory/product-foundations/monetizing-innovation-ramanujam-tacke.md
    - memory/product-foundations/pricing-roadmap-lehrskov-schmidt.md
    - memory/product-foundations/obviously-awesome-dunford.md
    - memory/product-foundations/crossing-the-chasm-moore.md
    - memory/product-foundations/7-powers-helmer.md
    - memory/product-foundations/escaping-the-build-trap-perri.md
  updated:
    - memory/MEMORY.md
  referenced:
    - kompete-research/market-validation/issue-trees/task5-product-form-factor.md
    - kompete-research/synthesis/ci-thesis-analysis.md
    - kompete-research/synthesis/mvp-demo-plan.md
related-chats: []
chat-source: claude-code-cli
status: live
---

# Product foundations research — 13 books

## Context

Before diving deeper into form-factor decisions, we read the canonical product literature to pressure-test the work we had so far (Task 5 form factor + CI thesis + 27 interviews). Goal: catch foundation-level mistakes before code is written. Two days of research; 13 books summarized; each filtered through a "Kompete: are we doing this?" gap audit.

## Work done

Three batches of book research, sourced from SVPG / Lenny's Newsletter / reputable summary sites (SVPG itself 403s automated fetches; worked around via secondary sources).

**Batch 1 (Cagan trilogy + synthesis):**
- INSPIRED (Cagan, 2017) — discovery vs delivery, 4 risks (value/usability/feasibility/viability), missionaries vs mercenaries, 10 root causes of failed products
- EMPOWERED (Cagan & Jones, 2020) — coaching, staffing, vision/topology/strategy framework, OKRs, 5th risk (ethics)
- TRANSFORMED (Cagan + 4 co-authors, 2024) — product operating model, 20 first principles in 5 categories, 3 dimensions of change, transformation playbook
- Cross-book synthesis applied to Kompete — outcome-vs-feature reframe of Task 5; 16-row anti-pattern audit (2 confirmed gaps, 8 future risks); 5 leveraged next moves

**Batch 2 (UX & behavioral econ):**
- HOOKED (Eyal, 2014) — Hook Model (Trigger → Action → Variable Reward → Investment); Fogg B=MAT; 6 elements of ability; tribe/hunt/self rewards; Habit Zone; Manipulation Matrix
- The Design of Everyday Things (Norman, 1988/2013) — affordances, signifiers, mappings, feedback, conceptual model; two gulfs (execution & evaluation); seven stages of action; design for error
- Predictably Irrational (Ariely, 2008) — relativity/decoy, anchoring, FREE, social vs market norms, endowment, doors-open, expectations, price-as-placebo
- The Cold Start Problem (Andrew Chen, 2021) — 5 stages, atomic network, hard side, magic moment, three flywheels, moat

**Batch 3 (idea validation / pricing / GTM / strategy):**
- The Mom Test (Fitzpatrick, 2013) — concrete past behavior > opinions; commitment currencies; compliments-as-noise; advancement test
- Continuous Discovery Habits (Torres, 2021) — weekly customer touchpoints, opportunity solution tree, product trio, assumption testing, story-based interviewing, interview snapshots
- Monetizing Innovation (Ramanujam & Tacke, 2016) — 4 failure modes (Minivation = our biggest risk), 9 rules, Van Westendorp WTP questions, Leaders/Fillers/Killers packaging
- The Pricing Roadmap (Lehrskov-Schmidt, 2023) — CUPID framework, pricing metric > price level, fencing & laddering, discounting policy
- Obviously Awesome (Dunford, 2019) — 5-component positioning, subsegment vs new-category strategy, status-quo as competitor
- Crossing the Chasm (Moore, 1991) — adoption lifecycle, D-Day/beachhead, whole product, 3 named-public references in 6 months as #1 GTM goal
- 7 Powers (Helmer, 2016) — 7 sources of Power (Benefit + Barrier); Counter-Positioning identified as Kompete's primary moat candidate; Cornered Resource as secondary
- Escaping the Build Trap (Perri, 2018) — Strategy Stack, Product Kata, three ingredients (strategy + process + org)

## Decisions

No durable decisions in this session — this was research that *informed* the next session's decisions (see [2026-05-18-strategy-and-principles-doc](2026-05-18-strategy-and-principles-doc.md)).

## Artifacts

- **Created:** 16 reference files in `memory/product-foundations/` (13 book summaries + Cagan synthesis + 2 sub-summaries within Cagan)
- **Updated:** `memory/MEMORY.md` — added "Product Foundations" section with all 16 pointers
- **Referenced:** existing Task 5, CI thesis, MVP plan, 27 interviews

## Open questions / next steps

Surfaced for the next session:
- 27 interviews need Mom-Test audit (concrete past behavior vs fluff)
- $299–499 pricing is likely Minivation; need WTP conversations to re-anchor
- Task 5 design rules should be promoted to first-class principles
- MVP plan needs outcome-language rewrite
- "Why won't Klue copy us?" Counter-Positioning thesis needs explicit pressure-test
- Whole Product gap (battlecard library, onboarding, CS motion) is bigger than current planning
- 3 named-public-reference customers in 6 months should be the #1 GTM goal — above feature velocity

## Notes

**The convergence is the headline.** All 13 books, read independently and 8 different domain perspectives, point at the same handful of conclusions for Kompete:

1. Outcomes > outputs (Cagan, Torres, Perri — said three different ways)
2. Pricing is a behavioral-design problem, not finance (Ramanujam, Lehrskov-Schmidt, Ariely)
3. Concrete past behavior > stated intent (Fitzpatrick; Torres operationalizes it)
4. Pragmatists buy whole products; visionaries buy core tech (Moore, Cagan)
5. Counter-Positioning is the moat that matters at our stage (Helmer)
6. Position as "deal intelligence" (Sales VP buyer) not "CI" (PMM buyer) (Dunford, Cagan)
7. Atomic network = 1 sales team; concierge the hard side (Chen, Moore)

When 13 independent authors converge on the same 7 conclusions, that's strong signal.
