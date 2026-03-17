# Interview Extract: Chanchal Gher

**Date:** 11th Feb, 2026
**Role/Company:** Former employee at Atlan (clarified mid-interview); Product/TPM background across multiple B2B SaaS companies in Bangalore
**Background:** Experienced product professional (TPM in most recent role, product contributor previously) with exposure to enterprise and mid-market B2B SaaS companies across 3–4 organizations. Has hands-on experience with competitive intelligence frameworks, product discovery, and growth functions.

---

## Objections & Challenges Raised

### Objection: Competitive Scraping Is Already Commoditized
- **Quote:** "Everybody can do it in the industry. You can have Databricks can have whatever Snowflake is doing. Snowflake can have whatever Databricks is doing. You can have multiple ways to get anything."
- **Timestamp:** [12:22]
- **Severity:** High — directly challenges the core data-gathering value prop
- **Category:** Differentiation
- **Summary:** Chanchal believes web scraping of changelogs, product updates, and public signals is trivially achievable by any company today. He implies there is no meaningful moat in the data collection layer. The differentiation challenge is therefore not in gathering data, but in what you do with it.
- **Connects to:** Similar to the "ChatGPT/Perplexity comparison" pattern seen in other interviews — interviewees suggest the raw intelligence layer is table stakes, not a differentiator.

---

### Objection: Mature Companies Already Have Internal Agents on CI Data
- **Quote:** "I think they already have some sort of agentic team on top of it now... usually you have a bot chain interface, a business app, something of that sort."
- **Timestamp:** [06:09]
- **Severity:** High — suggests the ICP's upper end (larger B2B SaaS companies) may already be solving this internally
- **Category:** Market Fit
- **Summary:** Chanchal observes that even large startups now have internal AI agents layered on top of competitive intelligence data. This implies that the most mature and well-resourced buyers in Kompete's target range may already have in-house solutions, narrowing the addressable sweet spot.
- **Connects to:** New — but related to the "build vs. buy" objection likely seen elsewhere.

---

### Objection: Real-Time Alerts Have Limited Value in B2B Due to Long Sales Cycles
- **Quote:** "The sales cycle is still... it's not like you know, you see a new change today and you go and buy tomorrow. It takes three months to start with and then it takes years in case of multi-million ARR deals to complete."
- **Timestamp:** [20:16]
- **Severity:** High — challenges the urgency/frequency angle of the value prop
- **Category:** Value Prop
- **Summary:** Chanchal argues that B2B sales cycles are long enough that the pace of competitor changes rarely creates an immediate, actionable trigger. The sub-3-minute alert differentiator may resonate less with his persona, as decisions are made on a quarterly cadence rather than in real time.
- **Connects to:** New — directly challenges the "sub-3-minute alerts" differentiator and the Duolingo/Google ChatGPT disruption framing Aditya raised.

---

### Objection: Hiring Signals Are a VC/Investor Play, Not a Product Team Play
- **Quote:** "This will be more of an VC play rather than company play... If I'm a product guy or if I'm in marketing, something like hiring, I don't care."
- **Timestamp:** [29:19]
- **Severity:** Medium — challenges the relevance of a specific feature module rather than the overall platform
- **Category:** Product
- **Summary:** Chanchal clearly does not see hiring signals as relevant to his day-to-day product role. While he acknowledged that combined signals (hiring + messaging + patents) could yield strategic insight, he was skeptical that this framing would resonate with product or marketing personas. The consolidated intelligence angle may need better packaging to land.
- **Connects to:** New — Persona-specific relevance gap; may connect to "buyer persona confusion" pattern if other interviews reveal similar signal dismissal by operators.

---

### Objection: Pricing Intel Is Unavailable for Most B2B Products
- **Quote:** "If people do not show pricing how you're getting the pricing intel in?"
- **Timestamp:** [28:48]
- **Severity:** Medium — highlights a data availability gap for the pricing module
- **Category:** Product
- **Summary:** For the majority of mid-market and enterprise B2B products, pricing is gated behind sales conversations. Chanchal pointed out that the pricing comparison feature is only viable for a subset of companies. This limits the breadth of the pricing intelligence module.
- **Connects to:** Pricing Opacity — likely raised in other interviews given Kompete's own awareness of this in its product roadmap.

---

### Objection: Review Platforms Are Biased / Funded
- **Quote:** "Usually no, because again most of these are funded. So again feedbacks are very funded... positives and all are very [biased]."
- **Timestamp:** [25:34]
- **Severity:** Medium — reduces trust in a core data signal source (G2, Capterra, etc.)
- **Category:** Value Prop
- **Summary:** Chanchal is skeptical of review platform data quality, viewing positive reviews as pay-to-play artifacts. He conceded negative reviews may carry more signal, but dismissed the category broadly. This weakens the review-based sentiment analysis component unless Kompete can demonstrate noise filtering or bias detection.
- **Connects to:** Stale Data / data quality concern — may connect to similar skepticism in other interviews about relying on G2/Capterra.

---

### Objection: B2B Change Velocity Is Slow — Quarterly Is Enough
- **Quote:** "Usually people do it and keep it right. You do a quarterly analysis or you do bi-monthly analysis. Monthly analysis is a maximum. Nobody goes into competitive analysis every day."
- **Timestamp:** [10:04]
- **Severity:** Medium — challenges frequency of use and therefore engagement/stickiness
- **Category:** Value Prop
- **Summary:** Chanchal believes competitive intelligence is fundamentally a periodic, event-triggered activity in B2B — not a daily one. This suggests that a continuous news-feed model may face adoption challenges unless tied to clear workflow triggers (RFPs, product discovery cycles, sales cycles).
- **Connects to:** New — but related to the "reactive vs. proactive" tension Aditya raised in his framing.

---

## Pain Points Validated

### Pain: Competitive Intel Lives in Docs Nobody Reads
- **Quote:** "It would be sitting somewhere in the document. It all depends on who the consumers are... If you are in customer success, you usually don't interact."
- **Severity:** HIGH
- **Category:** No System of Record
- **Currently solving with:** Battle cards in shared documents; informal knowledge held by CI team or strategy leads; ad hoc team briefings.

---

### Pain: Information Doesn't Flow Across Teams
- **Quote:** "Usually the CEO founders, few people, they know all the things. But across the world that visibility and that basically flow of competitive intelligence is not there."
- **Severity:** HIGH
- **Category:** Tool Fragmentation
- **Currently solving with:** Different teams maintaining separate intel (product = feature comparisons, marketing = messaging, partnerships = ecosystem, sales = win/loss), with no centralized, accessible layer.

---

### Pain: Point-in-Time Snapshots Miss Mid-Cycle Changes
- **Quote:** "It won't be in a point in time, but it would be some referential point... you do a quarterly analysis or you do bi-monthly analysis."
- **Severity:** MEDIUM
- **Category:** Stale Data
- **Currently solving with:** Quarterly or bi-monthly manual reviews; relying on changelogs and product scraping done ad hoc by CI team.

---

### Pain: Battle Cards Are Static and Hard to Keep Updated
- **Quote:** "Usually every company has some sort of battle cards... But is everyone interacting with it? I would say yes to this — it all depends."
- **Severity:** MEDIUM
- **Category:** Stale Data
- **Currently solving with:** Manually maintained documents; occasional PMM-driven updates; not systematically refreshed after trigger events.

---

### Pain: Competitive Intelligence Is Reactive, Not Proactive
- **Quote:** "We are always reactive. Some customer will come and tell us, this competitor is having this feature which you don't have."
- **Severity:** HIGH
- **Category:** Late Discovery
- **Currently solving with:** Customer feedback, win/loss notes in CRM, ad hoc RFP-triggered competitor research.

---

### Pain: Feature-Level Delta Is Hard to Track Continuously
- **Quote:** "The change logs... the definitions of the features and how it is different from what we have and the impact on what we have or what we don't have. Definitely that delta is important. It's something that we have to consider every time we build something or propose something or get funded for something."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Manual changelog review; product discovery research done before each build cycle.

---

## Product Feedback & Feature Requests

### Feedback: Change Log Tracking Is the #1 Most Valuable Signal
- **Quote:** "I'll say the change logs. The definitions of the features and how it is different from what we have and the impact on what we have or what we don't have. Definitely that delta is important."
- **Type:** Feature Request
- **Priority signal:** Strong — unprompted top-of-mind answer to "if you could track just one thing, what would it be?" Framed as essential to product decisions and funding proposals.

---

### Feedback: Competitive Intelligence as a News Feed Is Well-Received
- **Quote:** "Yeah" [affirming the news channel concept] — and earlier: "It would be sitting somewhere in the document... somebody on top of it and provide direct intelligent info to where you are would make more."
- **Type:** Positioning Feedback
- **Priority signal:** Moderate — validated the concept of a continuous feed, though Chanchal cautioned that daily engagement may be aspirational given B2B cadences.

---

### Feedback: Hiring Signals Need Better Framing for Operator Personas
- **Quote:** "If I'm a product guy or if I'm in marketing or someone, something like hiring, I don't care... I can care when trying to join a company, but not after."
- **Type:** Positioning Feedback
- **Priority signal:** Strong signal to reframe — the consolidated intelligence narrative (hiring + patents + messaging = "they're building X") needs to be the lead, not the raw hiring data itself.

---

### Feedback: Pricing Module Limited to Companies with Exposed Pricing
- **Quote:** "If people do not show pricing how you're getting the pricing intel in?"
- **Type:** UX Suggestion / Positioning Feedback
- **Priority signal:** Medium — a practical data gap concern, not a product dismissal. Chanchal acknowledged Reddit threads as an alternative source and didn't reject the module entirely.

---

### Feedback: Review Platform Data Requires Quality/Bias Filtering
- **Quote:** "Usually no, because again most of these are funded. So again feedbacks are very funded."
- **Type:** Positioning Feedback
- **Priority signal:** Medium — Kompete should proactively address data bias in its narrative around review sentiment (e.g., emphasizing negative review filtering or weighting).

---

## Strategic Insights

### Insight: Product Manager Is the Primary Initiator — and Best Entry Point
- **Quote:** "Product can be the person I would say to start with because usually product is the one who starts with competitive intelligence or competitive framework. And then other teams come and place as a collaborator."
- **Implication for Kompete:** The product team — not marketing or strategy — is often the founder of the CI practice at growing companies. This suggests leading GTM with a product-first narrative and targeting VP Product / Senior PMs as the champion persona, even if PMMs or strategy leads are the ultimate budget owners.

---

### Insight: Multiple Contributing Personas, No Single Owner
- **Quote:** "Multiple personas come into play — there's always use cases, there is always pricing, there is always sales feedbacks... depending upon what area of the business you look into."
- **Implication for Kompete:** The CI use case is genuinely cross-functional (product, PMM, pre-sales, CS, partnerships, strategy). Kompete's team-specific delivery differentiator is directly validated — the challenge is that no single persona is the universal buyer, making top-down sales through a strategy lead or CMO more efficient than bottoms-up.

---

### Insight: The Value of Aggregated Signals Is Greater Than Any Individual Signal
- **Quote:** "[On hiring signals:] If I'm in product, I don't care. But [Aditya:] if you look at in totality, it was also part of the puzzle to solve this."
- **Implication for Kompete:** Individual signals (hiring, changelog, messaging) are dismissed when presented in isolation by operator personas. The strategic insight layer that *synthesizes* signals into a forward-looking narrative ("High Radius is building an AI reconciliation agent because...") is where Kompete's real differentiation lives and should be the lead demo moment.

---

### Insight: B2B Competitive Intelligence Is Triggered, Not Continuous
- **Quote:** "From a company's point of view it usually keeps on getting updated as soon as you are in a sales cycle for any new customer or as an RFP discussion starts."
- **Implication for Kompete:** Designing for trigger-based workflows (RFP alerts, new prospect research, product discovery sprints) may drive higher adoption than positioning around always-on monitoring. Consider a "Briefing Mode" that surfaces relevant intel when a new deal or discovery cycle begins.

---

### Insight: AI Shipping Velocity Will Increase Urgency for Real-Time CI Over Time
- **Quote:** "With cloud code etc., what was being done in probably six months will be timed down to probably a month or so... if you have used Claude Code I think it fully tells you like okay let's do this then do this."
- **Implication for Kompete:** Even if real-time monitoring feels low-urgency today in B2B, accelerating AI-driven development (Aditya's framing, validated by Chanchal's "Yep") will compress competitive cycles. Kompete should position its real-time alerts as a future-proofing investment, using concrete examples like Duolingo's valuation drop post-ChatGPT to make the case.

---

## Persona Signals

- **Buyer or User?** User — Chanchal is a product practitioner (TPM/PM background). He would be a consumer of the platform, not a budget owner. He explicitly deferred to strategy leads, PMMs, and founders as the decision-making personas.
- **Willingness to pay:** Not directly discussed. No pricing sensitivity signals emerged. His comments suggest he would need organizational buy-in rather than making an independent purchase.
- **Decision process:** Chanchal would likely be a champion/validator rather than a buyer. He suggested speaking to "somebody who is on the strategic side" and PMM personas. Evaluation would likely be triggered by a pain point surfacing during a product discovery cycle or RFP.
- **Current tools mentioned:** Battle cards (company-maintained docs), internal agents/bots on CI knowledge bases, changelogs, G2/Capterra/Product Hunt (viewed skeptically), Gong calls, unstructured documents and Excel, conference intelligence, LinkedIn (dismissed as unnecessary for scraping).

---

## Key Quotes (Top 5)

1. *"Usually people do it and keep it right. You do a quarterly analysis or you do bi-monthly analysis. Monthly analysis is a maximum. Nobody goes into competitive analysis every day."* — [10:04] — validates the stale data pain point and challenges the real-time alert value prop; defines the baseline behavior Kompete must disrupt.

2. *"It would be sitting somewhere in the document. It all depends on who the consumers are... If you are in customer success, you usually don't interact."* — [14:09] — directly validates the "no system of record" pain and the need for team-specific delivery.

3. *"The change logs — the definitions of the features and how it is different from what we have and the impact on what we have or what we don't have. Definitely that delta is important. It's something that we have to consider every time we build something or propose something or get funded for something."* — [23:09] — single strongest feature validation in the interview; change log delta tracking is the #1 requested signal.

4. *"Everybody can do it in the industry. You can have Databricks can have whatever Snowflake is doing... you can have multiple ways to get anything."* — [12:22] — the sharpest challenge to Kompete's data-gathering moat; must be addressed in positioning.

5. *"Somebody on top of it and provide direct access to where you are or direct intelligent info to where you are would make more [sense]."* — [31:57] — organic, unprompted validation of Kompete's core value proposition of surfacing actionable intelligence directly to the right person at the right time.
