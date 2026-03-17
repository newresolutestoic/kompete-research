```markdown
# Interview Extract: Sai Bhaskar Devatha

**Date:** 10th February, 2026
**Role/Company:** Product Manager (AI/Knowledge Assistant Products), LTropy
**Background:** PM at LTropy, a unified conversations platform for U.S. credit unions (~$70–80M ARR, 250 employees, 28 product lines). Sai joined ~6 months ago and owns 3 product lines including an internal-facing AI knowledge assistant for credit union employees. Prior experience at Appraised (B2C, daily competitive tracking) and RKCM (hedge fund fintech, no CI process).

---

## Objections & Challenges Raised

### Objection: B2B Competitors Deliberately Obscure Product Info
- **Quote:** "The problem with these B2B companies is they don't put all their features on the landing page because it is sales heavy. They reach out to the customers with a different collateral like a PDF or PPT or something which I can't get."
- **Timestamp:** [19:32]
- **Severity:** High — directly caps the value a public-data CI tool can deliver in sales-led enterprise markets
- **Category:** Value Prop
- **Summary:** Enterprise competitors in Sai's niche don't expose features, pricing, or detailed product specs publicly. The real intelligence lives in offline sales collateral (PDFs, decks) that no scraping-based tool can access. Aditya acknowledged this limitation and positioned Kompete around publicly available data only, which Sai accepted but noted as a real gap.
- **Connects to:** New — specific to sales-led/enterprise market dynamics; likely recurs in other enterprise-facing interviews

---

### Objection: Competitor Products Are Gated — No Free Trials
- **Quote:** "They don't let me sign up. Right. They have some kind of mechanism — even we have mechanisms where we don't let others sign up. They don't let us sign up to see the product. Right. And these big companies don't have free trials or anything. So it's extremely difficult for us to know how the screens look."
- **Timestamp:** [19:36]
- **Severity:** High — the richest CI (actual product UX/feature depth) is inaccessible to any external tool
- **Category:** Product
- **Summary:** Gated products and the absence of free trials mean true product-level competitive intelligence requires manual workarounds (fake sign-ups, webinar infiltration). This is a structural limitation that Kompete cannot solve via public data monitoring. Sai drove home the point that without product access, feature claims can only be taken at face value from marketing copy.
- **Connects to:** Related to the "Access to Competitor Product" pain point; see also the marketing buzzword objection below

---

### Objection: Marketing Claims ≠ Reality — Claim Verification Is Hard
- **Quote:** "They use marketing terms like, for example, reinforcement learning is one of what competitors are using as a marketing material. But in reality it is some random thing that they have done, but they named it as reinforcement learning. Now for a customer who doesn't understand reinforcement learning, they will say, you know, they have reinforcement learning, why don't you have it?"
- **Timestamp:** [26:06]
- **Severity:** Medium — undermines the reliability of any CI derived purely from public content
- **Category:** Value Prop
- **Summary:** Competitors use technical buzzwords loosely in marketing, creating false impressions of capability. If Kompete surfaces these claims at face value, it may inadvertently amplify competitor misinformation rather than verify it. Sai implies that copy intelligence must be paired with claim verification context to be truly useful.
- **Connects to:** New — this is a nuanced signal about the reliability layer Kompete needs; relates to AEO/claim verification differentiator

---

### Objection: Pricing Intelligence Has No Utility in Their Domain
- **Quote:** "Pricing again will be very helpful. But we don't have the information outside. We can't really answer that."
- **Timestamp:** [44:09] (in response to Aditya demoing the pricing audit feature)
- **Severity:** Medium — one of Kompete's demo features is immediately deprioritized by this persona
- **Category:** Pricing
- **Summary:** LTropy's competitive set is 100% sales-led with no public pricing. The pricing audit feature Aditya showed resonated in concept, but Sai explicitly called it out as not actionable for his use case. This likely applies broadly to enterprise/vertical SaaS buyers.
- **Connects to:** Likely recurs in other enterprise-segment interviews; the pricing feature may be more relevant to mid-market PLG companies

---

### Objection: Multi-Product-Line Complexity — One Workspace Won't Fit All
- **Quote:** "Because there are lots of product lines inside. So email for credit unions will have 20, 30 competitors, or AI agents for credit unions will have 20–30 different competitors than AI agents for internal teams. Whatever I'm doing, it's not common for the entire platform. It is very specific to the product line that I am working on."
- **Timestamp:** [16:19]
- **Severity:** High — Kompete's current framing (company-level CI) doesn't map cleanly to how multi-product companies are organized
- **Category:** Product / Market Fit
- **Summary:** LTropy has 28 product lines, each with entirely different competitor sets, managed by different PMs. A single company-level dashboard creates noise rather than signal for individual PMs. Product-line-level workspaces, filtering, and segmentation appear to be a prerequisite for adoption at companies like LTropy.
- **Connects to:** New — this is a structural product architecture challenge; key GTM implication for land-and-expand

---

### Objection: Enterprise Procurement Is a Long, Compliance-Heavy Process
- **Quote:** "The company follows a particular procedure to onboard new tools. So they typically have a POC period of a month and then they do a couple of security checkups. So because we handle data of credit unions... SOC 2 Type 2 I think is required... And then we have a vendor team who does analysis of 15 days on your [tool]. They might ask you some questions and once it's there and the pricing is approved, that's when we onboard new tools."
- **Timestamp:** [46:04]
- **Severity:** High — significantly extends sales cycle; compliance certification may be a hard gate
- **Category:** GTM
- **Summary:** LTropy's fintech-adjacent positioning (serving credit unions) means their procurement process includes SOC 2 Type 2 requirements, a dedicated vendor review team, and multi-week security evaluation on top of a POC. For an early-stage startup like Kompete, this is a real barrier to closing a deal, even after proving value. The buyer journey is: prove value in POC → pass security → get pricing approved → onboard.
- **Connects to:** New — compliance/security as a GTM gating factor; likely to recur in regulated-industry prospects

---

## Pain Points Validated

### Pain: Monthly Manual Website Crawls Are Exhausting
- **Quote:** "Every month we have a call with the marketing team. So it's my job to keep that marketing material updated. So before the meeting I kind of go through all the websites, all my competitors... I just need to verify it, cross verify it every single month to see whether it is correct or not."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Manual website reviews before monthly marketing meetings; updates a competitive feature analysis table (yes/no matrix) and written comparison docs across 3 products

---

### Pain: Late Discovery of Competitor Feature Launches
- **Quote:** "The founders will post on their LinkedIn that we are launching this or somewhere. If I had missed that point, we reach to it later. So I need something where I can keep track of what other competitors are doing."
- **Severity:** HIGH
- **Category:** Late Discovery
- **Currently solving with:** Occasional LinkedIn browsing; no systematic monitoring; often learns about launches from sales calls or all-hands meeting callouts after the fact

---

### Pain: No System of Record — Institutional Memory Gets Lost
- **Quote (Sai):** "I mean, the time spent on that to create a similar kind of report. I have to do it mapping in my brain — that last time I've seen this website, this is what I've seen. Now they've changed."
- **Quote (Aditya, confirmed by Sai):** "We have to kind of create some spreadsheet, keep the messaging there. Then after five months probably a new spreadsheet will be created and that old one will get lost. And then again, you cannot humanly check all the 5, 6, 7 positioning changes they have done."
- **Severity:** HIGH
- **Category:** No System of Record
- **Currently solving with:** Spreadsheets (not maintained long-term); mental recall; no versioning or historical diff capability

---

### Pain: Cannot Access Competitor Products — Forced Into Dangerous Workarounds
- **Quote:** "I created a fake LinkedIn profile, reached out to the employees of the company saying that, you know, I want to join the company, can you give me a little bit of time to talk... I signed up with a different email, joined the [competitor's weekly webinar] session, saw the platform, asked some questions. That's how I gathered what features they have."
- **Severity:** HIGH
- **Category:** Access to Competitor Product
- **Currently solving with:** Fake LinkedIn profiles for employee outreach, pseudonymous email sign-ups for competitor webinars, reaching out to churned customers for feedback (received generic answers)

---

### Pain: Competitive Intelligence Is Siloed Across Teams With No Central Hub
- **Quote:** "We get a weekly message from the partnership's head who messages that in this last one week, these are the news around credit unions... Marketing has five people whose sole job is to collate information from all the product teams... Sales team tells us we've lost this deal because that other company has provided some features."
- **Severity:** MEDIUM
- **Category:** Tool Fragmentation
- **Currently solving with:** Ad-hoc communication across Slack/email; no single source of truth; each team (sales, marketing, partnerships, product) maintains its own partial picture

---

### Pain: Competitor Messaging Changes Faster Than Teams Can Track
- **Quote:** "This is also another pain point — they make a lot of change. So because AI is moving very fast, they release a lot of new features... They change their positioning. Initially we positioned it in this way — customer facing and employee facing. Then they also changed their positioning into that — customer facing and employee facing — maybe a year back."
- **Severity:** HIGH
- **Category:** Stale Data
- **Currently solving with:** Monthly manual reviews; changes between reviews go undetected; positioning drift is pieced together from memory

---

### Pain: Battle Card Creation Is Entirely Manual and Time-Consuming
- **Quote:** "So I have to try out their product and why should they prefer LTropy? I have to write a blog or kind of create a battle card in general. Right. That is the second type of competitive analysis that I do."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Manual product trials, blog research, writing battle cards from scratch; sales team requests them reactively after losing deals

---

## Product Feedback & Feature Requests

### Feedback: Positioning Drift / Website Change Tracking Is the #1 Priority Feature
- **Quote:** "Positioning drift is like what I generally do if I'm searching their websites once in a while. This is very helpful for me — positioning drift — because it will help me understand how are they changing their naming, how are they positioning their products, or are they building new features. So I'll club both of them together. It is basically for me to track websites."
- **Type:** Feature Request
- **Priority signal:** Strong — Sai named this as one of the two use cases he would use immediately if the product existed today; "very helpful for me" (unprompted)

---

### Feedback: Social Media Monitoring (LinkedIn + Twitter) Is Explicitly Requested
- **Quote:** "If we can add social media also into it, LinkedIn for example, or Twitter, that would give the entire picture of what the other company is doing."
- **Type:** Feature Request
- **Priority signal:** Strong — proactively raised without prompting, described as completing the "entire picture"; LinkedIn is where competitor founders announce launches

---

### Feedback: Keyword / Jargon Frequency Analysis Across Competitor Sites
- **Quote (exchange):** Aditya: "We can have basically a word count, simple word count of like what words or jargons are they using across the website... these words are the most used words... The reinforcement learning is something that they were using that you are not using. So that analysis — the words that they are using but you are not using." Sai: "Correct, correct."
- **Type:** Feature Request
- **Priority signal:** Medium — enthusiastically confirmed when suggested, directly connected to a real problem (competitor buzzword strategy); not raised organically but validated strongly

---

### Feedback: Product-Line-Level Workspaces Are a Prerequisite for Adoption
- **Quote:** "Correct. You can have different workspaces probably... for your use case for your product line, you'll utilize one... the other teams will utilize the other workspace where they get only the relevant thing."
- **Type:** Feature Request
- **Priority signal:** Critical — without this, the tool creates noise rather than signal for companies with multiple product lines; this is effectively a blocking requirement for Sai's use case

---

### Feedback: Pricing Audit Feature Has Low Utility for Sales-Led Verticals
- **Quote:** "Pricing again will be very helpful. But we don't have the information outside. We can't really answer that."
- **Type:** Positioning Feedback
- **Priority signal:** Negative signal — explicitly deprioritized; Kompete should lead with positioning/content/social tracking when selling to enterprise-vertical companies, not pricing intelligence

---

### Feedback: Auto-Generated Reports Would Already Be Valuable (Even Pre-Product)
- **Quote:** "No, agree. Yeah. I mean the time spent on that to create a similar kind of report, right. I mean I have to do it mapping in my brain... But you are making it extremely easy for me to have it in one place."
- **Type:** UX Suggestion
- **Priority signal:** Strong — open to receiving a one-time AI-generated report as a first step; validates a report-first, product-second GTM motion

---

## Strategic Insights

### Insight: Extreme Manual Workarounds Signal a Massive Legitimate Tooling Gap
- **Quote:** "I created a fake LinkedIn profile, reached out to the employees of the company saying that, you know, I want to join the company... I signed up with a different email, joined the session, saw the platform, asked some questions."
- **Implication for Kompete:** The competitive intelligence pain is severe enough that practitioners resort to ethically questionable tactics (impersonation, deception). This is a strong indicator that no legitimate automated tooling currently fills this gap — Kompete's opportunity is to replace covert human effort with transparent, automated monitoring of public signals.

---

### Insight: Customers of Customers Are Also Building DIY CI Tools
- **Quote:** "I've seen that a couple of credit unions have created multiple assistants for each of their competitors... They created a competitive analysis bot called Guardian CU. And then they ask questions to it — 'What are your loan rates?' It will give you a loan rate and they'll compare it with their own loan rates."
- **Implication for Kompete:** The competitive intelligence pain cascades downstream — not just SaaS vendors but their enterprise customers are improvising CI tooling. This hints at broader market demand beyond B2B SaaS, and potentially a channel play: if platforms like LTropy embedded CI natively, they'd be solving a pain their own customers feel.

---

### Insight: Partnerships and Integration Signals Are an Undervalued CI Vector
- **Quote:** "We get a weekly message from the partnership's head who messages that in this last one week, these are the news around credit unions... Competitors do go out of the industry and play with some other industries as well... The partnership thing that you said and the integrations that they are doing give you a hint into what Persona are they next targeting."
- **Implication for Kompete:** Partnership announcements and integration launches are a leading indicator of competitor strategy shifts. Tracking these signals as part of a "Strategy Timeline" could surface directional intelligence (new market entry, persona targeting) well before product launches become visible — a high-value differentiator over simple website monitoring.

---

### Insight: In Niche Verticals, Competitor Set Is Hyper-Specific and Varies by Product Line
- **Quote:** "Because there are lots of product lines inside. So email for credit unions will have 20–30 competitors, or AI agents for credit unions will have 20–30 different competitors than AI agents for internal teams. Whatever I'm doing, it's not common for the entire platform."
- **Implication for Kompete:** In vertical SaaS companies, a single company-level CI view is nearly useless. Kompete's product architecture must support granular, user-level workspace configuration tied to specific competitor sets — or it risks failing adoption even among enthusiastic users like Sai.

---

### Insight: Prior B2C Experience Normalized Daily CI Habits — B2B Lacks the Tooling
- **Quote:** "It used to be my job that every single day morning I have to open all my competitor websites and see what they are doing. Are they launching new programs? What is the price point of that program?... That was a B2C company."
- **Implication for Kompete:** The behavioral habit of daily competitive monitoring exists in practitioners who came from B2C environments. Kompete's "morning news feed" or alerting framing directly maps to this ingrained behavior and will feel natural to this persona — the sell is automation of a familiar workflow, not adoption of a new one.

---

### Insight: The Competitive Intelligence Workflow Has Multiple Distinct Stakeholder Entry Points
- **Quote:** "Marketing will reach out... sales team will reach out... the partnership head sends weekly messages... it's my job as PM to keep the marketing material updated."
- **Implication for Kompete:** At LTropy, CI is simultaneously owned by Product (feature gap analysis), Marketing (positioning and copy), Sales (battle cards and win/loss), and Partnerships (ecosystem news). Kompete's team-specific delivery feature is validated — but the go-to-market entry point matters. Product Managers appear to be the most pain-aware and most willing to champion a tool internally.

---

## Persona Signals

- **Buyer or User?** User, not budget holder. Sai is a hands-on PM who would use the tool daily and champion it internally. The buying decision would require sign-off from the Head of AI Product Management and go through a formal procurement process. He proactively offered to connect Aditya with the marketing stakeholder (Canada-based) and other PMs as additional references.
- **Willingness to pay:** Not explicitly discussed. Sai did not push back on pricing and expressed genuine excitement ("I'm very excited"). His company's $70–80M ARR suggests budget exists, but procurement is process-heavy and compliance-gated — not price-sensitive in the traditional sense.
- **Decision process:** (1) Another discovery/scoping call with Aditya + co-founder → (2) Kompete generates a sample report for Sai's specific use case → (3) If valuable, Sai shows leadership → (4) Formal POC (~1 month) → (5) Security review / SOC 2 check (~15 days, vendor team) → (6) Pricing approval → (7) Onboarding. Timeline estimate: 2–4 months minimum.
- **Current tools mentioned:** Manual website browsing, spreadsheets (ad hoc), fake LinkedIn profiles (covert), pseudonymous email sign-ups for competitor webinars, Microsoft Copilot (as a competitor being tracked, not a CI tool), LTropy's own internal AI knowledge assistant (used as a CI workaround by some credit union customers), G2/Captera (mentioned by Aditya — Sai confirmed they do **not** actively use these), partnership team Slack messages (informal newsletter)

---

## Key Quotes (Top 5)

1. *"I created a fake LinkedIn profile, reached out to the employees of the company saying that, you know, I want to join the company... I signed up with a different email, joined the [competitor webinar] session, saw the platform, asked some questions. That's how I gathered what features they have."* — On the lengths practitioners go to for competitive intelligence in gated B2B markets; signals massive legitimate tooling gap

2. *"It is very difficult to do it every time now and then the frequency. I mean one time you can do — put all your energy into this. But keeping it updated is where the problem comes. At least for us."* — Core pain point validation; the one-time research vs. ongoing maintenance gap is Kompete's exact wedge

3. *"They use marketing terms like, for example, reinforcement learning... but in reality it is some random thing that they have done. Now for a customer who doesn't understand reinforcement learning, they will say — you know, they have reinforcement learning, why don't you have it?"* — Exposes a dangerous downstream effect of unverified competitor claims reaching sales conversations; validates claim-verification as a must-have layer

4. *"I have to do it mapping in my brain — that last time I've seen this website, this is what I've seen. Now they've changed. But you are making it extremely easy for me to have it in one place."* — Direct validation of the Strategy Timeline / historical system-of-record concept; this is a homepage-ready quote

5. *"A couple of credit unions created a competitive analysis bot called Guardian CU. And then they ask questions to it — 'What are your loan rates?' It will give you a loan rate and they'll compare with their own loan rates."* — Unexpected downstream insight: the CI pain exists at the customer-of-customer level too; strong signal for broader market demand and potential platform/channel strategy
```
