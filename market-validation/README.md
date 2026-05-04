# Market Validation Research

Structured research to validate (or invalidate) the Kompete CI thesis.

## Folder Structure

```
market-validation/
│
├── README.md                          ← You are here. Index + methodology.
│
├── issue-trees/                       ← MECE issue trees (the reasoning structure)
│   ├── objection-1-customers-not-competitors.md
│   ├── objection-2-process-is-fulcrum.md
│   ├── objection-3-why-not-chatgpt.md
│   └── investor-thesis-ci-market.md   ← Market viability: funding, sizing, bear case, AI-native angle
│
├── sources/                           ← Raw research evidence, one file per source
│   ├── src-management-science-kim-2025.md      ← RCT, 3,218 firms
│   ├── src-klue-competitive-revenue-gap-2025.md ← 313 revenue leaders
│   ├── src-crayon-state-of-ci-2025.md           ← 8th annual report
│   ├── src-clozd-win-loss-analysis.md           ← 1,000+ deals analyzed
│   ├── src-gong-labs-competitive-deals.md       ← 1.8M opportunities
│   ├── src-amazon-ci-operations.md              ← The Bezos paradox
│   ├── src-strategic-theory-porter-christensen-blueocean.md
│   ├── src-chatgpt-ci-limitations.md            ← Hallucination cases
│   ├── src-meddpicc-competition.md              ← CI in sales methodology
│   ├── src-battlecard-effectiveness.md          ← Adoption gap data
│   ├── src-saas-benchmarks-budgets.md           ← Budget/headcount data
│   ├── src-klue-funding-layoffs-2025.md         ← $81M raised, 40% layoffs, CEO quotes
│   ├── src-ci-market-sizing.md                  ← TAM/SAM from Mordor, Fortune BI, MRCF
│   ├── src-competition-intensifying-thesis.md   ← 70K+ SaaS cos, AI barriers, vendor growth
│   ├── src-vc-ai-native-thesis.md               ← a16z, Sequoia, Bain, Moonshot frameworks
│   ├── src-ci-bear-case.md                      ← Bundling risk, funding drought, adoption
│   ├── src-gartner-forrester-ci-analysts.md     ← Inaugural Gartner MQ Apr 2026, Forrester Wave Q4 2024
│   ├── src-adjacent-tools-ci-expansion.md       ← Gong, Clari+Salesloft, HubSpot, Salesforce CI features
│   ├── src-ci-tool-churn-reasons.md             ← G2/Gartner reviews, churn root causes, buyer-user mismatch
│   └── src-india-ci-market.md                   ← Contify ($8.2M bootstrapped), India white space
│
└── methodology.md                     ← How we searched, why these sources, what we excluded
```

## How This Connects to Other Research

- `../interviews/` — 27 customer discovery interviews (primary research)
- `../synthesis/` — Pain points, personas, key themes from interviews
- `../../kompete-website/product-tabs-revenue-mapping.md` — Product → revenue impact mapping
- `../../kompete-website/cold-start-problem-principles.md` — GTM strategy (Chen + Godin)
- `../../.claude/.../memory/synthesis/` — Session memory: MVP plan, module status, CoStar prompts

## Process (Repeatable)

When validating any new thesis or objection:

1. **Frame** — Write the objection as a precise question
2. **Decompose** — Break into MECE dimensions (theory, evidence, behavior, reframe)
3. **Search** — For each dimension, search for: academic papers, industry reports, practitioner blogs, founder perspectives
4. **Log** — Create a source file per source in `sources/` with URL, date accessed, key data points, and direct quotes
5. **Synthesize** — Build issue tree in `issue-trees/` linking each leaf to source files
6. **Verdict** — Roll up to conclusion in `conclusion-and-verdict.md`
7. **Revise** — Flashcards for ongoing revision, update when new evidence emerges
