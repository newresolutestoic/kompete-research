# Interview Extract: Rashi Sekhsaria

**Date:** January 2026
**Role/Company:** Pricing Analyst, KPMG
**Background:** Rashi works as a pricing analyst at KPMG, where she participates in multi-month pricing strategy engagements costing $100K+ per project. She has hands-on experience with both quantitative methods (conjoint analysis, churn modeling) and qualitative competitive research (manual scraping, feature comparison tables, review mining).

> ⚠️ **Note on transcript quality:** This document is an interviewer's structured summary/notes, not a verbatim transcript. Quoted passages appear to be direct quotes captured during the interview. No timestamps are present in the source material. All timestamps are noted as "N/A – no raw transcript provided."

---

## Objections & Challenges Raised

### Objection: AI Output Distrust
- **Quote:** "Use AI cautiously (don't fully trust outputs)"
- **Timestamp:** N/A
- **Severity:** High — directly challenges the core of Kompete's AI-powered extraction pipeline (Firecrawl + Gemini)
- **Category:** Product
- **Summary:** Rashi noted that KPMG analysts use AI tools carefully and do not fully trust AI-generated outputs. This implies that even sophisticated, analyst-level users will have reservations about AI-extracted pricing and feature data. If the core differentiator is automation via AI, skepticism about AI accuracy is a fundamental adoption risk. Kompete will need to demonstrate data quality, provide source citations, and allow human verification.
- **Connects to:** New — but likely recurs across personas who are professional analysts or work in regulated/high-stakes environments

---

### Objection: MVP Is Incomplete Without Survey/WTP Data
- **Quote:** "100-300 respondent surveys with conjoint analysis. Measures customer willingness to pay. Tests price increase scenarios (20-30%). Churn modeling based on price sensitivity."
- **Timestamp:** N/A
- **Severity:** Medium — does not reject the MVP, but implies that competitive benchmarking alone is only Phase 1 of a full pricing strategy engagement; a customer relying solely on Kompete may feel underserved
- **Category:** Value Prop
- **Summary:** Rashi described how KPMG's pricing work has two distinct phases: competitive benchmarking (Phase 1) and willingness-to-pay research via survey/conjoint analysis (Phase 2). Kompete currently only addresses Phase 1. A sophisticated buyer may view the tool as incomplete for driving an actual repricing decision. This isn't a blocker for adoption, but it is a ceiling on the perceived value of the product for enterprise-level use.
- **Connects to:** New — raises a "feature completeness" concern that could resurface with CFO or Head of Revenue buyers

---

### Objection: Prescriptive Framing Undermines Credibility
- **Quote:** "The product would deliver diagnostic and descriptive insights, not prescriptive pricing recommendations. Support informed decision-making."
- **Timestamp:** N/A
- **Severity:** High — the original Kompete/Valoris framing ("Roast My Pricing," "you should charge $X") was explicitly contradicted by a domain expert
- **Category:** Positioning Feedback / GTM
- **Summary:** Rashi drew a clear line between what software should do (describe the landscape) and what consultants or analysts do (make recommendations). Prescriptive outputs ("your price is too high, change it") would likely trigger skepticism or distrust from professional buyers who know that pricing decisions require context that no automated tool can fully capture. This is both a product and a messaging objection — and it's coming from someone who would be a power user.
- **Connects to:** Likely to recur with any analytically-sophisticated buyer persona — finance teams, pricing leads, RevOps

---

### Objection: KPMG's Client Base Doesn't Overlap With Kompete's Target
- **Quote:** "Companies with $500k to $3M ARR can't afford $100k consulting but need pricing help. They rely on internal pricing analysts or marketing teams."
- **Timestamp:** N/A
- **Severity:** Medium — validates target market but creates a nuance: the interviewee herself serves *different* companies than Kompete's target, meaning her validation is secondhand for the primary ICP
- **Category:** Market Fit
- **Summary:** Rashi confirmed that KPMG works with clients at $10M+ ARR, while Kompete is targeting $500K–$3M ARR. This means Rashi's direct knowledge of the $500K–$3M segment is inferential ("they rely on internal teams") rather than experiential. The pain point is real, but the validation is one degree removed. Kompete still needs direct interviews with the actual ICP — internal pricing analysts at sub-$3M ARR companies.
- **Connects to:** New — this is a methodological signal worth flagging; future interviews should prioritize the primary ICP directly

---

### Objection: "Roast" Framing Is Unprofessional
- **Quote:** *(Inferred from document)* — The interviewer explicitly noted the need to move away from "Roast My Pricing" and "see how bad your pricing is" language based on Rashi's feedback
- **Timestamp:** N/A
- **Severity:** Medium — not a product objection, but a positioning one that could create friction with professional buyers and enterprise champions
- **Category:** GTM / Positioning Feedback
- **Summary:** Rashi's framing of what the product should do — "strategic pricing intelligence," "diagnostic insights," "support informed decision-making" — implies that the playful/confrontational "roast" branding clashes with how she and her peers think about pricing work. A KPMG analyst would not forward a "roast" tool to their VP. The language needs to match the seriousness of the use case to earn professional credibility.
- **Connects to:** New — but this objection will almost certainly recur with any enterprise or mid-market buyer in a finance/strategy role

---

## Pain Points Validated

### Pain: Manual Competitive Research Is Extremely Time-Consuming
- **Quote:** "Research and feature comparison are the most time-consuming parts. Automating extraction of pricing and features from websites would reduce analyst workload significantly."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** KPMG analysts manually compile competitor lists, manually scrape pricing pages, and manually build feature comparison tables — a process that takes days to weeks per engagement

---

### Pain: No Real-Time Monitoring — Only Periodic Reports
- **Quote:** "Real-time alerts on competitor pricing shifts would add strategic value. Sales teams could proactively engage clients when competitor prices change."
- **Severity:** HIGH
- **Category:** Stale Data
- **Currently solving with:** Periodic reports delivered at the end of a consulting engagement; no continuous monitoring infrastructure exists within KPMG's current workflow

---

### Pain: Feature Presence/Absence Tracking Is Manual and Error-Prone
- **Quote:** "Detailed feature lists across competitors, marking presence or absence. Number of competitors offering a feature indicates essentiality."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Analysts visit each competitor's website, manually validate exact wording, and note unique offerings — no automation, no version history

---

### Pain: No Systematic Tracking of Strategic Competitor Moves
- **Quote:** "Need to track investor reports, acquisitions, strategic moves." *(paraphrased from notes)*
- **Severity:** MEDIUM
- **Category:** Late Discovery
- **Currently solving with:** Ad-hoc research; likely relies on news alerts, Capital IQ for public companies, and analyst intuition

---

### Pain: Public Company Data Only via Capital IQ
- **Quote:** "Capital IQ for public company data only." *(extracted from KPMG process notes)*
- **Severity:** MEDIUM
- **Category:** Tool Fragmentation
- **Currently solving with:** Capital IQ covers public companies; private SaaS competitor data has no equivalent structured source — manually filled in

---

### Pain: Consulting Firms Can't Deliver Real-Time Intelligence at Scale
- **Quote:** "Automating competitive research would free consultants for higher-level analysis. KPMG would use a trusted tool to accelerate Phase 1."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Junior analyst labor, billable to the client at $100K+ per engagement; the inefficiency is currently the revenue model for consulting firms

---

## Product Feedback & Feature Requests

### Feedback: Product Must Be Descriptive, Not Prescriptive
- **Quote:** "The product would deliver diagnostic and descriptive insights, not prescriptive pricing recommendations. Support informed decision-making."
- **Type:** Positioning Feedback
- **Priority signal:** Strong — this is framed as a boundary condition for credibility, not a nice-to-have. A prescriptive tool would likely be dismissed by professional analysts.

---

### Feedback: Add "% of Competitors Offering This Feature" Metric
- **Quote:** "Number of competitors offering a feature indicates essentiality."
- **Type:** Feature Request
- **Priority signal:** Strong — Rashi uses this metric in her own manual process; it's a core analytical lens, not an enhancement

---

### Feedback: Real-Time Alerts Are the Killer Feature
- **Quote:** "Real-time alerts on competitor pricing shifts would add strategic value. Sales teams could proactively engage clients when competitor prices change."
- **Type:** Feature Request
- **Priority signal:** "Would pay for this" — described as adding "strategic value," connected to a clear downstream business action (proactive sales engagement)

---

### Feedback: Survey / Conjoint Analysis Integration for Phase 2
- **Quote:** "100-300 respondent surveys with conjoint analysis. Measures customer willingness to pay. Tests price increase scenarios (20-30%). Churn modeling based on price sensitivity."
- **Type:** Feature Request
- **Priority signal:** Nice to have for MVP, but high-value for enterprise tier — this is how pricing strategy is actually operationalized, not just observed

---

### Feedback: Sentiment Monitoring from G2, Product Hunt, Reddit, Twitter
- **Quote:** "G2, Product Hunt, Reddit, Twitter for customer sentiment and feature reception."
- **Type:** Feature Request
- **Priority signal:** Nice to have — mentioned as part of research methodology but not flagged as urgent; useful for a Phase 3 roadmap

---

### Feedback: Track Up to 10 Competitors — Tier Limit Is Correct
- **Quote:** *(Paraphrased)* "Typical analysis: 5-10 competitors. Distinguish direct vs indirect. Track market leader separately."
- **Type:** Positioning Feedback
- **Priority signal:** Strong validation — the 10-competitor cap on the paid tier directly matches industry norms; no need to over-engineer with "unlimited" as the default

---

### Feedback: Rename Away from "Roast" Language
- **Quote:** *(Inferred from notes)* — Rashi's professional framing implicitly contradicts confrontational branding
- **Type:** Positioning Feedback
- **Priority signal:** Strong — from a professional services context; would affect enterprise and mid-market adoption

---

## Strategic Insights

### Insight: Consulting Firms Are a Viable B2B2B Customer Segment
- **Quote:** "Automating competitive research would free consultants for higher-level analysis. KPMG would use a trusted tool to accelerate Phase 1."
- **Implication for Kompete:** Consulting firms (KPMG, Simon-Kucher, boutique pricing firms) have a strong economic incentive to use Kompete — it reduces junior analyst labor while maintaining client billing rates. A white-label or API-access tier priced at $5K–$10K/month could be a high-margin revenue stream *after* establishing credibility with 50+ direct customers.

---

### Insight: Repricing Is Cyclical and Trigger-Driven, Not Continuous
- **Quote:** "Average repricing: every 3 years. Triggers: New features (AI), market shifts, PE pressure. Price increases: 12-30% over 4 years tested."
- **Implication for Kompete:** The value of continuous monitoring isn't "reprice every day" — it's "be ready when a trigger event happens." Kompete's messaging should frame real-time alerts as trigger detection, not constant vigilance, which aligns better with how buyers actually use competitive intelligence.

---

### Insight: The Primary ICP Has No Dedicated Tool Today
- **Quote:** "Companies with $500k to $3M ARR can't afford $100k consulting but need pricing help. They rely on internal pricing analysts or marketing teams."
- **Implication for Kompete:** There is a clear tooling gap for internal pricing analysts at sub-$3M ARR SaaS companies — they do the work manually or don't do it at all. Kompete has no direct incumbent competitor in this segment; the competition is spreadsheets and Google, not Klue or Crayon.

---

### Insight: The Real Competitive Frame Is "Consulting ROI," Not "Klue vs. Crayon"
- **Quote:** "KPMG projects: 3 months, 5-6 consultants, >$100,000 per engagement. Repricing every 3 years on average."
- **Implication for Kompete:** The most compelling ROI story is not "we're cheaper than Klue" but "we replace a $100K consulting project." This repositions Kompete's price anchor entirely — $499/month ($6K/year) vs. $100K every 2–3 years is a 94% cost reduction for comparable Phase 1 output.

---

### Insight: Internal Pricing Analysts at Larger Companies Are a Secondary Buyer
- **Quote:** "Secondary market: Internal pricing analysts at larger companies."
- **Implication for Kompete:** There's a second ICP beyond the founder-led $500K–$3M company: pricing/finance team members at $5M–$50M ARR companies who have budget authority and would use Kompete as a research acceleration tool, similar to how Rashi herself described using it at KPMG. This persona has a higher willingness to pay and a clearer professional use case.

---

### Insight: AI Output Verification Is a Trust Barrier, Not Just a UX Issue
- **Quote:** "Use AI cautiously (don't fully trust outputs)."
- **Implication for Kompete:** KPMG analysts validate AI outputs against primary sources. Kompete must build source transparency (show the URL and raw text behind every extracted data point) into the product from day one — not as a compliance feature, but as the credibility layer that professional users require before they'll stake their analysis on it.

---

## Persona Signals

- **Buyer or User?** Primarily a **User** in a B2B2B scenario (she would use Kompete to accelerate her own consulting work) and a **secondary Buyer signal** — she noted KPMG would "use a trusted tool to accelerate Phase 1," implying she could influence a purchase decision within KPMG for a white-label or API tier. She is not the primary ICP buyer (internal analyst at a $500K–$3M ARR SaaS company), but her perspective is a strong proxy.
- **Willingness to pay:** High — validated $499/month as reasonable given the $100K consulting comparison. For a B2B2B consulting license, she implicitly signaled $5K–$10K/month could work ("reduces junior analyst workload by 50%, higher margin").
- **Decision process:** Would likely require a proof-of-quality moment — a free trial on a real project with verifiable output before recommending tool adoption internally at KPMG. Procurement at a Big 4 firm is process-heavy; initial adoption would likely route through a pilot program.
- **Current tools mentioned:** Capital IQ (public company data), manual website scraping, G2, Product Hunt, Reddit, Twitter, survey platforms for conjoint analysis (TypeForm/SurveyMonkey implied), AI tools (used cautiously, unnamed)

---

## Key Quotes (Top 5)

1. *"Real-time alerts on competitor pricing shifts would add strategic value. Sales teams could proactively engage clients when competitor prices change."* — Rashi directly naming the killer use case for Kompete Radar; this is a board-slide quote

2. *"Research and feature comparison are the most time-consuming parts. Automating extraction of pricing and features from websites would reduce analyst workload significantly."* — A KPMG analyst confirming that Kompete's core pipeline solves a real, costly pain point even at enterprise consulting firms

3. *"The product would deliver diagnostic and descriptive insights, not prescriptive pricing recommendations. Support informed decision-making."* — The single most important product framing quote; defines the correct positioning and corrects the original "roast" approach

4. *"Companies with $500k to $3M ARR can't afford $100k consulting but need pricing help. They rely on internal pricing analysts or marketing teams."* — Kompete's target market, defined in the words of a Big 4 pricing expert — ideal for pitch decks and investor materials

5. *"Automating competitive research would free consultants for higher-level analysis. KPMG would use a trusted tool to accelerate Phase 1."* — Opens the B2B2B channel; a future partnership or case study quote from Rashi would be one of the most powerful credibility signals Kompete could acquire
