# Kompete.ai — Objection Playbook

> Single source of truth for every objection encountered. Grouped by type. Each entry has: source, date, one-liner response, evidence, full response.
>
> Evidence links to `market-validation/sources/` for detailed citations.
>
> **Last updated:** 2026-05-04

---

## How to use this file

- **Before a call:** Ctrl+F the likely objection keywords. Read the one-liner + evidence.
- **During a call:** Use the one-liner. If pushed, cite 1-2 data points from evidence.
- **After a call:** If you hear a new objection, add it here with date + source.
- **Monthly:** Review open questions at the bottom. Update responses as thinking evolves.

---

## Table of Contents

### A. Category-Level Doubts ("Should CI even exist?")
- [A1. "Great companies focus on customers, not competitors"](#a1)
- [A2. "Process execution matters more than intelligence"](#a2)
- [A3. "Why not just use ChatGPT / Perplexity?"](#a3)

### B. Product & Value Objections ("Why THIS product?")
- [B1. "How is this different from Perplexity / Deep Research?"](#b1)
- [B2. "Static vs Dynamic — only dynamic info is worth paying for"](#b2)
- [B3. "Will I pay for it? Information vs business value"](#b3)
- [B4. "Enterprise data doesn't change frequently"](#b4)
- [B5. "Signal vs noise — AI gives surface-level answers"](#b5)
- [B6. "AI should discover competitors, not the user"](#b6)
- [B7. "Customer voice should inform CI, not just competitor tracking"](#b7)
- [B8. "Sales team already knows faster than public data"](#b8)
- [B9. "Make me open your dashboard twice a day"](#b9)
- [B10. "Trigger events drive deep analysis, not continuous monitoring"](#b10)

### C. GTM & Buyer Objections ("Who buys this?")
- [C1. "Buyer vs user persona confusion — who owns the budget?"](#c1)
- [C2. "ROI justification is hard for PMM"](#c2)
- [C3. "Spreading too thin on user personas"](#c3)
- [C4. "Target founders first — they'll pull in teams"](#c4)
- [C5. "SME market won't pay (India)"](#c5)
- [C6. "Sell outcomes, not capabilities"](#c6)

### D. Competitive Moat Objections ("What stops someone else?")
- [D1. "Lock-in problem — what stops someone using Glean?"](#d1)

### E. Pricing Objections
- [E1. "Low subscription, usage-heavy pricing"](#e1)
- [E2. "Figure out who/why/what they'll pay — before building"](#e2)

---

## A. CATEGORY-LEVEL DOUBTS

These are not product objections. They question whether competitive intelligence as a category deserves investment. Must be answered before any product conversation.

---

<a id="a1"></a>
### A1. "Great companies focus on customers, not competitors"

| | |
|---|---|
| **Source** | Field conversations with founders during outreach (2026 Q1-Q2) |
| **Date first heard** | 2026 Q1 (recurring — most common category-level pushback) |
| **Who says this** | Founders, CEOs, occasionally VPs of Product |
| **Frequency** | Very high — comes up in nearly every founder conversation |
| **Type** | Category-level doubt |

**One-liner response:**
> "Agreed — your customers are everything. That's exactly why you need to know when a competitor is targeting them. Only 40% of CS teams can detect when a competitor shows up in a renewal."

**Evidence (sourced):**

| Claim | Data | Source |
|-------|------|--------|
| Every framework cited actually REQUIRES competitive awareness | Porter = competitive structure; Christensen = companies die from over-focusing on customers; Blue Ocean = Strategy Canvas maps against competitors | [src-strategic-theory](market-validation/sources/src-strategic-theory-porter-christensen-blueocean.md) |
| Amazon says "customer obsessed" but runs massive CI operation | 310+ CI roles on LinkedIn; crawlers on competitor websites; Global Intelligence Program | [src-amazon-ci](market-validation/sources/src-amazon-ci-operations.md) |
| Competitive info causally improves revenue | RCT across 3,218 firms: +4.8% revenue, +8% customers | [src-management-science](market-validation/sources/src-management-science-kim-2025.md) |
| Deals lost to competitors | 21% of deals; 33% of those winnable = ~7% recoverable | [src-klue](market-validation/sources/src-klue-competitive-revenue-gap-2025.md) |
| CS teams can't detect competitive threats | Only 40% confident they can detect competitor presence in renewals | [src-klue](market-validation/sources/src-klue-competitive-revenue-gap-2025.md) |
| Customer retention = #1 revenue stream | 38% of revenue leaders say so | [src-klue](market-validation/sources/src-klue-competitive-revenue-gap-2025.md) |

**Full response:**

This is a false dichotomy. CI IS customer focus.

1. **Christensen's Innovator's Dilemma** says companies are disrupted precisely BECAUSE they over-focus on current customers and miss market shifts. The theory warns AGAINST pure customer obsession.

2. **Amazon** — the poster child for "customer obsession" — has 310+ competitive intelligence roles, runs automated crawlers on competitor websites, and purchases competitor products to benchmark fulfillment. "Customer obsessed" is their slogan. Competitor-aware is their operation.

3. **A randomized controlled trial** across 3,218 firms (Management Science, 2025) proved that receiving competitor information causes 4.8% revenue improvement. Half the firms didn't even know competitor prices before the study.

4. **The reframe:** "We don't help you obsess over competitors. We help you protect and win customers by knowing what they're comparing you to." 38% of revenue leaders say retention is their #1 priority — but only 40% are confident their CS team can detect when a competitor enters a renewal conversation.

**MECE issue tree:** [objection-1-customers-not-competitors.md](market-validation/issue-trees/objection-1-customers-not-competitors.md)

---

<a id="a2"></a>
### A2. "Process execution matters more than intelligence"

| | |
|---|---|
| **Source** | Field conversations with operators, VPs of Sales, COOs (2026 Q1-Q2) |
| **Date first heard** | 2026 Q1 (recurring — common from ops-minded leaders) |
| **Who says this** | VPs of Sales, COOs, RevOps leaders, process-oriented operators |
| **Frequency** | High — especially from companies that just implemented MEDDPICC or similar |
| **Type** | Category-level doubt |

**One-liner response:**
> "Your process is strong. But MEDDPICC literally has Competition as a required letter, and 85% of the competitive data in your CRM is wrong. That's not a process gap — it's an information gap."

**Evidence (sourced):**

| Claim | Data | Source |
|-------|------|--------|
| MEDDPICC requires Competition as a core element | Second "C" = Competition — any person, vendor, or initiative competing for same funds | [src-meddpicc](market-validation/sources/src-meddpicc-competition.md) |
| CRM competitive data is garbage | Wrong 70% of the time; buyer-seller reasons align only 15% | [src-clozd](market-validation/sources/src-clozd-win-loss-analysis.md) |
| Early competitive prep lifts close rates | 49% higher close rate when competitors discussed early | [src-gong](market-validation/sources/src-gong-labs-competitive-deals.md) |
| Late competitor detection = discounting | 47% of reps don't spot competitors until negotiation; only lever left = discount | [src-klue](market-validation/sources/src-klue-competitive-revenue-gap-2025.md) |
| Daily CI engagement = massive effectiveness lift | 84% increase in competitive sales effectiveness | [src-crayon](market-validation/sources/src-crayon-state-of-ci-2025.md) |
| Battle cards work but adoption is the problem | 71% see improved win rates, but only 26% of reps use them | [src-battlecard](market-validation/sources/src-battlecard-effectiveness.md) |

**Full response:**

Process and intelligence are not substitutes — CI is a required INPUT to process execution.

1. **MEDDPICC** — the most respected enterprise sales methodology — has Competition as a literal required element. You cannot execute MEDDPICC without competitive intelligence.

2. **85% of CRM closed-lost data is inaccurate** (Clozd, 1,000+ deals analyzed). Companies are optimizing their sales process based on wrong data. Better process with bad intelligence = efficiently losing deals you should've won.

3. **47% of reps** don't spot competitors until negotiation stage (Klue). By then, the shortlist is set, positioning is locked, and the only lever left is discounting — which means lower margins and smaller deals.

4. **The key insight:** The "process vs CI" objection is actually an objection to CI's FORM FACTOR. People don't want another dashboard to check. They want CI injected into the process they already run. This tells us HOW to build (embedded in CRM, pushed to Slack), not WHETHER to build.

**MECE issue tree:** [objection-2-process-is-fulcrum.md](market-validation/issue-trees/objection-2-process-is-fulcrum.md)

---

<a id="a3"></a>
### A3. "Why not just use ChatGPT / Perplexity?"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor, 2026-03-14), Siddharth Jain [LeadSquared] (coffee chat, 2026-02-19), field conversations |
| **Date first heard** | 2026-02-19 (Siddharth LS); confirmed as pattern 2026-03-14 (Sanchit) |
| **Who says this** | Technical founders, PMs, anyone who uses AI tools daily |
| **Frequency** | Very high — THE #1 pitch obstacle. Two independent operators asked unprompted. |
| **Type** | Category-level doubt |

**One-liner response:**
> "Try asking ChatGPT your competitor's current pricing — it'll confidently give you numbers that don't exist. We monitor changes in real-time, push to your team, and update battle cards automatically. ChatGPT makes one person smarter once. We make your whole org smarter continuously."

**Evidence (sourced):**

| Claim | Data | Source |
|-------|------|--------|
| ChatGPT fabricates competitor data | Klue test: fabricated detailed pricing tiers that don't exist; invented fake TechCrunch articles | [src-chatgpt](market-validation/sources/src-chatgpt-ci-limitations.md) |
| Enterprise AI hallucination rate | 52% of responses contain fabrications (Gartner, 2024) | [src-chatgpt](market-validation/sources/src-chatgpt-ci-limitations.md) |
| Detection lag vs real-time monitoring | 14-day lag documented; 3 enterprise deals lost | [src-chatgpt](market-validation/sources/src-chatgpt-ci-limitations.md) |
| The 40-30-30 rule | 40% handled well, 30% adequate with oversight, 30% complete failure (monitoring, routing, team distribution) | [src-chatgpt](market-validation/sources/src-chatgpt-ci-limitations.md) |
| No team distribution | 40+ hour delay between discovery and team awareness | [src-chatgpt](market-validation/sources/src-chatgpt-ci-limitations.md) |

**Full response (expanded from war room Obj 3 + Obj 15):**

| Dimension | ChatGPT / Perplexity | Kompete |
|-----------|---------------------|---------|
| **Monitoring** | You ask when you remember. Nobody runs 75 prompts/day. | Autonomous 24/7. You don't think about it. |
| **Accuracy** | Fabricates pricing tiers, invents articles. 52% hallucination rate (Gartner). | Scraped from actual sources. Claims verified. |
| **Memory** | Every query starts from zero. | Strategy Timeline — 12+ months of history, pattern recognition. |
| **Speed** | You search when you think to search. By definition, late. | Sub-3-minute alerts. Detected before you'd think to look. |
| **Team** | One person gets one answer. "If I just put summaries to my team, they ignore me." — Rajesh Sahu | Team-specific briefs auto-delivered. Sales ≠ Product ≠ CS. |
| **Workflow** | Copy-paste into Slack/doc. No CRM integration. | Battle cards in CRM. Alerts in Slack. Weekly brief to CEO. |
| **Cost of time** | 21+ daily source checks; $20-39K/year in hidden PMM time | Automated. PMM time freed for strategy. |

**The concession:** ChatGPT IS good at ~40% of CI work (market overviews, summarization, ad-hoc research). Don't argue it's bad — argue it's incomplete. The 60% it fails at is where the product lives.

**Three-line elevator version (from war room):**
1. "ChatGPT answers the question you remembered to ask. We answer the ones you didn't."
2. "ChatGPT has no memory. We have 12 months of competitive history."
3. "ChatGPT tells you. We tell your whole team — in their language, in their tools."

**MECE issue tree:** [objection-3-why-not-chatgpt.md](market-validation/issue-trees/objection-3-why-not-chatgpt.md)

---

## B. PRODUCT & VALUE OBJECTIONS

These accept that CI matters but question whether THIS product delivers enough value.

---

<a id="b1"></a>
### B1. "How is this different from Perplexity / Deep Research specifically?"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Advisors, technically sophisticated operators |
| **Frequency** | High — variant of A3 but more specific to Perplexity |
| **Type** | Product comparison |

**One-liner response:**
> "Perplexity answers the question you asked. Kompete answers the questions you didn't know to ask — and does it every day, for every team, without you lifting a finger."

**Full response:**

Same core argument as A3 but with specific Perplexity framing:

> "Can you run a Perplexity deep research query every morning for each of your 15 competitors across pricing, features, reviews, hiring, and social? That's 75 queries a day. We automate that entire workflow and turn it into a system of record."

**Analogy:** Perplexity is like asking a really smart person a question. Kompete is like hiring a full-time CI analyst who works 24/7, never forgets anything, and automatically briefs every team in their language.

---

<a id="b2"></a>
### B2. "Static vs Dynamic — only dynamic info is worth paying for"

| | |
|---|---|
| **Source** | Siddharth Jain [LeadSquared] (coffee chat) |
| **Date first heard** | 2026-02-19 |
| **Who says this** | Experienced B2B operators, enterprise PMs |
| **Frequency** | Medium — but it's a critical PRODUCT DESIGN insight, not just an objection |
| **Type** | Product value framework |

**One-liner response:**
> "Exactly right. That's why our feed and alerts are the product. The static analysis is the foundation — the dynamic signals are what make you open it twice a day."

**The framework (from Siddharth):**

**Dynamic (= worth paying for):**
- Competitor acquired your target customer → CS/Sales: win-back campaign
- Competitor launched campaign targeting your base → Marketing: counter within 24hrs
- Leadership departure at competitor → Sales: target destabilized accounts
- Pricing change → Sales: adjust active negotiations
- Competitor outage/crisis → Sales: outbound to frustrated customers NOW
- Negative review surge → Marketing: comparison content, SDR outreach

**Static (= nice-to-have, free/entry tier):**
- Feature comparison matrix (changes quarterly)
- Competitor "about us" page (rarely changes)
- Integration list (updates slowly)
- Pricing page for enterprise SaaS (changes 1-2x/year)

**Product implication:** The feed/alert layer IS the product. Static analysis is the reference library. Dynamic signals should be the paid tier. This aligns with pricing (low-sub + usage-heavy).

---

<a id="b3"></a>
### B3. "Will I pay for it? Information vs business value"

| | |
|---|---|
| **Source** | Siddharth Jain [LeadSquared] (coffee chat) |
| **Date first heard** | 2026-02-19 |
| **Who says this** | Revenue-minded operators, founders |
| **Frequency** | High — the fundamental commercial question |
| **Type** | Value objection |

**One-liner response:**
> "68% of your deals involve a competitor. 21% are lost to them. A third of those are winnable. At your deal size, that's real money walking out the door."

**Key quote from Siddharth:** *"A competitive information which does not help me scale my business or get new business is something I would not put money upon. Happy to read it. But will I pay for it?"*

**Evidence that CI drives business outcomes:**

| Outcome | Data | Source |
|---------|------|--------|
| Revenue lift from competitor info | +4.8% (causal, RCT) | [src-management-science](market-validation/sources/src-management-science-kim-2025.md) |
| Deals lost to competitors | 21%, 33% winnable | [src-klue](market-validation/sources/src-klue-competitive-revenue-gap-2025.md) |
| Cost of competitive losses | $2-10M/year | [src-crayon](market-validation/sources/src-crayon-state-of-ci-2025.md) |
| Battle card win rate lift | Up to 59% | [src-crayon](market-validation/sources/src-crayon-state-of-ci-2025.md) |
| Win-loss programs → increased win rates | 84% of companies after 2+ years | [src-clozd](market-validation/sources/src-clozd-win-loss-analysis.md) |

**Product rule:** Every notification must include a "business impact" line and a "recommended action." If we can't articulate the business impact, we shouldn't send the notification — it's noise.

**Framework for every alert:**
- ❌ "Competitor X updated their homepage messaging."
- ✅ "Competitor X is now positioning against your core value prop. 3 active deals mention this feature. Here's the counter-narrative."

---

<a id="b4"></a>
### B4. "Enterprise data doesn't change frequently"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | People with enterprise (SAP/Oracle-level) backgrounds |
| **Frequency** | Low — ICP-specific. Only comes up from enterprise people. |
| **Type** | Product relevance objection |

**One-liner response:**
> "You're right for SAP vs Oracle. But in the SaaS world where our ICP lives, competitors move weekly. Battle cards go stale within a week."

**Full response:** Sanchit is right for enterprise — and that's NOT our ICP. Our ICP is $5-200M ARR B2B SaaS where competitors ship weekly, pricing experiments happen constantly, and positioning changes in days. Even in Sanchit's framing, the Strategy Timeline has value — a quarterly review based on 3 months of auto-captured data is 10x better than a manually assembled one.

**Evidence:** *"They launched the same product two days before us. We had no idea."* — Tanvir (HackerRank). 5-15 meaningful competitive signals per week in SaaS.

---

<a id="b5"></a>
### B5. "Signal vs noise — AI gives surface-level answers"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Experienced operators who've been burned by AI hype |
| **Frequency** | Medium — the honest and hardest objection |
| **Type** | Product quality concern |

**One-liner response:**
> "Day 1, we're better than manual research but not better than a great PMM. By month 3, we're better than that PMM because we never forget, never miss, and have pattern data they can't hold in their head."

**Full response:** What AI does well today: monitor at scale, surface changes, cross-reference signals, structured analysis. Where the gap is: context-specific interpretation, strategic synthesis, action quality. Our approach: the Strategy Timeline + company context builds calibration over time. Week 1 is generic. Month 3 is calibrated to your reality.

**Key interview evidence:**
- *"Any agent can be built to scrap data and give a summary. The decision is far more important."* — Rajesh Sahu
- *"If you will build some insights from that data, it will just flip the whole game."* — Garima (BrowserStack)

---

<a id="b6"></a>
### B6. "AI should discover competitors, not the user"

| | |
|---|---|
| **Source** | Siddharth Jain [SaaS Labs/JustCall] (interview) |
| **Date first heard** | 2026-02-10 |
| **Who says this** | PMs, product-minded operators |
| **Frequency** | Medium — but could be the aha moment in signup flow |
| **Type** | Product design insight |

**One-liner response:**
> "Exactly. You tell us about your business, we tell you who to watch."

**Full response:** Instead of "add your competitors," start with "tell us about your business." AI maps the domain and suggests a competitor landscape. Tiered: free discovery (lightweight, LLM-based list) → deep tracking per competitor (paid).

**Interview convergence:**
- Siddharth: "If you could analyze on a global level, companies working in the same domain..."
- Rohan (Inkle): "There are others that we don't even know that we may have missed."
- 7/27 interviewees flagged unknown unknowns as high-value

---

<a id="b7"></a>
### B7. "Customer voice should inform CI, not just competitor tracking"

| | |
|---|---|
| **Source** | Siddharth Jain [SaaS Labs/JustCall] (interview) |
| **Date first heard** | 2026-02-10 |
| **Who says this** | PMs who've shifted from competitor-watching to customer-listening |
| **Frequency** | Medium |
| **Type** | Product design insight |

**One-liner response:**
> "That's exactly why we scrape competitor REVIEWS — their customers' voice tells you where the market opportunity is."

**Full response:** Siddharth isn't saying CI is useless — he's saying CI disconnected from customer context is useless. Our Review Intelligence already bridges this: G2/Capterra reviews from competitor customers ARE customer voice. Every alert should include a "customer impact" line — not just "Competitor X did Y" but "This likely affects Z segment of your customers because..."

**Now backed by data:** The false dichotomy is proven — competitive awareness improves customer outcomes (Management Science RCT: firms receiving competitor info had 8% more customers). [src-management-science](market-validation/sources/src-management-science-kim-2025.md)

---

<a id="b8"></a>
### B8. "Sales team already knows faster than public data"

| | |
|---|---|
| **Source** | Siddharth Jain [LeadSquared] (coffee chat) |
| **Date first heard** | 2026-02-19 |
| **Who says this** | Enterprise operators with large field teams (1000+ employees) |
| **Frequency** | Low — only from large companies |
| **Type** | ICP boundary objection |

**One-liner response:**
> "True at 2000+ employees. But at 50-500 people, your sales team's intel is scattered across Slack and people's heads with no system of record."

**Full response:** This sharpens ICP. At 2000+ employees, field teams ARE faster on many signals. Our sweet spot is 50-1500 employees where: sales exists but isn't a comprehensive intelligence network, no dedicated CI analyst, intel scattered with no system of record, geographic blind spots.

**Siddharth validated the geographic use case:** *"New geography... you don't have field eyes and field ears to get you what you need there."*

---

<a id="b9"></a>
### B9. "Make me open your dashboard twice a day"

| | |
|---|---|
| **Source** | Siddharth Jain [LeadSquared] (coffee chat) |
| **Date first heard** | 2026-02-19 |
| **Who says this** | Engagement-minded operators |
| **Frequency** | Low as an objection — high as a DESIGN PRINCIPLE |
| **Type** | Product quality bar |

**Key quote:** *"If you bring that information which makes me open your dashboard like twice a day... that will always be linked to business, not to information."*

**What makes twice-a-day:**
1. Morning: brief arrived — "here's what changed overnight"
2. During day: push alert — "Competitor dropped pricing, 3 of your active prospects affected"

**What does NOT:** Feature matrices, competitor profiles, historical timeline (reference material, not daily habit).

**Product implication:** The feed IS the product. Everything else is the reference library. This validates our v6.1/v6.2 scrolling intel feed as the default landing.

---

<a id="b10"></a>
### B10. "Trigger events drive deep analysis, not continuous monitoring"

| | |
|---|---|
| **Source** | Siddharth Jain [LeadSquared] (coffee chat) |
| **Date first heard** | 2026-02-19 |
| **Who says this** | Enterprise operators |
| **Frequency** | Medium |
| **Type** | Product design insight |

**The pattern:** (1) Monthly baseline check → (2) Trigger event (sales reports competitor move) → (3) Deep dive activated → (4) Update competitive database.

**Product implication:** We automate mode 1 (continuous monitoring = surfaces trigger events). Humans engage for mode 2 (deep dive — profiles, matrices, timeline). We make mode 2 faster by having all data pre-assembled.

---

## C. GTM & BUYER OBJECTIONS

These accept the product value but question who buys, how, and why.

---

<a id="c1"></a>
### C1. "Buyer vs user persona confusion — who owns the budget?"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Advisors, GTM-experienced operators |
| **Frequency** | High — our most important GTM question |
| **Type** | GTM strategy |

**One-liner response:**
> "We don't sell to PMM. We sell to the person who loses money when competitive intelligence fails — founder/CEO at $5-50M, CMO at $50-200M."

**Full response:** PMM is the user, not the buyer. Land with Founder/CEO (they ARE the CI function at $5-50M). Expand to Sales (battle cards in CRM). Expand to Product (feature gaps). The weekly CEO brief is the Trojan horse.

**Convergence:** Sanchit, Siddharth [SaaS Labs], Siddharth [LeadSquared] all independently arrived at: founder/CEO is the buyer.

---

<a id="c2"></a>
### C2. "ROI justification is hard for PMM"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Advisors, enterprise sellers |
| **Frequency** | Medium |
| **Type** | Pricing/value justification |

**One-liner response:**
> "We don't sell ROI on CI. We sell ROI on outcomes: a single saved deal at $50K ACV pays for 3+ years of Kompete."

**Now backed by data:**
- 21% of deals lost to competitors, 33% winnable = ~7% recoverable ([src-klue](market-validation/sources/src-klue-competitive-revenue-gap-2025.md))
- $2-10M/year in winnable losses ([src-crayon](market-validation/sources/src-crayon-state-of-ci-2025.md))
- A $20K tool recovering 1% of winnable losses at $20M ARR = $200K recovered = 10x ROI
- We price at fraction of legacy ($3-5K/yr vs $40-80K), so the ROI bar is dramatically lower

---

<a id="c3"></a>
### C3. "Spreading too thin on user personas"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Advisors, product strategists |
| **Frequency** | Medium |
| **Type** | Product focus |

**One-liner response:**
> "We don't build 6 products. We build ONE intelligence layer and DELIVER it 6 ways."

**Full response:** Core engine is the same — monitoring + analysis + synthesis. What changes per persona is: signals highlighted, format delivered, actions recommended. Launch with PMM + Sales. Expand to Product + CS. Weekly CEO brief is the Trojan horse for org-wide adoption.

**Analogy:** Slack doesn't build separate products for engineering, sales, and marketing. One product, team-specific channels.

---

<a id="c4"></a>
### C4. "Target founders first — they'll pull in teams"

| | |
|---|---|
| **Source** | Siddharth Jain [SaaS Labs/JustCall] (interview) |
| **Date first heard** | 2026-02-10 |
| **Who says this** | Experienced B2B operators |
| **Frequency** | This is advice, not an objection |
| **Type** | GTM insight |

**Key quote:** *"Target the founders... give them the insights they're looking for... Once they get good outcome, their teams."*

**Convergence:** Siddharth [SaaS Labs], Siddharth [LeadSquared], and Sanchit all independently said the same thing. Three for three. Founder-first GTM is validated.

---

<a id="c5"></a>
### C5. "SME market won't pay (India)"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Anyone with India B2B experience |
| **Frequency** | Medium — geography-specific |
| **Type** | Market selection |

**One-liner response:**
> "Agreed. India SMEs are NOT our primary market."

**Full response:** Priority: (1) US B2B SaaS $10-200M ARR. (2) India B2B SaaS $5M+ ARR, US-facing (HighRadius, HackerRank, BrowserStack). (3) India SMEs = NOT a target. Free early access for design partners only, time-bounded.

---

<a id="c6"></a>
### C6. "Sell outcomes, not capabilities"

| | |
|---|---|
| **Source** | Siddharth Jain [SaaS Labs/JustCall] (interview) |
| **Date first heard** | 2026-02-10 |
| **Who says this** | Marketing-experienced operators |
| **Frequency** | This is advice, not an objection |
| **Type** | Messaging discipline |

**The reframe table:**

| Capability-Led (Avoid) | Outcome-Led (Use) |
|------------------------|-------------------|
| "8 AI agents monitoring competitors" | "Never get blindsided by a competitor move again" |
| "Auto-updating battle cards" | "Your sales team walks into every competitive deal prepared" |
| "Pricing intelligence" | "Know the moment a competitor undercuts you — before your customers do" |
| "Strategy Timeline" | "See the pattern behind your competitor's moves — and predict the next one" |

---

## D. COMPETITIVE MOAT OBJECTIONS

---

<a id="d1"></a>
### D1. "Lock-in problem — what stops someone using Glean?"

| | |
|---|---|
| **Source** | Sanchit Agarwal (advisor conversation) |
| **Date first heard** | 2026-03-14 |
| **Who says this** | Advisors, investors, technically sophisticated operators |
| **Frequency** | Medium |
| **Type** | Defensibility question |

**One-liner response:**
> "Glean searches what you already know. We discover what you don't know yet. They're complementary."

**Three layers of lock-in:**
1. **Strategy Timeline (time-based moat):** 12+ months of history that no tool can replicate
2. **Calibrated intelligence (learning moat):** Learns what YOUR company cares about over time
3. **Workflow lock-in:** Battle cards in Salesforce, alerts in Slack, weekly CEO brief in the operating rhythm

---

## E. PRICING OBJECTIONS

---

<a id="e1"></a>
### E1. "Low subscription, usage-heavy pricing"

| | |
|---|---|
| **Source** | Siddharth Jain [SaaS Labs/JustCall] (interview) |
| **Date first heard** | 2026-02-10 |
| **Who says this** | Experienced SaaS operators |
| **Frequency** | This is advice, not an objection |
| **Type** | Pricing architecture |

**Siddharth's model applied:**
- $0-$49/mo subscription — gets in the door
- Usage charges on: competitors tracked, team seats, custom reports, integrations, API calls
- Aligns with B2 (static = free, dynamic = paid) and B3 (pay for business value, not information)

**Budget context:** S&M = 31-40% of ARR at $5-50M. CI tools at $20-40K/year are a rounding error. Real competitor = PMM's manual time at $20-39K/year hidden cost. ([src-saas-benchmarks](market-validation/sources/src-saas-benchmarks-budgets.md))

---

<a id="e2"></a>
### E2. "Figure out who/why/what they'll pay — before building"

| | |
|---|---|
| **Source** | Siddharth Jain [LeadSquared] (coffee chat) |
| **Date first heard** | 2026-02-19 |
| **Who says this** | Business-first operators |
| **Frequency** | This is meta-advice |
| **Type** | Strategic discipline |

**Key quote:** *"You figure out who will pay, why will they pay, and what will they pay — and then you come to this dashboard to decide which information to show."*

**Current status:**

| Question | Current Answer | Confidence |
|----------|---------------|------------|
| **Who pays?** | Founder/CEO at $5-50M ARR; CMO/VP Marketing at $50-200M | Medium-High |
| **Why they pay?** | Win more deals, don't lose customers, save 15hrs/week | Medium — now backed by Klue/Crayon/Gong data |
| **What they pay?** | $2-5K/yr (2-3% of consulting equivalent) | Low — untested |

---

## Cross-Reference

- **MECE issue trees with full evidence chains:** `market-validation/issue-trees/`
- **Raw source files with URLs and bias notes:** `market-validation/sources/`
- **Search methodology (why these sources, not others):** `market-validation/methodology.md`
- **Strategic war room (mission, vision, personas, pitch, marketing framework):** `../kompete-website/research/synthesis/strategic-war-room.md`
- **Customer interview transcripts:** `interviews/`
- **Pain points synthesis from 27 interviews:** `synthesis/pain-points.md`

---

## Open Questions (from war room, preserved)

1. Positioning language: "CI Platform" vs "Competitive Revenue Engine" vs "Competitive Operating System"
2. Hero feature for launch: Strategy Timeline vs AEO vs Battle Cards vs Competitor Discovery
3. Pricing model: low-sub + usage needs testing
4. Consulting angle: Big 4 as beachhead or stay B2B SaaS direct?
5. India vs US-first: current plan is US-first with India design partners
6. Outcome vs capability messaging: audit all website copy
7. Competitor Discovery in signup flow: hook or premium?
8. Customer context integration: every recommendation tied to "what this means for YOUR customers"
9. Static vs Dynamic product tiers: static = free, dynamic = paid?
10. "Twice a day" engagement: identify top 5 trigger events by business impact
11. ChatGPT objection: must be addressed proactively on website, in deck, in first 30 seconds of demo
12. Enterprise ceiling: 2000+ employees = lower value from public data monitoring

---

*Add new objections below with date + source. Update responses as thinking evolves.*
