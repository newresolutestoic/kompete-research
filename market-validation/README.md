# Market Validation Research

Structured research to validate (or invalidate) the Kompete CI thesis. Built over 5 research tasks between 2026-05-03 and 2026-05-11.

## Folder Structure

```
kompete-research/
│
├── objection-playbook.md                  ← SINGLE SOURCE for all 21 objections (A-E categories)
│
├── market-validation/                     ← Evidence base for all research
│   │
│   ├── README.md                          ← You are here
│   ├── methodology.md                     ← How we searched, why these sources, what we excluded
│   │
│   ├── issue-trees/                       ← MECE reasoning structures (7 files)
│   │   │
│   │   │  OBJECTION HANDLING (Task 1-2)
│   │   ├── objection-1-customers-not-competitors.md   ← "Focus on customers" → false dichotomy
│   │   ├── objection-2-process-is-fulcrum.md          ← "Process matters more" → CI is a process input
│   │   ├── objection-3-why-not-chatgpt.md             ← "ChatGPT can do this" → handles 40%, fails at 60%
│   │   │
│   │   │  INVESTOR THESIS (Task 3)
│   │   ├── investor-thesis-ci-market.md               ← 10 dimensions. Viable but narrow. 5 conditions.
│   │   │
│   │   │  CONVERSION FAILURE (Task 4)
│   │   ├── task4-why-ci-tools-fail-to-convert.md      ← 7-barrier compound model. ~2% conversion.
│   │   │
│   │   │  PRODUCT FORM FACTOR (Task 5)
│   │   └── task5-product-form-factor.md               ← AI-native autopilot, not dashboard. 7 design principles.
│   │
│   └── sources/                           ← Raw evidence (20 files, one per source)
│       │
│       │  OBJECTION EVIDENCE
│       ├── src-management-science-kim-2025.md          ← RCT, 3,218 firms, +4.8% revenue (CAUSAL)
│       ├── src-klue-competitive-revenue-gap-2025.md    ← 313 leaders, 21% deals lost, 33% winnable
│       ├── src-crayon-state-of-ci-2025.md              ← 8th annual, 68% competitive, 59% battlecard lift
│       ├── src-clozd-win-loss-analysis.md              ← 1,000+ deals, CRM wrong 70%, 84% see win rate lift
│       ├── src-gong-labs-competitive-deals.md           ← 1.8M deals, 49% higher close rate with early CI
│       ├── src-amazon-ci-operations.md                  ← 310+ CI roles, crawlers, GIP program
│       ├── src-strategic-theory-porter-christensen-blueocean.md  ← All 3 frameworks require CI
│       ├── src-chatgpt-ci-limitations.md                ← Hallucination test, 14-day lag, 40-30-30 rule
│       ├── src-meddpicc-competition.md                  ← Competition = required element
│       ├── src-battlecard-effectiveness.md              ← 71% see lift, but only 26% adoption
│       ├── src-saas-benchmarks-budgets.md               ← S&M 31-40% of ARR, CI budget context
│       │
│       │  INVESTOR THESIS EVIDENCE
│       ├── src-klue-funding-layoffs-2025.md             ← $81M raised, 40% laid off, CEO: "losing to ChatGPT"
│       ├── src-ci-market-sizing.md                      ← TAM $0.6-0.9B, adjacent $6-12B
│       ├── src-competition-intensifying-thesis.md       ← 70K+ SaaS, 64% CEOs say barriers lowering
│       ├── src-vc-ai-native-thesis.md                   ← a16z, Sequoia, Bain, Moonshot frameworks
│       ├── src-ci-bear-case.md                          ← Bundling, funding drought, category risk
│       ├── src-gartner-forrester-ci-analysts.md         ← Inaugural MQ Apr 2026, AlphaSense $500M ARR
│       ├── src-adjacent-tools-ci-expansion.md           ← Gong, Clari+Salesloft, HubSpot threat assessment
│       ├── src-ci-tool-churn-reasons.md                 ← G2 reviews, buyer-user mismatch, structural churn
│       ├── src-india-ci-market.md                       ← Contify $8.2M bootstrapped, India white space
│       │
│       │  CONVERSION + PRODUCT FORM EVIDENCE
│       ├── src-ci-conversion-failure-structural.md      ← 7 barriers, compound funnel math
│       └── src-ai-native-product-form-factor.md         ← Push/pull, agent UX, embedded, pricing models
│
├── interviews/             (27 files)     ← Original customer discovery transcripts
├── synthesis/                             ← Pain points, personas, key themes, extracts
└── investor-decks/                        ← Investor materials
```

## How This Connects to Other Documents

| Document | Location | What it contains |
|----------|----------|-----------------|
| **Objection Playbook** | `../objection-playbook.md` | All 21 objections, categorized A-E, with dates/sources/evidence |
| **Strategic War Room** | `../../kompete-website/research/synthesis/strategic-war-room.md` | Mission, vision, personas, pitches, marketing framework, discussion log |
| **Product Module Status** | `../../.claude/.../memory/synthesis/product-module-status.md` | Which frontend modules are live vs dummy data |
| **MVP Demo Plan** | `../../.claude/.../memory/synthesis/mvp-demo-plan.md` | 3-phase plan for demo-ready MVP |
| **CI Thesis Analysis** | `../../.claude/.../memory/synthesis/ci-thesis-analysis.md` | Working synthesis with full MECE tree |
| **Product-Tabs Revenue Mapping** | `../../kompete-website/product-tabs-revenue-mapping.md` | Every product tab mapped to revenue impact |
| **Cold Start Principles** | `../../kompete-website/cold-start-problem-principles.md` | Chen + Godin GTM framework |

## Research Task Summary

| Task | Question | Verdict | Key Finding |
|------|----------|---------|-------------|
| 1 | "Focus on customers, not competitors" | False dichotomy | CI IS customer focus. Christensen warns AGAINST pure customer obsession. Amazon has 310+ CI roles. |
| 2 | "Process is the fulcrum" | CI is a process input | MEDDPICC requires Competition. 85% of CRM data is wrong. Process on bad data = blind process. |
| 3 | Is CI a viable investment? | Viable but narrow (5 conditions) | $0.6-0.9B standalone market. Klue stalling. Must be AI-native, expand into sales enablement, solve adoption. |
| 4 | Why don't people buy? | 7-barrier compound model | ~2% conversion from validated pain. Vitamin + attribution + urgency + buyer + DIY + adoption + category = death. |
| 5 | What should the product feel like? | Autopilot agent, not dashboard | No primary UI. Push to Slack/CRM/email. Zero behavioral change. $299-499/mo. Outcome-based expansion. |

## Process (Repeatable)

When validating any new thesis or objection:

1. **Frame** — Write the question precisely
2. **Decompose** — Break into MECE dimensions
3. **Search** — Academic papers, industry reports (Klue/Crayon/Clozd/Gong), practitioner blogs, VC theses
4. **Log** — Create source file in `sources/` with URL, date, bias note, key data, which tree node it supports
5. **Synthesize** — Build issue tree in `issue-trees/` linking each leaf to sources
6. **Update** — Add to objection playbook if applicable
7. **Revise** — Flashcards for ongoing revision
