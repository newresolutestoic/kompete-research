# Research Methodology

## How we searched and why these sources

### The search strategy

For each MECE dimension, we searched for evidence at three levels of credibility:

```
Level 1 (Highest): Academic / peer-reviewed
  → Management Science, HBS publications, Christensen Institute
  → Only 1 source qualified (Kim 2025 RCT) — CI is under-researched academically

Level 2 (Strong): Large-N industry reports from established firms
  → Klue (313 leaders), Crayon (8th annual report), Clozd (1,000+ deals), Gong (1.8M deals)
  → These have large sample sizes but vendor bias — cross-referenced against each other

Level 3 (Supporting): Practitioner analysis, case studies, job posting data
  → Amazon CI jobs (LinkedIn), GTMnow, Parano.ai case study
  → Used for specific examples and revealed preference, not statistical claims
```

### Why these specific sources and not others

| Source | Why included | What it uniquely provides |
|--------|-------------|--------------------------|
| Management Science (Kim) | Only RCT in CI. Causal evidence, not correlation. | Proves competitor info → revenue. No other source can claim causation. |
| Klue Revenue Gap Report | Largest recent survey of revenue leaders on competitive dynamics | Specific deal-loss percentages, rep preparedness data, CS vulnerability |
| Crayon State of CI | Longest-running annual report (8 editions). Trend data. | Practice-level correlations: daily engagement, battlecard frequency, sponsor impact |
| Clozd | Unique methodology: compares CRM data vs actual buyer interviews | Proves CRM data is wrong 70% of time. No other source has this comparison. |
| Gong Labs | 1.8M real deals. Largest dataset of actual sales conversations. | Behavioral data from calls, not self-reported surveys. Early vs late competitor mention. |
| Amazon CI operations | Most-cited "customer obsession" company. Their actual CI practice. | Kills the Bezos objection with Amazon's own job postings. |
| MEDDPICC documentation | Most respected enterprise sales methodology. | Proves CI is a required process input, not an alternative to process. |
| ChatGPT limitation sources | Documented failure cases, not theoretical arguments. | Klue's hallucination test, Parano.ai's 14-day lag case, Gartner's 52% fabrication stat. |

### What we deliberately excluded

| Excluded | Why |
|----------|-----|
| Generic "CI is important" blog posts | No data, no sample size, no methodology. Opinions disguised as evidence. |
| Klue/Crayon marketing pages | Vendor landing pages are sales collateral, not research. Used their REPORTS, not their marketing. |
| Pre-2021 studies | AI has changed CI economics. Pre-LLM data on CI tool adoption is misleading. |
| Competitor funding announcements | "Klue raised $X" proves investor belief, not customer value. Saved for Task 3 (investor thesis). |
| Reddit/HN anecdotes | Used for signal detection only, never as evidence for a claim. |

### Bias acknowledgment

**3 of 5 major data sources are CI vendors** (Klue, Crayon, Clozd). Their data likely overstates CI value. We mitigated this by:

1. Cross-referencing vendor claims against each other (Klue's 21% deal loss vs Crayon's 68% competitive deals — different metrics, consistent story)
2. Prioritizing the ONE academic source (Management Science RCT) as the anchor
3. Using Gong (revenue intelligence, not CI vendor) as an independent data point
4. Using Amazon (not a CI vendor at all) as the behavioral evidence
5. Flagging vendor bias explicitly in each source file

### Search queries used

**Objection 1 (Customers vs Competitors):**
- "Porter Five Forces competitor monitoring importance"
- "Christensen disruption theory customer focus"
- "Blue Ocean Strategy competitor analysis required"
- "Amazon competitive intelligence jobs LinkedIn"
- "Amazon Global Intelligence Program"
- "Bezos customer obsessed competitor aware"
- "competitive intelligence revenue impact study"
- "win loss analysis ROI data"
- "B2B SaaS deals lost to competitors percentage"
- "competitive intelligence customer retention"

**Objection 2 (Process vs Intelligence):**
- "what drives B2B SaaS win rates data"
- "Gong research competitive deal win rate"
- "MEDDPICC competition element"
- "sales process competitive intelligence integration"
- "battlecard effectiveness win rate data"
- "B2B SaaS spending benchmarks 2025"
- "when do companies hire competitive intelligence"
- "Sun Tzu foreknowledge business strategy"
- "B2B buyer research before sales contact"

**Objection 3 (ChatGPT):**
- "ChatGPT competitive intelligence limitations"
- "ChatGPT hallucination competitive data"
- "AI competitive analysis vs dedicated CI tool"
- "ChatGPT competitor pricing accuracy"
- "Gartner AI hallucination rate enterprise"
- "competitive intelligence AI automation percentage"

### How to replicate or extend

To add a new objection or update existing evidence:

1. Start with the highest-credibility sources first (academic, then large-N reports)
2. Search for COUNTER-evidence, not just supporting evidence
3. Create a source file in `sources/` with: URL, date accessed, type, bias note, key data points, and which tree node it supports
4. Update the relevant issue tree in `issue-trees/`
5. If the new evidence changes a verdict, update `conclusion-and-verdict.md`
