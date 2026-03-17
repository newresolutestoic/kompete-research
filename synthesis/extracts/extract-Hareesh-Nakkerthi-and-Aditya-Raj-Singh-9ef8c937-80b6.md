# Interview Extract: Hareesh Nakkerthi

**Date:** 18th February, 2026
**Role/Company:** Product Manager (4 years), B2B SaaS brand protection company (steganography + computer vision; serves enterprise FMCG and automotive clients globally)
**Background:** Hareesh is a PM at an enterprise brand protection SaaS firm serving clients across North America, South America, Europe, and India. He has independently built and manages an N8N + LLM-powered competitive intelligence workflow for his organization, tracking 25 competitors weekly into a Google Spreadsheet.

---

## Objections & Challenges Raised

### Objection: Real-Time Ticker Feed Will Drive Away Users

- **Quote:** "A ticker would be a deterrent in adoption and would drive away people because that's not something that people are actually looking for on a hardly or a daily basis in a stable or not so much movement happening industries or spaces."
- **Timestamp:** [50:05]
- **Severity:** High — directly challenges Kompete's sub-3-minute alert and continuous monitoring differentiator
- **Category:** Value Prop
- **Summary:** Hareesh argues that constant streaming intel creates noise, not value. For companies in stable or slower-moving industries, real-time feeds are not just unnecessary — they risk hurting adoption by overwhelming users. He isn't opposed to alerts altogether, but insists they need to be filtered and rated by importance before delivery.
- **Connects to:** Information Overload objection pattern; similar concern about signal-to-noise ratio that may appear in other interviews

---

### Objection: Passive Feed Is "Good to Have," Not "Must Have"

- **Quote:** "For a system to feed that information it's a good to have meaning... a must have I think is more on the lines of when I'm looking for something I am slightly lost respect to which sources should I look for, what else should I cover. So that's the reason I'm saying in addition to the system of records that you're thinking in the MVP a simple agent that can use that system of records and provide information and insights. That would be a huge value add."
- **Timestamp:** [58:09]
- **Severity:** Critical — reframes Kompete's core monitoring product as a secondary feature; positions the search/query agent as the true MVP anchor
- **Category:** Product
- **Summary:** Hareesh explicitly demotes the automated push-feed to "good to have" status. His primary unmet need is a research agent he can query on demand — something that knows the competitive landscape and can answer targeted questions. He sees the system of record as foundational infrastructure, but the query interface as the daily-use value driver.
- **Connects to:** ChatGPT/Perplexity comparison — interviewee currently uses Gemini and ChatGPT as a fallback; Kompete risks being compared to free general-purpose LLMs without a differentiated query layer

---

### Objection: Competitive Intelligence Is Not a Daily Priority in Stable Industries

- **Quote:** "Competition analysis is something that in a high. In a fast moving setup or in a high growth organization or industry, the competition use is more checked more frequently. But in a relatively stable industry or relatively stable space, competition information is not something... it's a constant or a daily focus point."
- **Timestamp:** [50:05]
- **Severity:** High — challenges the GTM assumption that all B2B SaaS companies need continuous monitoring
- **Category:** Market Fit
- **Summary:** Hareesh introduces an important market segmentation insight: the value of real-time CI is proportional to industry velocity. In his niche (brand protection / steganography), weekly cadence is sufficient. Kompete's high-frequency alert messaging may only resonate with companies in fast-moving, competitive-dense SaaS verticals. Targeting stable or niche industries with the same pitch risks misalignment.
- **Connects to:** New — this is an industry-velocity segmentation signal not common in general SaaS CI conversations

---

### Objection: Strategic Recommendations Layer Is Premature

- **Quote:** "I think that can come later. I can follow once as you said, ensuring that the system of records is the right set of information. And then that's the major value add. I think the strategic investment, sorry, strategic insights part that can follow a little later."
- **Timestamp:** [1:01:28]
- **Severity:** Medium — pushes back on Kompete's planned third-layer AI strategy recommendations feature
- **Category:** Product
- **Summary:** While Hareesh acknowledges that predictive and strategic insights would be the "key" differentiator long-term, he recommends focusing the MVP on building a reliable system of record first. He is skeptical that LLM-generated strategic recommendations can account for internal company context (goals, constraints, partner dynamics), limiting their reliability.
- **Connects to:** ROI justification — if the AI recommendations are wrong, they erode trust in the whole platform

---

### Objection: One-Size-Fits-All Tracking Won't Work Across Product Types

- **Quote:** "One thing is one size fits all. You know, competitive intelligence maybe difficult I feel given the different products that you would be tracking. Right. And also yeah, that should be a configurable aspect, I feel with respect to what do you. What are you looking for? What do you want to track?"
- **Timestamp:** [1:09:39]
- **Severity:** Medium — raises UX/product concern about configurability
- **Category:** Product
- **Summary:** Hareesh flags that large companies track multiple product lines with different competitive sets, and a single default tracking profile won't be sufficient. He implies that without meaningful configuration options, enterprise adoption will stall at the team level. This is also implicitly an argument for workspace-level customization early in the product.
- **Connects to:** New — though related to buyer persona confusion around multi-product enterprise customers

---

## Pain Points Validated

### Pain: Competitive Intelligence Siloed Across Teams

- **Quote:** "The marketing team is doing it independently. The sales team and marketing team again that way in my organization there is some separation of this research that's happening in let's say product as well as marketing side. Not really unified. But yeah, with your thing coming in that is something that can be unified also."
- **Severity:** HIGH
- **Category:** Tool Fragmentation
- **Currently solving with:** Product team runs N8N workflow into Google Spreadsheet; marketing team does its own ad-hoc competitor messaging research; no shared system or cross-team synthesis

---

### Pain: No Discovery of Unknown/Emerging Competitors

- **Quote:** "That discovery of new upcoming names, that's something that would help us like the unknown. Unknown. Like we don't know that a competition is being built. Right. So that is something that we are mostly in the dark until it hits our radar either as I said in the technical research side of the sales or the customer side."
- **Severity:** HIGH
- **Category:** Late Discovery
- **Currently solving with:** Reactive discovery only — learning about new competitors from customers during active sales conversations, or from a dedicated R&D/research team monitoring academic papers and patent filings

---

### Pain: Manually Built CI Workflow Is Fragile and Labor-Intensive

- **Quote:** "We have a list of around 25 companies now that we have configured using an N8N workflow to look for their appearances, their websites on certain parameters... web search plus LLM on top of it and then [feeds into] a Google spreadsheet."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Custom-built N8N automation; web search; LLM summarization (Gemini / ChatGPT); Google Spreadsheet as system of record. Built and maintained by the product team.

---

### Pain: No Tracking of User Reviews or Voice of Customer on Competitor Products

- **Quote:** "Another thing is I think the voice of customers or the voice of employees as well as the user reviews, which is there but we're not really consuming. That is again, yeah, voice of customers."
- **Severity:** MEDIUM
- **Category:** Stale Data
- **Currently solving with:** Not addressed at all — acknowledged as a blind spot

---

### Pain: No Visibility Into Competitor Messaging Drift Over Time

- **Quote:** "After six months we are not always kind of seeing the drift... The system of records basically kind of gives you that viewpoint like okay in the last one year from say starting from 2024 to 2026 today what has been the change in their messaging, in their features, integrations, partnerships."
- **Severity:** MEDIUM
- **Category:** No System of Record
- **Currently solving with:** Periodic manual website checks; no versioned history or diff-tracking of competitor messaging

---

### Pain: No Targeted Search When Looking for Specific Competitive Intel

- **Quote:** "When I'm looking for something I am slightly lost respect to which sources should I look for, what else should I cover."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** General-purpose LLMs (Gemini, ChatGPT Deep Research) used ad-hoc; no purpose-built search grounded in a competitive data corpus

---

## Product Feedback & Feature Requests

### Feedback: Replace Raw Ticker With Insight Digest / Newsletter Format

- **Quote:** "Rather a good thing would be to create an insight out of it and predict an impact of the news that you come across and stitch that together as a newsletter. Not. Yeah, a newsletter of sorts. That would be more impactful... What it means for you, meaning if I am taking your product, what it means for me and my company."
- **Type:** Feature Request / UX Suggestion
- **Priority signal:** Strongly expressed — framed as the difference between adoption and abandonment; not "nice to have," closer to "this is the only format I'd actually use"

---

### Feedback: Natural Language Agent / Query Interface Over System of Records

- **Quote:** "When I am wanting to look for some information a natural language based search or discovery that's something that I think it's already... that would drive a good adoption I feel in the first MVP release."
- **Type:** Feature Request
- **Priority signal:** Explicitly labeled "must have" vs. the push-feed which he labeled "good to have" — this is the single strongest product signal from the interview

---

### Feedback: Competitor Pricing Tier Tracking and Historical Comparison

- **Quote:** "That would be a really good addition with the system of record that you're building Aditya, which is like a research agent. I feel like that is where there is a gap... tracking over time how competitor pricing tiers are changing — what's being feature-gated, what moved between tiers."
- **Type:** Feature Request
- **Priority signal:** Unprompted enthusiasm after Aditya demoed the pricing audit module — described as filling a genuine gap; moderate-to-strong signal

---

### Feedback: Importance/Severity Scoring on Incoming Alerts

- **Quote:** "It's like a metric that would help rate the importance of a news that could go as a ticker, not everything as a ticker because that's too much."
- **Type:** Feature Request / UX Suggestion
- **Priority signal:** Framed as a prerequisite for the alert feature to be usable at all — without it, the ticker is unusable

---

### Feedback: Persona-Based Filtering and Delivery of Intel

- **Quote:** "From your profile or your Persona it can be... from say a sales Persona, it can be something different. They post this customer, they kind of. So yeah, new partnership integration. Integration will be relevant for you probably. Right? So the faster you know, the better."
- **Type:** Feature Request
- **Priority signal:** Validated enthusiastically, though acknowledged as a future-state feature ("that will come later") — clear directional endorsement

---

### Feedback: Patent and Research Paper Monitoring

- **Quote:** "Papers become very important for us... we operate in the domain of steganography... the research kind of monitors that the names."
- **Type:** Feature Request
- **Priority signal:** Industry-specific need (IP-heavy sectors); moderate signal — handled by a separate research team today, so not a personal daily-use need for Hareesh but is an organizational gap

---

## Strategic Insights

### Insight: DIY CI Workflows Are Table Stakes Among Sophisticated Product Teams

- **Quote:** "We have a list of around 25 companies now that we have configured using an N8N workflow to look for their appearances... we get a report in a Google Excel, a Google spreadsheet every Monday or Tuesday."
- **Implication for Kompete:** The addressable market includes companies that have already proven the pain is real enough to self-solve. Kompete's pitch to this segment shouldn't be "do you need CI?" but "how much time and fragility are you tolerating with your DIY setup?" Hareesh's workflow is the archetype Kompete should be replacing.

---

### Insight: Industry Velocity Determines CI Frequency — And Therefore the Right Value Prop

- **Quote:** "In a high growth organization or industry, the competition use is more checked more frequently. But in a relatively stable industry or relatively stable space, competition information is not something that it's a constant or a daily focus point."
- **Implication for Kompete:** Kompete must segment its GTM by industry dynamism. Real-time alert messaging resonates with fast-moving, VC-backed SaaS markets (security, AI, fintech infrastructure) but falls flat in niche or industrially stable B2B segments. Consider two value prop frames: "always-on radar" for high-velocity markets, and "quarterly intelligence layer" for stable verticals.

---

### Insight: The Research Query Agent Is the "Killer Feature" — Not the Dashboard

- **Quote:** "For a system to feed that information it's a good to have meaning... a must have I think is more on the lines of when I'm looking for something I am slightly lost respect to which sources should I look for, what else should I cover."
- **Implication for Kompete:** Users are solving their push-intel problem with N8N or ChatGPT. What they lack is a trusted, domain-specific research agent they can ask targeted questions and get grounded answers from. Kompete should position the Strategy Timeline + corpus as the backend that makes its query agent trustworthy in ways ChatGPT cannot be.

---

### Insight: Competitive Intelligence Unification Is a Cross-Functional Selling Point

- **Quote:** "With your thing coming in that is something that can be unified also."
- **Implication for Kompete:** The ICP buyer is not just a product team but any company where marketing, sales, product, and CS are each running parallel, uncoordinated CI efforts. The "single system of record" messaging will land strongest at companies where this fragmentation is already causing pain and visible inefficiency — a strong discovery question for sales.

---

### Insight: Predictive Intel Is Valued but Viewed With Skepticism Without Internal Context

- **Quote:** "The third leg that you mentioned that would be the key. That would be the major contribution in the competitive space... The only thing is that we don't have information of how the internal strategy, how the internal teams are thinking about all these pointers. That is something that the LLM is not aware of."
- **Implication for Kompete:** Users will be excited by the predictive layer in demos but will discount recommendations they can't validate internally. Kompete should design the predictive intel layer with explicit evidence citations ("we believe X because: [patent filing] + [8 ML hires] + [acquisition]") to build trust, and allow users to annotate or contextualize predictions with internal knowledge.

---

## Persona Signals

- **Buyer or User?** Primarily a **User** (controls the tool build, not the budget). However, he is the internal champion who built and owns the CI workflow for the whole org — making him a high-influence evaluator and potential internal sponsor of a paid Kompete subscription.
- **Willingness to pay:** No pricing discussion occurred. Implied willingness is moderate-to-high given the time investment already made in building a DIY solution. Would likely need to justify to finance or a VP with a clear "we replaced X hours/week of manual work" ROI frame.
- **Decision process:** Evaluates tools by testing against real workflows. Would want to see a working prototype/POC before committing — explicitly offered to review Kompete's POC when ready. Likely needs to involve marketing leadership or a senior stakeholder for org-wide adoption.
- **Current tools mentioned:** N8N, Google Spreadsheet, Gemini, ChatGPT (Deep Research mode), RSS feeds (legacy), general web search, G2 / Capterra (aware but not actively consuming), Slack (mentioned as integration target)

---

## Key Quotes (Top 5)

1. *"For a system to feed that information it's a good to have meaning... a must have I think is more on the lines of when I'm looking for something I am slightly lost respect to which sources should I look for, what else should I cover."* — Directly inverts Kompete's assumed MVP priority; the query agent outranks the monitoring feed

2. *"A ticker would be a deterrent in adoption and would drive away people because that's not something that people are actually looking for on a hardly or a daily basis in a stable or not so much movement happening industries."* — Critical warning against defaulting to real-time alerts as the hero feature for all segments

3. *"That discovery of new upcoming names, that's something that would help us like the unknown. Unknown. Like we don't know that a competition is being built."* — Validates the blind spot that existing DIY workflows can't solve; a compelling acquisition hook for Kompete

4. *"The marketing team is doing it independently... Not really unified. But yeah, with your thing coming in that is something that can be unified also."* — Organic, unprompted validation of the cross-functional system-of-record value proposition

5. *"Rather a good thing would be to create an insight out of it and predict an impact of the news that you come across and stitch that together as a newsletter... What it means for me and my company — that way, and factual information versus an insight."* — Defines the exact output format that drives engagement; strong positioning input for Kompete's digest/alert UX
