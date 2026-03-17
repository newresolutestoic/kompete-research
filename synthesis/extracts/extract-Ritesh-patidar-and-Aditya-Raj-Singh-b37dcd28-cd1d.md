# Interview Extract: Ritesh Patidar

**Date:** 28th February, 2026
**Role/Company:** Product Manager, 5 years in B2B SaaS (US market) — luxury retail/wholesale POS, back-office, inventory, and supply chain software
**Background:** IIM Indore MBA, mechanical engineering undergrad. Has managed product for a niche North American luxury retail vertical for ~5 years, handling competitive analysis as part of core PM responsibilities across a team of 5 PMs.

---

## Objections & Challenges Raised

### Objection: Cannot Access Competitor Product Directly
- **Quote:** "You cannot always experience the product because obviously you need to sign up for it. They'll ask for a company and if they know you are from a competitor they won't give you a demo and everything. So there's no a premium or a try in available."
- **Timestamp:** [07:13]
- **Severity:** High — directly limits the depth of intelligence Kompete can provide, and the founders themselves acknowledged this is a gap they "might not be able to solve today"
- **Category:** Product
- **Summary:** Ritesh's most acute pain is understanding what a competitor's product actually *does* — its workflows, UX, depth of features. Since competitors in niche B2B markets gate demos and trials aggressively, scraping public-facing web data will always leave a blind spot on actual product capabilities. He noted this as his primary frustration and was told explicitly by the founders it won't be solved near-term.
- **Connects to:** New — specific to complex B2B verticals with sales-led demos; not a classic web-scraping product gap

---

### Objection: Why Should I Trust This Data?
- **Quote:** "Like how do you make anyone trust this data? Like why should I trust this data?"
- **Timestamp:** [34:17]
- **Severity:** Critical — this is a trust objection that could block adoption entirely; raised spontaneously mid-demo without prompting
- **Category:** Value Prop
- **Summary:** Immediately upon seeing the product, Ritesh's first reaction was questioning data reliability. He followed up with a structured PM-style framing: adding confidence levels and explainability as a design pattern, citing an analogous AEO/brand-tracking product he'd evaluated that made explainability its core design principle. He also referenced that the founders' current answer (agents + human-in-the-loop) is not visible in the UI.
- **Connects to:** ChatGPT/Perplexity comparison — LLMs are already his current research tool, so he's calibrated to their hallucination risk; connects to AI data trust pattern seen broadly across AI-native products

---

### Objection: Reviews Not Useful for His Use Case
- **Quote:** "Reviews, to me, I don't think they're helpful because often and not they talk about the kind of service and all those things. Like from a product standpoint, for me, what this matters, like what's the other platforms other product is capable of doing and what we are capable of doing."
- **Timestamp:** [15:30]
- **Severity:** Medium — directly challenges one of Kompete's marketed differentiators (G2/Capterra review aggregation); however, this may be vertical-specific rather than universal
- **Category:** Value Prop
- **Summary:** When asked whether G2/review data would help justify premium pricing, Ritesh flatly said no. In his vertical (niche luxury retail POS), what matters is workflow depth and domain-opinionated product design — things reviews rarely capture well. This is a meaningful signal that review intelligence may be a weaker selling point for product-led buyers in complex B2B verticals.
- **Connects to:** New — specific to complex, workflow-heavy B2B products; may not generalize to all ICP segments

---

### Objection: GTM / Buyer Persona Fragmentation Risk
- **Quote:** "The decision maker. So let's see. You know, I'm running a B2B SaaS product company. I'm the CEO, I think, I don't know, like this is my thought, but as a CEO, I would be more interested in getting this for me and then I might share it across with my, like I'll share the logins with my other team members."
- **Timestamp:** [44:27]
- **Severity:** Medium — raises a real GTM question about who should be targeted first; Ritesh is the user persona but not the buyer
- **Category:** GTM
- **Summary:** Ritesh gently pushed back on the multi-persona GTM approach, suggesting that targeting CEOs/founders with a simplified executive view and letting them distribute downward is cleaner and more realistic. He implied that building for all personas simultaneously before nailing one could dilute the sales motion and add complexity to the first impression.
- **Connects to:** New — but consistent with classic "too broad ICP" early-stage GTM risk

---

### Objection: Type 1 and Type 2 Data Errors (Validated by Prateek, Confirmed by Ritesh)
- **Quote:** "So type one error where we are showing something that is incorrect... And then there should be something that we cannot capture and that's. So these are two kinds of errors." [Prateek raised; Ritesh acknowledged and affirmed, adding]: "explainability and a confidence level if you add that so would only give confidence to your users."
- **Timestamp:** [35:42] – [36:48]
- **Severity:** High — both false positives (showing wrong data) and false negatives (missing real data) could undermine decisions made based on platform outputs
- **Category:** Product
- **Summary:** Ritesh engaged with this seriously from a PM perspective. While Prateek offered sourcing links as the mitigation for Type 1 errors, Ritesh proposed an additive UX solution: confidence scores and explicit explainability layers, which he'd seen implemented well in an analogous AEO/LLM brand-tracking product. He positioned this not as a dealbreaker but as essential product design work before launch.
- **Connects to:** Data trust objection above — both stem from the same root concern about AI-generated intelligence reliability

---

## Pain Points Validated

### Pain: Blind-Sided by Unknown Competitors
- **Quote:** "At times it get to you know the worst where our sales team kind of demoed one of our competitor who were building the same product in the same space and they do a proper check and they went ahead and give them a demo."
- **Severity:** HIGH
- **Category:** Late Discovery
- **Currently solving with:** Ad hoc research; relying on sales team to surface competitors incidentally during prospect calls

---

### Pain: No Structured Competitive Tracking Cadence
- **Quote:** "There's no cadence. Actually it's. It's me who's doing the research. But I'm just trying to put at the gravity of me missing out or being in the dark spot as that it's coming from the sales."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Individual PM research, Confluence notes, CRM loss tracking — no systematic cadence

---

### Pain: Competitive Intelligence Siloed Across Teams
- **Quote:** "Previously this data used to be in silos across different teams. TA would know, okay, this competitor is hiring in this space... Probably the product team would have idea around, okay, what are the features... the CS and sales team would know probably feedback on the product."
- **Severity:** HIGH
- **Category:** Tool Fragmentation / No System of Record
- **Currently solving with:** Confluence for product team; separate CRM for sales; no cross-functional aggregation

---

### Pain: Reactive Feature Gap Discovery (Post-Deal-Loss)
- **Quote:** "So it's very late. It's very reactive process right now. So you get to know about it once you lost a deal to a competitor and you get to know."
- **Severity:** HIGH
- **Category:** Late Discovery
- **Currently solving with:** Post-mortems on lost deals (when prospects choose to share where they went); no proactive signal

---

### Pain: LLMs Used as Primary Competitive Research Tool
- **Quote:** "A lot of research right now happens via the LLMs or you know, Perplexity Chat, GPT or something like that. Because these companies may not be on the platforms like Angel List, YC or everything because the market is niche."
- **Severity:** MEDIUM
- **Category:** Manual Process / Stale Data
- **Currently solving with:** ChatGPT, Perplexity — ad hoc queries, no persistence or monitoring

---

### Pain: New Entrant Discovery in Non-Funded Markets
- **Quote:** "There are buying groups, there are industry groups, they also come together and fund any of these. So they also launch new products... the second or third generation has taken over and these guys are like more into tech... they'll hire someone in Philippines, Indonesia agency to develop the product for themselves."
- **Severity:** MEDIUM
- **Category:** Late Discovery / Other (non-traditional competitor sources)
- **Currently solving with:** Sales team anecdotes, Perplexity/ChatGPT searches; no systematic monitoring

---

### Pain: Cannot Verify Competitor Pricing Comprehensively
- **Quote:** "Some yes, some not." [on whether competitor pricing is exposed]
- **Severity:** MEDIUM
- **Category:** Pricing Opacity
- **Currently solving with:** Manual website checks; incomplete picture

---

## Product Feedback & Feature Requests

### Feedback: Explainability and Confidence Scores Are Essential
- **Quote:** "Explainability and a confidence level if you add that so would only give confidence to your users. So just coming from that point... so they were also building the same kind of report and I saw that their most focus was on keeping it explainable and like structuring it around the user trust."
- **Type:** UX Suggestion / Positioning Feedback
- **Priority signal:** Strong — unprompted, backed by competitive research from another product category, framed as a trust prerequisite not a nice-to-have

---

### Feedback: Support Tier and SLA Tracking
- **Quote:** "If you support you need to create a ticket and then the SLA is 48 hours to close the ticket or 12 hours. That makes a lot of difference in a retail business where you have a customer standing and let's say there's some issue with your POS... I think that's a maybe important insight because that differentiates the kind of service."
- **Type:** Feature Request
- **Priority signal:** Strong — novel signal (founders confirmed "that is a first we have heard basically"); Ritesh specified an exact taxonomy: community → chat → email → phone/Teamviewer, with SLA data as the key differentiator; directly tied to his competitive positioning need

---

### Feedback: Customer Recognition / Named Customer Tracking
- **Quote:** "Please be also planning to add like maybe you know, number of customers that they have or any, you know, big brand logos that they have."
- **Type:** Feature Request
- **Priority signal:** Moderate — mentioned casually; founders showed it already existed in a "Customer Recognition" tab, suggesting validation rather than a gap

---

### Feedback: Integration and Partnership Monitoring (Validated)
- **Quote:** "Anyone who, because you know they can do integrations or partnership with any of the other extended service provider... those partnerships are usually revealed on the company's websites. So that information we will get to know it when we log in. So we might not be going and searching the websites every day. But yeah, the information if you know, could be more inbound like as soon as it's there, like as a change, you know, for sure."
- **Type:** Feature Request
- **Priority signal:** Strong — specifically named integration/partnership monitoring as one of the top two signals he'd want tracked; real-time alerting on changes explicitly valued over periodic manual checking

---

### Feedback: Reviews Are NOT a Differentiator for His Vertical
- **Quote:** "Reviews, to me, I don't think they're helpful because often and not they talk about the kind of service and all those things. Like from a product standpoint, for me, what this matters, like what's the other platforms other product is capable of doing."
- **Type:** Positioning Feedback
- **Priority signal:** High (as a negative signal) — actively disqualified this feature for his use case; product capability comparison is what drives his decisions

---

## Strategic Insights

### Insight: CEO is the Buyer, Not the PM
- **Quote:** "As a CEO, I would be more interested in getting this for me and then I might share it across with my, like I'll share the logins with my other team members, my product managers, my CS."
- **Implication for Kompete:** The CEO/founder is the natural buyer who controls budget and distribution — selling to PMs first may create adoption without a budget owner. Kompete should build an executive summary layer (2-3 tabs max) designed for a 5-minute MBR/WBR review, and use that as the wedge into the C-suite rather than selling feature depth to individual contributors first.

---

### Insight: Non-VC-Backed Competitors Invisible to Standard Monitoring
- **Quote:** "Because these companies may not be on the platforms like Angel List, YC or everything because the market is niche, the industry is niche, they don't get funded like that. But they're mostly bootstrapped, self funded or they'll get angel fund... in form of the industry groups or the buying groups that are there."
- **Implication for Kompete:** Standard funding signal tracking (Crunchbase, AngelList) will miss an entire class of competitors in traditional or niche B2B verticals. Kompete needs supplementary discovery signals — industry association announcements, LinkedIn company page creation, domain registration monitoring, or even job board scraping — to catch bootstrapped entrants before they appear in deal loss reports.

---

### Insight: LLMs Are the Incumbent, Not Klue or Crayon
- **Quote:** "A lot of research right now happens via the LLMs or you know, Perplexity Chat, GPT or something like that."
- **Implication for Kompete:** In this segment (niche B2B, lean teams), the primary competitor being displaced is not Klue ($40-80K/yr) but ad hoc ChatGPT/Perplexity usage. Kompete's real switching cost argument should be: persistence, proactive monitoring, and structured output — things LLMs don't provide. Pricing and positioning should reflect this "structured LLM alternative" angle, not just "cheaper Klue."

---

### Insight: Support Intelligence Is an Untapped Competitive Dimension
- **Quote:** "The major segmentation would be like is it no human involved... so you're getting live support, not it's not a live support, it's chat only support or email only support or community only support or are you able to actually email someone get on a teams call or a team viewer... SLAs are also mentioned on the website."
- **Implication for Kompete:** Support tier and SLA tracking emerged as a novel, first-of-kind signal in this interview. For service-heavy verticals (retail POS, fintech, healthcare SaaS), this data point is a genuine competitive differentiator and a gap no current tool fills. This could be a high-value niche feature that drives word-of-mouth in support-sensitive industries.

---

### Insight: Feature Roadmap Decisions Need Demand Signal, Not Just Gap Signal
- **Quote:** "I need to get the information beforehand. So if I can get that information beforehand... if there's something where I can know that, you know, X feature not built, there are like I'm gonna lose or something like that, then you know, it becomes important for me to kind of evaluate it more and see if you know, it's actually providing some value."
- **Implication for Kompete:** PMs don't want a raw list of "competitors have this, you don't" — they need demand-weighted feature gap intelligence. Knowing a competitor has a feature is table stakes; knowing that feature is a *frequent deal-loss driver* is what justifies putting it on the roadmap. Kompete should consider layering CRM signal integrations (e.g., loss reason data from HubSpot/Salesforce) onto feature gap analysis to close this loop.

---

## Persona Signals

- **Buyer or User?** User — Ritesh is a PM who would actively use the platform day-to-day. He explicitly identified the CEO/founder as the budget holder and likely buyer. He can, at best, refer the tool to a senior PM colleague internally.
- **Willingness to pay:** Not discussed explicitly. He expressed genuine enthusiasm ("I do feel a lot of value in it") but was not asked about pricing. His company pays "hundreds of thousands of dollars a year" for POS software, suggesting the business has budget — question is whether competitive intelligence sits in PM's budget or CEO's.
- **Decision process:** Would want to pilot with real competitor data first, share with one senior PM colleague for internal validation, then presumably escalate to management. Discovery → demo → pilot pattern mirrors how his own company sells. No mention of formal RFP or procurement process — likely informal evaluation.
- **Current tools mentioned:** Confluence (competitive notes), CRM (sales, vendor unknown), ChatGPT, Perplexity, Google (general research)

---

## Key Quotes (Top 5)

1. *"At times it get to you know the worst where our sales team kind of demoed one of our competitor who were building the same product in the same space and they do a proper check and they went ahead and give them a demo."* — On the severity of late competitor discovery; validates the core Kompete pain point with a visceral real-world example

2. *"So it's very late. It's very reactive process right now. So you get to know about it once you lost a deal to a competitor."* — Clearest articulation of the status quo failure mode; pitch-deck ready

3. *"Like how do you make anyone trust this data? Like why should I trust this data?"* — First and most instinctive reaction upon seeing the product demo; the single most important product design challenge identified in this interview

4. *"A lot of research right now happens via the LLMs or you know, Perplexity ChatGPT or something like that. Because these companies may not be on the platforms like AngelList, YC or everything because the market is niche."* — Reveals who the real incumbent is in lean B2B teams; critical for competitive positioning

5. *"Explainability and a confidence level if you add that so would only give confidence to your users... I saw that their most focus was on keeping it explainable and like structuring it around the user trust."* — Actionable, specific UX recommendation from a PM-trained evaluator; doubles as a product principle and a trust-building mandate
