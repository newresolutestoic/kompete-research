# Interview Extract: Sanchit Agarwal

**Date:** 7th March, 2026
**Role/Company:** Head of Data Platform, Sequoia (US-based brokerage firm); formerly Senior PM at Cleartax (4 years), ZS Associates (4 years)
**Background:** IIT 2016 graduate with deep B2B SaaS product experience, having scaled Cleartax's GST product from $1M to $10M ARR. Currently building a total compensation and benefits SaaS data platform at Sequoia, where he actively tracks competitors using a self-built automation stack.

---

## Objections & Challenges Raised

### Objection: Perplexity/Claude Already Does This
- **Quote:** "How is it different than what perplexity can do right now given a very decent quality prompt with the right amount of context?"
- **Timestamp:** [16:01]
- **Severity:** Critical — directly challenges core differentiation
- **Category:** Differentiation
- **Summary:** Sanchit has already built a personal workflow using Perplexity and Claude for deep monthly competitive research. He prefers these because they are specific, contextual, and query-driven. He is skeptical that Kompete adds meaningful signal beyond what a well-prompted LLM already delivers, especially for a power user who knows how to prompt.
- **Connects to:** ChatGPT/Perplexity comparison objection — a recurring pattern in interviews with technically sophisticated PMs/operators who have already stitched together their own AI workflows.

---

### Objection: Unclear Buyer vs. User Persona
- **Quote:** "I am not getting clarity on who is going to be your buyer. Well, probably a lot of people can use your product because it mixes different functions, brings insights from different functions. But I'm not also able to wrap my head around okay, what are different functions do I even need at a very high frequency?"
- **Timestamp:** [21:19]
- **Severity:** Critical — challenges GTM and go-to-market viability
- **Category:** GTM
- **Summary:** Sanchit draws on his extensive SaaS selling experience to highlight the danger of building for multiple user personas (PMMs, PMs, TA, sales) without a clear primary buyer. He notes that buyer and user personas are often vastly misaligned in B2B SaaS, and a tool that attempts to serve everyone risks being bought by no one. He also points out that competitive intelligence is historically an "orphan function" — it has reported to CPO, then CEO, then CBO — making budget ownership ambiguous.
- **Connects to:** Buyer persona confusion — likely a recurring objection; connects to the "who owns competitive intel" challenge observed in other interviews.

---

### Objection: Low Update Frequency for Enterprise Competitive Data
- **Quote:** "A very good feature I believe but it's like a competitive analysis which is not going to change probably in six months or nine months once I do it's done. It's like a play card for me... enterprise deployments, usually enterprises SAPs of the world, they do like deployments once in six months."
- **Timestamp:** [54:12]
- **Severity:** High — directly challenges the value of real-time/frequent monitoring for enterprise segment
- **Category:** Market Fit
- **Summary:** For enterprise-grade competitors (SAP, Oracle, Workday, High Radius), product features and integrations change on a 6-9 month cadence, not daily or weekly. Sanchit argues that the competitive intelligence dashboard shown — feature matrices, integration coverage, pricing — becomes a one-time artifact rather than a living feed. He implies that Perplexity deep research can handle this infrequent need adequately, reducing perceived necessity for a subscription tool.
- **Connects to:** Static vs. dynamic data tension — especially relevant when targeting customers who track large, slow-moving enterprise competitors.

---

### Objection: No Clear Lock-In / Substitutability
- **Quote:** "What is stopping any organization to probably let's say get glean and then provide it other data as well through some manner. And what are some of the deeper non-transient problems you are solving."
- **Timestamp:** [43:14]
- **Severity:** High — challenges defensibility of the product moat
- **Category:** Differentiation
- **Summary:** Sanchit asks why a company wouldn't just use a general-purpose enterprise search tool like Glean, augmented with additional competitive data. He distinguishes between transient problems (e.g., one-off hiring signal) and non-transient problems (deeply embedded workflows). His implicit suggestion: unless Kompete solves a deeply recurring, non-substitutable pain, it risks being a thin wrapper that gets bypassed.
- **Connects to:** New — not typically framed as a Glean comparison, but structurally similar to "why not just use ChatGPT" objections.

---

### Objection: ROI Hard to Justify for PMM / Marketing
- **Quote:** "PMM actually uses a lot of tools. PMM is a cost function. Real value. How do you calculate the ROI? Because at Clear when we moved the pricing from let's say 5 lakh average ASP to 20-25 lakh average ASP then it became very difficult to sell the product and it became very difficult to calculate the ROI."
- **Timestamp:** [25:00]
- **Severity:** High — directly challenges commercial viability for the identified buyer persona
- **Category:** Value Prop
- **Summary:** Sanchit flags that PMMs, despite being heavy tool users, sit in a cost center. As pricing increases, ROI justification becomes increasingly difficult to quantify. Drawing from his Cleartax experience, he notes that when ASP rose significantly, deals became harder to close precisely because the value was intangible. This creates a ceiling risk if Kompete targets PMMs as the primary user/buyer.
- **Connects to:** ROI justification — common pattern in B2B SaaS tool adoption for cost-center functions.

---

### Objection: Spreading Across Too Many Personas
- **Quote:** "You are spreading out too thin. User Persona. You will start getting a lot of requests."
- **Timestamp:** [51:xx–53:50]
- **Severity:** High — challenges product focus and roadmap integrity
- **Category:** GTM / Product
- **Summary:** When shown the product demo, Sanchit cautioned that targeting CS teams, SDRs, PMs, and PMMs simultaneously will fragment the product roadmap and dilute the core value proposition. He implied from experience that trying to serve multiple personas leads to a bloated product that satisfies no one deeply enough to create stickiness.
- **Connects to:** Buyer persona confusion objection above.

---

### Objection: India SME Market Won't Pay
- **Quote:** "SME doesn't want to pay. They want it to be free and even with the free product they are very demanding."
- **Timestamp:** [31:15]
- **Severity:** Medium — relevant if India is the initial target market
- **Category:** Market Fit
- **Summary:** Sanchit draws from Clear Tax's own experience pivoting away from SMEs: they don't pay, they churn, and they don't generate good word of mouth. He implicitly advises targeting mid-market or enterprise in India, which has a tighter but more reliable buyer community (e.g., CFOs are a close-knit community that does word of mouth referrals).
- **Connects to:** New — India-specific market fit concern not likely raised in conversations targeting US market.

---

## Pain Points Validated

### Pain: Automated Reports Are Too Noisy
- **Quote:** "The bi weekly report, I feel sometime it gets very noisy because very large report and lot of information is there. It's very difficult to find signals in such reports."
- **Severity:** HIGH
- **Category:** Information Overload
- **Currently solving with:** Falls back on personal deep research (Perplexity/Claude) on a monthly basis with specific, self-crafted prompts.

---

### Pain: Competitive Research Used to Take Days
- **Quote:** "Used to take me days at least. And then after that I would be frustrated enough to find out the signals."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** AI-powered deep research (Perplexity, Claude) and N8n-based crawlers that reduce the grunt work.

---

### Pain: AI Gives Surface-Level Answers Without Product Context
- **Quote:** "It still give you surface level answers as if we are trying to build it from scratch, but that's not the case."
- **Severity:** HIGH
- **Category:** Stale Data / Other
- **Currently solving with:** Manually injecting context into prompts; relying on personal domain knowledge to interpret AI output.

---

### Pain: No Source Traceability for Crawled Data
- **Quote:** "I am not fully aware of how does this crawler truly works and what are different sources does it depend on."
- **Severity:** MEDIUM
- **Category:** Tool Fragmentation
- **Currently solving with:** Accepts the opacity; supplements with manual research for validation.

---

### Pain: Competitive Intelligence Is an Orphan Function
- **Quote:** "It was under CPO for about two, three years and then it went under CEO then it went under the CBO. So there's a very like it's an orphan function at times I feel."
- **Severity:** HIGH
- **Category:** No System of Record
- **Currently solving with:** Not solved — acknowledged as a structural organizational problem.

---

### Pain: Competitor Marketing Videos Are Uninformative
- **Quote:** "Marketing videos are mostly gimmick. It doesn't show you the entire product... You mostly see a marketing video where some screens are there which are also not real and then they talk a lot but deliver less."
- **Severity:** MEDIUM
- **Category:** Access to Competitor Product
- **Currently solving with:** Relies on testimonials, customer reviews on G2/Capterra, and product copy/release notes to reverse-engineer actual capabilities.

---

### Pain: Difficulty Extracting Problem-Signal from Competitor Feature Launches
- **Quote:** "Nobody says that, okay, in your release note, you're not going to say I will solve this problem in the release notes. It would probably be, okay, we are launching this feature... So you read through that feature list or you read through that launch and you try to understand, okay, this is the kind of problem it gets."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Manual inference; reading between the lines of release notes and feature announcements.

---

## Product Feedback & Feature Requests

### Feedback: Initial Excitement on Reviews Dashboard
- **Quote:** "I will tell you while I look at this for the first time. It looks very exciting."
- **Type:** Positioning Feedback
- **Priority signal:** Positive first impression, but immediately followed by frequency/relevance concerns — "nice to have" for enterprise segment.

---

### Feedback: Feature Matrix / Integration Coverage Feels Like a One-Time Artifact
- **Quote:** "It's like a play card for me... a competitive analysis which is not going to change probably in six months or nine months once I do, it's done."
- **Type:** UX Suggestion / Positioning Feedback
- **Priority signal:** Implies this is not a "subscribe monthly for" feature but a one-time export — reduces recurring revenue justification.

---

### Feedback: Testimonials and Reviews Are the Highest-Signal Source
- **Quote:** "The reviews or the testimonies [are very helpful]. A lot of websites, a lot of competition have very good testimonials from their clients where they really talk about some deep problem statements."
- **Type:** Feature Request
- **Priority signal:** Strongly expressed — he actively mines testimonials for problem statements and would value a structured, aggregated view of these.

---

### Feedback: Prediction Layer Is the Real Differentiator
- **Quote:** "[Mixing signals across hiring and marketing to predict a product launch] — so we are really sure that they'll be launching in probably another six months. You get a sense of that."
- **Type:** Positioning Feedback
- **Priority signal:** Endorsed the multi-signal prediction concept as the one thing a well-prompted LLM alone cannot easily replicate. Would likely pay for this.

---

### Feedback: Backward Hypothesis Creation
- **Quote:** "Backward problem create... backward hypothesis creation. Probably helpful."
- **Type:** Feature Request
- **Priority signal:** Mild signal — the idea of reverse-engineering a competitor's problem-solving strategy from their feature releases resonated, though expressed informally.

---

## Strategic Insights

### Insight: The Power User Has Already Built Their Own Stack
- **Quote:** "These days we have automations which constantly crawls the competition's website, downloads their content, downloads their release notes, videos and then generates insights on top of it and then shares to the broader PM team."
- **Implication for Kompete:** Technically sophisticated PMs at mid-to-large companies are self-sufficient with N8n + LLM workflows. Kompete's ICP may need to exclude this persona or focus on what they still can't get (cross-signal prediction, verified sources, org-wide delivery). The real opportunity is the less technical buyer — or the team that doesn't have a power-user PM building infra for them.

---

### Insight: Competitive Intelligence Is Organizationally Homeless
- **Quote:** "It was under CPO for about two, three years and then it went under CEO then it went under the CBO. So there's a very like it's an orphan function at times I feel."
- **Implication for Kompete:** The budget owner for competitive intelligence is structurally unstable, which makes a top-down sales motion difficult. This supports a bottom-up PLG approach — getting PMMs or PMs addicted to the product — before escalating to a budget conversation with whoever owns the function at a given time.

---

### Insight: Enterprise Competitive Cycles Are Slow — Frequency Mismatch
- **Quote:** "Enterprises SAPs of the world, they do like deployments once in six months. Enterprise grade production as a product manager daily... it becomes my responsibility to figure out."
- **Implication for Kompete:** The 24/7 real-time monitoring value prop is compelling for fast-moving SaaS competitors but poorly matched to enterprise-tracking use cases. Kompete should segment by competitor-type, not just customer-type — customers tracking large enterprise rivals need quarterly intelligence digests, not daily alerts.

---

### Insight: Customer Testimonials Are an Underutilized Competitive Intel Source
- **Quote:** "Testimonials... where they really talk about some deep problem statements — okay, at my org we were facing this problem, this was the issue, this competition or this product came in and they solved this problem this way."
- **Implication for Kompete:** Testimonials on competitor websites are goldmines for extracting ICP pain points and use-case signals — yet they are rarely part of formal competitive intel tooling. This is a differentiating data source Kompete could explicitly index and structure.

---

### Insight: Microsoft Teams Is a Distribution Blocker
- **Quote:** "At Sequoia we don't use Slack, we have Teams and it's slightly difficult to set up these automations with Teams."
- **Implication for Kompete:** Slack-first alert delivery creates a GTM blind spot for enterprise customers on Microsoft Teams. Email delivery or a native Teams integration should be treated as a first-class requirement, not an afterthought, especially for enterprise/financial services targets.

---

### Insight: India Enterprise Buyers Are a Close-Knit Word-of-Mouth Network
- **Quote:** "Large organizations, the CFOs — we used to [sell to them] — and it's a very close-knit community. So as a [referral] high possibility."
- **Implication for Kompete:** If targeting India enterprise, a reference-led sales motion (warm intros through existing customers) may dramatically outperform cold outbound. One credible enterprise logo can unlock the entire buyer community.

---

## Persona Signals

- **Buyer or User?** User — Sanchit controls no budget for competitive intelligence tools; he is a power-user PM/data head who builds his own workflows. He could be a champion but not a buyer.
- **Willingness to pay:** Low-to-medium personal signal. He has invested time (not money) in building his own stack. Implied preference for tools that are either free/low-cost or solve something clearly unsolvable by Perplexity/Claude. Did not react to any pricing anchors.
- **Decision process:** Would evaluate bottom-up — tool has to prove immediate, personal value before he'd advocate upward. Likely tests with a free trial or demo, compares against his existing Perplexity workflow, and only escalates to a budget conversation if the signal quality is demonstrably superior.
- **Current tools mentioned:** Perplexity, Claude, ChatGPT, N8n (automation/crawling), Microsoft Teams, Glean (referenced as a potential alternative), Grammarly, Quillbot, SAP, Oracle, Workday

---

## Key Quotes (Top 5)

1. *"How is it different than what Perplexity can do right now given a very decent quality prompt with the right amount of context?"* — The core differentiation challenge, raised unprompted at [16:01]; the single most important objection to sharpen the pitch around.

2. *"Finding signals within the noise is where I am valuable... Where AI can get better is doing that given the context of work right now we are doing — is AI able to find the right signal? I right now don't see that happening."* — Validates the core pain AND identifies the product's unproven frontier simultaneously; ideal for framing the "why now" narrative.

3. *"It was under CPO for about two, three years and then it went under CEO then it went under the CBO. So there's a very like it's an orphan function at times I feel."* — Most quotable strategic insight; crystallizes the organizational chaos that makes competitive intel a systemic, not individual, problem.

4. *"The bi-weekly report — I feel sometime it gets very noisy because very large report and lot of information is there. It's very difficult to find signals in such reports."* — Clean, direct validation of the noise-over-signal pain point; usable verbatim in marketing copy or investor pitch.

5. *"What is stopping any organization to probably let's say get Glean and then provide it other data as well through some manner. And what are some of the deeper non-transient problems you are solving."* — The sharpest strategic challenge in the interview; forces Kompete to articulate its non-substitutable, sticky value before going to market.
