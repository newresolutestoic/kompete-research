# Interview Extract: Siddharth Jain

**Date:** 10th February, 2026
**Role/Company:** Former Technical PM / Partnerships Lead, SaaS Labs (JustCall product); briefly at Super AGI; currently between roles
**Background:** Siddharth is a Technical PM with 12+ years of experience across developer, operations, and product roles. At SaaS Labs he managed 70+ integrations and later led the partnerships channel for JustCall, a cloud telephony platform. He is currently looking for his next role.

---

## Objections & Challenges Raised

### Objection: Users Shouldn't Self-Select Their Competitors
- **Quote:** "I would rather want that AI should understand what kind of business domain I'm operating in. Right. And then figure out all different businesses that are operating in the same domain around the globe."
- **Timestamp:** [15:11]
- **Severity:** High — challenges the current onboarding UX assumption that users know and correctly name their competitors
- **Category:** Product
- **Summary:** Siddharth argues that asking users to manually add competitors is flawed by design. Users have blind spots and biases about who their real competitors are. He suggests the platform should take the user's business description as input and autonomously surface the competitive landscape. This reframes the core onboarding flow entirely.
- **Connects to:** New (unique framing), though it partially connects to the "wrong competitors being tracked" pain pattern

---

### Objection: Tracking Too Many Competitors Is Expensive and Unscalable
- **Quote:** "There's a cost associated with each of the competitor that we are kind of saying the data that we are fetching. Right. So for each competitors there are multiple say 700 pages at times for different companies."
- **Timestamp:** [18:12] *(raised by Aditya in response to Siddharth's feature suggestion, implicitly validated by Siddharth)*
- **Severity:** Medium — raised as an internal product/infrastructure constraint, acknowledged but not directly challenged
- **Category:** Product
- **Summary:** Auto-discovering the full competitive landscape raises a real infrastructure cost concern — each competitor requires calls to multiple data sources (G2, Gartner, website pages, LinkedIn, Reddit, etc.). The unit economics of comprehensive, auto-surfaced competitor tracking is not trivially solved. Siddharth's response was to suggest a tiered approach: surface a list first without full analysis, let users opt in to track specific ones.
- **Connects to:** New

---

### Objection: Buyer Persona Ambiguity — Business vs. Individual Teams
- **Quote:** "So what you are building for, you're building for a business or you're building for building. Building to build cater to individual team within a business."
- **Timestamp:** [39:42]
- **Severity:** High — strikes at GTM clarity and ICP definition
- **Category:** GTM
- **Summary:** Siddharth directly challenges whether Kompete.ai is a company-level product or a departmental tool. The distinction matters significantly for sales motion, pricing model, buyer identification, and feature prioritization. He observed that competitive intelligence needs vary significantly by team (marketing vs. product vs. partnerships), and a product trying to serve all of them simultaneously risks being unfocused in its value delivery and hard to sell.
- **Connects to:** Buyer persona confusion — similar to what would emerge across other interviews targeting different departments

---

### Objection: CI Tools May Get Deprioritized as Teams Mature
- **Quote:** "I used to focus on competitive analysis, but I quickly, I over the time I pivoted from looking at what competitors are doing towards what customers are asking."
- **Timestamp:** [05:26]
- **Severity:** Medium — not a direct objection to the product, but signals that experienced PMs may deprioritize competitor tracking in favor of customer research
- **Category:** Market Fit
- **Summary:** Siddharth describes a professional evolution where he moved away from competitor-tracking toward customer-driven development. While he acknowledges competitive intelligence has value, his personal framework shifted. This suggests a risk that mid-level PMs — a likely user persona — may not be the most receptive audience if they've already "graduated" from competitive analysis as a primary input.
- **Connects to:** New — important counter-signal for user persona targeting

---

### Objection: Pricing Opacity Limits the Depth of Pricing Intelligence
- **Quote:** "Is the pricing transparent on just call? No." *(Siddharth's single-word confirmation)*
- **Timestamp:** [32:24]
- **Severity:** Medium — validates a data collection challenge for the product
- **Category:** Product
- **Summary:** When Aditya asked whether JustCall's pricing was publicly listed, Siddharth confirmed it was not. This is a common pattern in B2B SaaS ("contact us" pricing), which limits Kompete.ai's ability to perform direct pricing benchmarking. The product will need to rely on review site mentions, user-reported pricing, or inference from feature tiers — none of which are fully reliable.
- **Connects to:** New — pricing opacity is a product data challenge

---

### Objection: Mild Skepticism About AI Reliability Without Platform Foundation
- **Quote:** "Honestly, I'm not very AI strong...AI also is as strong as your platform is...I would just say make it amendable into other products."
- **Timestamp:** [30:07–30:47]
- **Severity:** Low — a general caution rather than a pointed critique
- **Category:** Product
- **Summary:** Siddharth expresses that he is not deeply versed in AI and approaches the product from a platform/integrations lens. He suggests the product's value will depend on how well the underlying data infrastructure is built, and that the ability to integrate with other tools will be a signal of robustness. This is more of a positioning note than a hard objection.
- **Connects to:** New

---

## Pain Points Validated

### Pain: No Automated Notifications for Competitor Changes
- **Quote:** "Currently we don't have such a tool. So what you're working on is something that you need to do your research. You have to keep a track of all the changes that are happening in the market when the competitors. You have to constantly every time look at what others are doing versus your tool would be providing your. Your tool will give you a notification. So it makes their job easy basically."
- **Severity:** HIGH
- **Category:** Manual Process / Stale Data
- **Currently solving with:** Manual monitoring — team members periodically visiting competitor websites and pricing pages; no systematic process

---

### Pain: Tracking the Wrong Competitors (Competitive Blind Spots)
- **Quote:** "When I was in Just Call, I realized this as a mistake. We were looking at wrong competitors. Right. Where were at. And were, you know, comparing ourselves with the established players. Which are already very far into the game."
- **Severity:** HIGH
- **Category:** Manual Process / Other (Competitor Discovery Gap)
- **Currently solving with:** Not solved — they manually selected competitors based on brand awareness, which led to benchmarking against irrelevant market leaders instead of true-tier peers

---

### Pain: Competitive Intelligence Is Siloed and Unstructured Across Teams
- **Quote:** "Every day me, Ishan Mukunda...we used to kind of see on LinkedIn what computer doing...we would take that snapshot, post it on our say slack groups to marketing team, to product team. Like okay, let's analyze this."
- **Severity:** HIGH
- **Category:** No System of Record / Tool Fragmentation
- **Currently solving with:** Manual Slack posts and ad hoc screenshots shared across teams — no structured system for logging, dating, or synthesizing competitive observations

---

### Pain: Portfolio Size Forces Manual Triage — Most Competitors Go Unmonitored
- **Quote:** "I was managing 70 plus integrations in total...But ideally in most cases it's just the top three, top two or top three that you circle back, keep circling back...If I have 70 integrations, I cannot put my hundred like focus on or provide give focus to every each individual integration as such."
- **Severity:** HIGH
- **Category:** Manual Process / Information Overload
- **Currently solving with:** Prioritization by adoption/business impact — only the top 10–15 integrations monitored regularly, leaving long-tail competitors entirely unchecked

---

### Pain: Competitive Intelligence Is Narrow, Not Holistic
- **Quote:** "Not all of it. But speaking specifically about integrations. Yes. I was doing a lot of competitive analysis on that front."
- **Severity:** MEDIUM
- **Category:** Tool Fragmentation / Manual Process
- **Currently solving with:** Each team does their own CI in their own domain — product, marketing, integrations, partnerships each operate separately without a shared intelligence layer

---

### Pain: Website Messaging Changes Require Manual Discovery
- **Quote:** "In 2024...end of 24, beginning 25, you know, in that six months, eight months of time I had to completely change the. How were marketing integrations on the website. And that brought in a lot of, you know, new, fresh visitors, new signups, all of that."
- **Severity:** MEDIUM
- **Category:** Stale Data / Manual Process
- **Currently solving with:** Manual periodic review of competitor pages — no tracking of when or how competitor messaging shifts over time

---

## Product Feedback & Feature Requests

### Feedback: AI-Driven Competitor Discovery From Business Description
- **Quote:** "I would rather, you know, just add details. Like let's say Super AGI as an example. I would add details of what super AGI is, what we are trying to achieve, what is our goals and objectives...basis that and the. I would rather want that AI should understand what kind of business domain I'm operating in. Right. And then figure out all different businesses that are operating in the same domain around the globe."
- **Type:** Feature Request
- **Priority signal:** "Would pay for this" — described this as a core design philosophy change, not an add-on. He returned to this point multiple times and framed the current approach (user inputs competitors) as a likely mistake.

---

### Feedback: Tiered Competitor List Without Full Analysis (Low-Cost Discovery Layer)
- **Quote:** "Initially at like one first level you can share other competitors they should be looking at. Right...just list it out again, don't provide any analysis about it. So that won't cost you a lot."
- **Type:** Feature Request / UX Suggestion
- **Priority signal:** "Nice to have" but pragmatic — framed as a cost-conscious solution to the full auto-discovery challenge

---

### Feedback: Usage-Based Pricing With Low Base Subscription
- **Quote:** "Keep the subscription cost low. And usage price heavy. Okay, got it. That is where people won't, you know, they won't mind even if the cost comes out higher because they used it. Right. They can, they can't question you. That why you are charging me so much?"
- **Type:** Pricing Feedback
- **Priority signal:** Strong — based on direct experience with pricing-related churn at SaaS Labs. He spoke with conviction and cited concrete customer behavior patterns as evidence.

---

### Feedback: Partnership & Integration Competitive Landscape as a Module
- **Quote:** "If there was a tool like yours where after providing some details it can recommend me which integration, which tools I should look at to build integrations with."
- **Type:** Feature Request
- **Priority signal:** "Would pay for this" within his specific context — he described a real past gap (not knowing which integrations to prioritize) that this would have solved

---

### Feedback: Build for Founders First, Expand to Teams Later
- **Quote:** "I would say like target the founders of businesses, right? Especially startups, right. Because at the startup stages where founders are looking more rather than established businesses...once they get good like outcome from your product, they themselves will, you know, then you keep adding on more modules."
- **Type:** Positioning Feedback / GTM Suggestion
- **Priority signal:** Strong — he framed this as a strategic sequencing recommendation, not a casual aside. Aditya also confirmed this aligns with their current thinking.

---

### Feedback: Outcome-First Messaging Over Feature-First
- **Quote:** "In terms of your product, it's very important you show the outcome. Right. The marketing has to be done what you are going to provide rather than what you can do. Right. That is very important is what I've learned."
- **Type:** Positioning Feedback
- **Priority signal:** Strong — based on direct experience changing JustCall's integration marketing page, which he said drove measurable new signups. He applied the lesson directly to Kompete.ai.

---

### Feedback: Make the Product Embeddable / API-First
- **Quote:** "I would just say make it amendable into other products might."
- **Type:** Feature Request / UX Suggestion
- **Priority signal:** "Nice to have" — mentioned briefly without elaboration; stems from his integrations background

---

## Strategic Insights

### Insight: Competitive Intelligence Has a Clear Organizational Owner — The CEO's Office
- **Quote:** "There was a business team, we used to call them CEOs office. We used to, you know, work with PM CEO and others to come up with the pricing or benchmark the pricing."
- **Implication for Kompete:** The buyer is not the product team or marketing team independently — pricing and competitive benchmarking decisions at JustCall ran through the CEO's office. This validates founder/C-suite as the primary buyer persona, and suggests that departmental value props should be framed as roll-ups to the CEO's strategic decision-making, not standalone team tools.

---

### Insight: AI Has Reversed the Traditional Direction of Competitive Monitoring
- **Quote:** "Previously used to be the startups will look up to the market leader, right, as the North Star. Now it's happening in reverse also if you think about it, right."
- **Implication for Kompete:** The market timing argument for competitive intelligence is stronger than ever. Incumbents now need to watch emerging startups as potential disruptors (e.g., ChatGPT vs. Google Ads), not just the inverse. This opens the ICP to larger companies worried about AI-native upstarts, not only scrappy startups benchmarking against leaders.

---

### Insight: Experienced PMs Consciously Deprioritize CI in Favor of Customer Research
- **Quote:** "I used to focus on competitive analysis, but I quickly, I over the time I pivoted from looking at what competitors are doing towards what customers are asking."
- **Implication for Kompete:** There is a maturity segment of PMs who have philosophically moved away from competitive analysis. Kompete.ai's positioning should address this directly — framing CI not as a substitute for customer research but as a complementary signal layer that catches market shifts customer interviews alone cannot reveal (e.g., a competitor's stealth AI pivot flagged months before launch).

---

### Insight: Funded Companies Will Pay If Value Is Clearly Communicated
- **Quote:** "All the companies who have picked up funding, they not shy away if the pricing is good and within their budget. Right. If they really want to invest in something like this. They will be willing to pay if the messaging or marketing is strong."
- **Implication for Kompete:** The ICP of recently funded B2B SaaS companies ($5M–$50M raised) is a strong fit — they have budget, motivation to compete, and are more receptive to new tooling. Messaging clarity is the primary conversion lever, not price point.

---

### Insight: Users Only Track 2–3 Competitors Manually, Leaving a Dangerous Blind Spot
- **Quote:** "Ideally in most cases it's just the top three, top two or top three that you circle back, keep circling back...If I have 70 integrations, I cannot put my hundred like focus on or provide give focus to every each individual integration as such."
- **Implication for Kompete:** The manual CI process is structurally biased toward established, known competitors. This creates systematic blind spots for long-tail and emerging competitors — exactly where disruption comes from. Kompete's automation value prop should explicitly call out this gap: "You're watching the wrong 3 companies. We watch the full field."

---

### Insight: The Connecting-the-Dots Problem Is the Core Unsolved Pain
- **Quote:** "So it was zoom in, zoom out definitely. But that zoomed out view across these meetings is something that is probably not possibly humanly possible actually...We have to discuss the roadmap, we have to discuss the feature so that each flow you are discussing and in that just to remember, okay, hiring me and then it's my CS team came up with this insight and then I have to marry that..."
- **Implication for Kompete:** The highest-value pitch is not "we collect data" but "we connect the dots across departments that no human can reliably hold in their head simultaneously." This frames the Strategy Timeline and cross-signal intelligence as the true differentiator, not the data collection layer.

---

## Persona Signals

- **Buyer or User?** User — Siddharth was a mid-level technical PM. He did not control budget for tooling. Pricing decisions ran through the CEO's office at SaaS Labs. He is currently unemployed and has no active buying authority.
- **Willingness to pay:** Could not provide a specific number ("I'll have to do my own research to come up with some number for this"). Qualitatively suggested pricing should feel "neglectable" as a subscription with usage-based upside — reflecting the lens of someone who experienced customer churn from high subscription costs at SaaS Labs.
- **Decision process:** Did not describe a formal evaluation process — at SaaS Labs, new tooling decisions (especially for CI/pricing strategy) would have gone through the CEO's office. He would likely be an internal champion, not a final decision-maker. Would evaluate based on outcome clarity and integration ease.
- **Current tools mentioned:** G2, Gartner, LinkedIn, Reddit, Product Hunt, Salesforce, HubSpot, Zapier, Make, N8N, Claude (MCP), Plivo, Twilio, Slack (for internal CI sharing), JustCall (employer's product)

---

## Key Quotes (Top 5)

1. *"Currently we don't have such a tool. So what you're working on is something that you need to do your research. You have to keep a track of all the changes that are happening in the market...Your tool will give you a notification. So it makes their job easy basically."* — Direct validation of the core alert/monitoring use case; unprompted acknowledgment of the gap [57:13]

2. *"When I was in Just Call, I realized this as a mistake. We were looking at wrong competitors. Right. Where were at. And were, you know, comparing ourselves with the established players."* — Validates the AI-driven competitor discovery feature as a painkiller, not a vitamin [15:37]

3. *"Keep the subscription cost low. And usage price heavy...That is where people won't, you know, they won't mind even if the cost comes out higher because they used it."* — Concrete, experience-backed pricing model recommendation with churn data behind it [54:53]

4. *"That zoomed out view across these meetings is something that is probably not possibly humanly possible actually...there are so many details into each separate meeting."* — Articulates the core product thesis in the customer's own language; highly quotable for pitch and landing page [45:36]

5. *"I would say like target the founders of businesses, right? Especially startups...once they get good like outcome from your product, they themselves will...then you keep adding on more modules like for marketing team."* — Validates the founder-first GTM wedge and land-and-expand model simultaneously [41:42]
