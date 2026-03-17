# Interview Extract: Manasa Maragiri

**Date:** 2nd February, 2026
**Role/Company:** Pricing Consultant / Implementation Specialist at Tech Mahindra (Synchron Price practice); formerly a Java developer
**Background:** Six years in enterprise pricing consulting, specializing in Synchron Price deployments across ~50 global manufacturing customers (automotive, cargo, food) spanning Europe, US, APAC, and India. Deep expertise in price modeling, stakeholder management, and moving manufacturing clients off Excel-based workflows.

---

## Objections & Challenges Raised

### Objection: Competitor Pricing Data Is Not Publicly Available in Manufacturing
- **Quote:** "No, no, no. It's mostly the product. I mean all the teams that who will be working stakeholders will have all the idea and they'll have people to catch hold of all these prices. So it's an internal information, so we'll get it done somewhere."
- **Timestamp:** [26:11]
- **Severity:** Critical — directly challenges the core web-scraping / real-time monitoring value proposition of Kompete.ai if applied to manufacturing verticals
- **Category:** Market Fit
- **Summary:** Manasa confirms that in manufacturing, competitor pricing is not surfaced on the public internet. It is gathered informally, person-to-person ("you'll hear some number and then you'll just assume it"), and then manually uploaded as static data into tools like Synchron. A product that promises to auto-fetch competitor prices from the web would find little surface area to scrape in this industry. This makes the manufacturing vertical a poor fit for Kompete.ai's current architecture.
- **Connects to:** New (specific to manufacturing sector); contrasts favorably with the B2B SaaS thesis where pricing pages, feature tiers, and G2/Capterra reviews ARE public.

---

### Objection: Static Data Is the Current Accepted Standard, Not Dynamic Monitoring
- **Quote:** "It's not dynamic, it's a static one. Whenever you change it will get changed. You don't need a ERP system to get the competitor data. It's easier to do it in the system itself."
- **Timestamp:** [25:34]
- **Severity:** High — suggests that manufacturing buyers have low expectations for real-time competitor monitoring; they are satisfied with manual, periodic uploads
- **Category:** Value Prop
- **Summary:** The current workflow treats competitor data as a static input updated manually by the pricing team, not a live feed. This implies that the "24/7 monitoring" and "sub-3-minute alerts" positioning of Kompete.ai would be solving for a problem that manufacturing customers don't yet feel the pain of. There is no perceived urgency around latency of competitive data in this segment.
- **Connects to:** Stale Data pain point (see below); also echoes a broader market education challenge.

---

### Objection: Global SaaS Products Break Local Market Customization
- **Quote:** "If you focus more on global market it becomes difficult when you want to implement it on the local market... the way it is handled here there it's totally different and the way they arrive at price and we arrive at price is totally different."
- **Timestamp:** [21:20]
- **Severity:** Medium — relevant if Kompete.ai pursues international manufacturing clients; less critical for US/EU B2B SaaS focus
- **Category:** Product
- **Summary:** Manasa warns that globally-built SaaS pricing tools often create friction when localized — taxes, pricing structures, and formulas differ by region. Hard-coded global configurations frustrate local teams and slow adoption. She specifically calls out the risk of changes in a global system affecting all markets simultaneously, which makes customers hesitant to adopt or configure the platform.
- **Connects to:** New

---

### Objection: India Market Not Ready to Adopt AI-Driven Pricing Tools
- **Quote:** "India mostly the market is not that exposed or they're not ready to adopt for the AI changes that they want to. But there is a great exposure I would say because there are so many customers that we can just catch hold of them."
- **Timestamp:** [02:44]
- **Severity:** Medium — signals that India should not be a near-term GTM priority for AI-led pricing intelligence
- **Category:** GTM
- **Summary:** While the India market is large in terms of addressable customers, the procurement and technology maturity to adopt AI-powered pricing tools is low. Legacy systems make integration difficult, and organizational change management is a barrier. Europe is called out as the most mature market for pricing technology adoption in manufacturing.
- **Connects to:** New

---

### Objection: B2B SaaS Pricing Intelligence Is Better Served, But Misfit With Her Domain
- **Quote:** "In india, let's take India as an example, you don't get competitor prices very easily. It's just like people to people, person to person... your first option seems more clearer and apt for this industry."
- **Timestamp:** [08:50]
- **Severity:** Low — actually confirms the B2B SaaS thesis is sound, but from an outsider perspective; she cannot validate use cases directly
- **Category:** Market Fit
- **Summary:** Manasa validates that the B2B SaaS use case — where competitor pricing tiers and features ARE publicly visible — makes more logical sense for a web-scraping competitive intelligence tool than manufacturing. This is indirect but useful validation of Kompete.ai's original target market. However, it also reveals she is not the right persona to co-design the product with.
- **Connects to:** New

---

## Pain Points Validated

### Pain: Manual Excel-Driven Pricing Workflows
- **Quote:** "Mostly they are doing in Excel. So it's a manual process which is very complex. Let's say 31st is revision day. Price revision has to happen and they have to work for continuously two, three days, just set an Excel."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Excel spreadsheets; significant manual labor around scheduled revision cycles (quarterly or biannually for most customers)

---

### Pain: Competitor Pricing Is Informal and Unreliable
- **Quote:** "You don't get competitor prices very easily. It's just like people to people, person to person. You'll hear some number and then you'll just assume it and then you'll price according to that."
- **Severity:** HIGH
- **Category:** Pricing Opacity
- **Currently solving with:** Informal person-to-person intelligence gathering; teams have dedicated staff to "catch hold of" competitor prices through networks. Data is then manually uploaded into Synchron as a static file.

---

### Pain: Resistance to Moving Off Excel to Modern Systems
- **Quote:** "Excel they are used to, they're working already. So we want them not to use Excel and come into the system, do everything in the system. That's the key here."
- **Severity:** HIGH
- **Category:** Manual Process
- **Currently solving with:** Synchron Price's implementation team spends significant effort on change management and migration from Excel to their platform. Upload functionality from Excel serves as a bridge.

---

### Pain: Pricing Decisions Are Made Without Full Simulation Visibility
- **Quote:** "They'll have a clear cut idea, okay what my simulation looks and they can have multiple scenarios... mostly the customers would choose cost plus pricing. Nobody wants to do variable pricing because it's actually risky sometimes."
- **Severity:** MEDIUM
- **Category:** No System of Record
- **Currently solving with:** Synchron Price's scenario simulation module; historically done in Excel with limited scenario modeling capacity

---

### Pain: Stale Competitor Data Embedded in Pricing Decisions
- **Quote:** "It's not dynamic, it's a static one. Whenever you change it will get changed."
- **Severity:** MEDIUM
- **Category:** Stale Data
- **Currently solving with:** Manual uploads to Synchron Price whenever pricing team gathers new competitor data through informal channels

---

### Pain: Complex Approval Hierarchies Slow Down Pricing Changes
- **Quote:** "You can't just randomly change a part price randomly... only if I'm increasing my price until 2 lakhs, I can do it myself... if it comes between 2 lakhs to 5 lakhs, then my approver comes into picture and if it is anything above that it will go to CEO."
- **Severity:** MEDIUM
- **Category:** Manual Process
- **Currently solving with:** Synchron Price's role-based approval workflows

---

## Product Feedback & Feature Requests

### Feedback: Prioritize User-Friendliness Over Feature Depth
- **Quote:** "It's good to get the feedback and make it a little user friendly. That's the key here I would say and make it less complex."
- **Type:** UX Suggestion
- **Priority signal:** Expressed as a general principle, not a specific must-have. "Nice to have" framing but repeated twice — moderate signal.

---

### Feedback: Customizability for Local Markets Without Breaking Global Config
- **Quote:** "Have a do where it's like basic example is taxes... So it's better to have a tool where it is a little not complex and very user friendly where you can make changes... don't hard code it for a particular customer. That's actually affecting when you're trying to grow."
- **Type:** Feature Request
- **Priority signal:** Strong. She frames hardcoding as a growth-killer for SaaS products — this is strategic product architecture advice, not a casual comment.

---

### Feedback: Feedback Modules Are Underutilized and Represent Opportunity
- **Quote:** "Feedback quotations, different modules are already included. Yeah but it's not, I mean it's not that much rapidly used and this is a good opportunity and path to explore."
- **Type:** Positioning Feedback
- **Priority signal:** Moderate. She identifies that even mature platforms like Synchron haven't fully cracked stakeholder feedback loops. Suggests a gap Kompete.ai could address.

---

### Feedback: Consulting Firms as a Viable Distribution Channel
- **Quote:** "Let's say Deloitte or something and they want to do all this pricing, they'll anyway outsource any other products. So it's a great option to do that way."
- **Type:** Positioning Feedback
- **Priority signal:** Strong endorsement — she validates the channel partner model for consultancy-led adoption without being prompted beyond a brief mention.

---

### Feedback: Scenario Simulation Is a Core Value Driver, Not a Nice-to-Have
- **Quote:** "If I increase my margin by 1%, what will be the answer?... they can have multiple scenarios... based on the simulation they can see."
- **Type:** Feature Request
- **Priority signal:** Strong. Simulation is described as central to daily workflows and stakeholder buy-in. Customers won't adopt pricing tools that lack this capability.

---

## Strategic Insights

### Insight: Manufacturing Is a Poor-Fit Vertical for Kompete.ai's Current Architecture
- **Quote:** "It's mostly internal information, so we'll get it done somewhere... It's not dynamic, it's a static one."
- **Implication for Kompete:** Kompete.ai's core engine (real-time web monitoring of pricing, features, reviews, hiring signals) has no applicable surface area in manufacturing, where competitor data lives offline. Pursuing manufacturing would require a fundamentally different product (manual data ingestion, internal data enrichment). B2B SaaS remains the right beachhead.

---

### Insight: Europe Is the Most Mature Market for Pricing Technology Adoption
- **Quote:** "Europe is far more on par where we see... They have a broader perspective on what they want to do and their systems are also great."
- **Implication for Kompete:** If Kompete.ai expands geographically, European B2B SaaS companies may be more receptive to sophisticated competitive intelligence tooling than US counterparts who are still "a little hesitant to change." This could inform a future EU GTM motion.

---

### Insight: Cost-Plus Pricing Conservatism Signals Broader Market Risk Aversion
- **Quote:** "Mostly the customers would choose cost plus pricing. Nobody wants to do variable pricing because it's actually risky sometimes. So they don't want to do a trial and error."
- **Implication for Kompete:** Pricing teams across industries tend to be risk-averse by nature. Kompete.ai's messaging should de-risk adoption — emphasize observation and monitoring (low commitment) over automated pricing recommendations, which may feel too high-stakes to buyers.

---

### Insight: Synchron Price's 3-5 Year Contract Model Reveals Incumbent Lock-In Dynamics
- **Quote:** "It's a five year contract types where three years or five years contract basis. So implementation takes around six months or one year depends."
- **Implication for Kompete:** Enterprise pricing platforms win on deep integration and lock-in, not agility. Kompete.ai's positioning at a fraction of the cost with faster time-to-value (vs. 6-12 month implementations) is a structural advantage if targeting mid-market B2B SaaS companies who can't afford Klue/Crayon-level enterprise cycles.

---

### Insight: Consultancy-Led Channel Partner Model Has Validation
- **Quote:** "I can now understand if I have to go to another company where let's say Deloitte or something and they want to do all this pricing, they'll anyway outsource any other products. So it's a great option to do that way."
- **Implication for Kompete:** A consulting firm channel (strategy boutiques, RevOps consultants, fractional CMOs/CSOs) could accelerate distribution — these firms advise multiple B2B SaaS clients simultaneously and have recurring intelligence needs. A partner/reseller tier could be a meaningful GTM lever.

---

### Insight: Persona Confusion Risk — Pricing Consultants vs. Competitive Intelligence Buyers Are Different Roles
- **Quote:** "I've worked majorly in consulting for past six years where I've worked on synchron price, it's a enterprise as pricing platform."
- **Implication for Kompete:** This interview was conducted with a pricing platform implementer/consultant, not a competitive intelligence practitioner or a B2B SaaS product/marketing leader. While the conversation yielded market texture, it should not be used to validate willingness-to-pay or feature priorities for Kompete.ai's core ICP. Future interviews should specifically target product marketers, sales enablement leaders, or competitive intelligence analysts at $5-200M ARR SaaS companies.

---

## Persona Signals

- **Buyer or User?** Neither in Kompete.ai's ICP. Manasa is a **pricing platform implementer** (consultant) for manufacturing clients — adjacent to Kompete.ai's universe but not a direct buyer or user. She could be a potential future **beta tester or channel referral** (she explicitly offered).
- **Willingness to pay:** Not directly assessed. Her familiarity with 3-5 year enterprise contracts at Synchron Price ($100K+ range implied) suggests she has encountered high-cost pricing infrastructure. No specific signal on willingness to pay for competitive intelligence tooling.
- **Decision process:** As a consultant, Manasa influences clients' tool selection but does not control budget. Decision authority sits with pricing team heads and CFOs/CEOs for large contract values.
- **Current tools mentioned:**
  - Synchron Price (enterprise pricing platform — primary tool)
  - SAP (ERP / base price source)
  - Excel (manual fallback and data bridge)
  - Power BI (analytics/insights, mentioned as comparable to Synchron's insights module)
  - Fireflies (mentioned by Aditya as an example of a B2B SaaS product with tiered pricing)

---

## Key Quotes (Top 5)

1. *"You don't get competitor prices very easily. It's just like people to people, person to person. You'll hear some number and then you'll just assume it and then you'll price according to that."* — Validates the pain of competitor pricing opacity, even if the context is manufacturing; the underlying frustration (guessing competitor prices) is universal across industries.

2. *"It's not dynamic, it's a static one. Whenever you change it will get changed."* — Reveals that even purpose-built enterprise pricing platforms treat competitor data as a manual, static upload — a clear capability gap that Kompete.ai's real-time monitoring directly addresses for B2B SaaS.

3. *"Mostly they are doing in Excel. So it's a manual process which is very complex. Let's say 31st is revision day. Price revision has to happen and they have to work for continuously two, three days."* — Vivid illustration of the manual process pain that drives pricing team exhaustion; resonates with the broader competitive intelligence workflow problem.

4. *"Don't hard code it for a particular customer. That's actually affecting when you're trying to grow. SaaS is not like you just do it today. One year it survives, two years it survives."* — Strategic product architecture warning applicable to Kompete.ai's own build decisions — avoid over-customization that creates technical debt and prevents scale.

5. *"Your first option seems more clearer and apt for this industry... I mean if I have to say, I mean if we are into a product and product is already there, which is implemented, then the second option wouldn't help much."* — Indirect but genuine validation that a market-monitoring/competitive intelligence tool (Option 1 in Aditya's framing) is more compelling than an internal pricing workflow tool for audiences with existing systems — supports Kompete.ai's positioning as the external intelligence layer.
