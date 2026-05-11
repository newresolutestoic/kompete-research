# Source: AI-Native CI Product Form Factor — Design Patterns & Evidence

## Metadata
- **URLs:**
  - Microsoft agent UX: https://microsoft.design/articles/ux-design-for-agents/
  - Sequoia services thesis: https://sequoiacap.com/article/services-the-new-software/
  - Vivun agentic AI UX: https://www.vivun.com/blog/ui-and-ux-for-agentic-ai-designing-ai-agents-that-work-as-true-teammates
  - Salesforce Headless 360: https://www.salesforce.com/news/stories/salesforce-headless-360-announcement/
  - Crayon MCP Server: https://www.crayon.co/blog/crayon-launches-first-competitive-intelligence-mcp-server
  - Klue Compete Agent: https://klue.com/compete-agent
  - Steve (hiresteve.ai): https://hiresteve.ai/
  - Parano.ai: https://parano.ai/
  - ARISE GTM: https://arisegtm.com/blog/agentic-competitive-intelligence
  - Bessemer AI pricing: https://www.bvp.com/atlas/the-ai-pricing-and-monetization-playbook
  - Intercom Fin: https://fin.ai/pricing
  - PagerDuty alert intelligence: https://support.pagerduty.com/main/docs/intelligent-alert-grouping
  - Momentum.io: https://www.momentum.io/notifications
  - Gong sales intelligence: https://www.gong.io/sales-intelligence-software
  - Designing for Analytics (flow of work): https://designingforanalytics.com/resources/episodes/182
  - Orbix generative UI: https://www.orbix.studio/blogs/ai-driven-ux-patterns-saas-2026
  - Unkover AI CI maturity: https://unkover.com/blog/ai-competitive-intelligence/
  - Monetizely pricing: https://www.getmonetizely.com/blogs/the-2026-guide-to-saas-ai-and-agentic-pricing-models
  - L.E.K. outcome pricing: https://www.lek.com/insights/tmt/us/ei/rise-outcome-based-pricing-saas-aligning-value-cost
- **Date accessed:** 2026-05-11
- **Type:** VC thesis pieces, product design frameworks, competitor analysis, pricing research

## Key findings by dimension

### Push vs Pull
- Microsoft: agents should "nudge, not notify" — contextual prompts at right moments
- Gong: proactive Slack alerts for churn, competitor mentions, stalled deals — event-driven, not scheduled
- Momentum.io: auto-creates Gong-enriched Slack channels per deal, reps move deals forward FROM Slack
- PagerDuty: 98% noise reduction via intelligent alert grouping, severity classification, deduplication

### Agent vs Dashboard
- Sequoia: "Copilots sell the tool. Autopilots sell the work. The work budget dwarfs the tool budget."
- Vivun: "The best design is invisible. Technology so powerful you barely notice it."
- Generative UI: dashboards created on-demand for specific questions, not static navigation

### Embedded / Headless
- Salesforce Headless 360 (2026): "Slack becomes the surface, Salesforce becomes the brain"
- Crayon MCP Server: CI as infrastructure for any AI tool. ZoomInfo integrated for instant Slack CI.
- Clearbit model: automatic CRM enrichment, no separate login
- Ivan Burazin: "Traditional software rebuilt with agent-first APIs. No UI. Entirely new business model."

### Trigger-based delivery
- ARISE GTM workflow: detect change → identify affected deals → alert AEs with talking points → draft battlecard update → 5-minute PMM approval → propagate
- Three-tier architecture: Critical (Slack DM, immediate), Warning (channel, same-day), Info (weekly digest)
- PagerDuty research: SOC teams get 4,484 alerts/day, 67% ignored. Severity tiers + dedup essential.

### Defeating behavioral change
- "Flow of work" principle: enter user's workflow like a raft on a river
- Klue Compete Agent: 72% adoption (vs 34% median) by pushing to Slack/Salesforce
- Klue: 28% win rate increase, 12x ROI, 243 Deal Tips auto-sent
- Battlecard failure: 65% outdated, only 43% include talk tracks, median staleness = 45 days

### Next-gen CI tools
- Steve: autonomous agent, monitor → synthesize → push battlecards → capture win/loss → feedback loop
- Parano.ai: from EUR89/mo, change detection, no dashboards to babysit
- RivalSense: from $45/mo, affordable CI for startups
- AI CI Maturity: Level 1 (manual) → 2 (assisted) → 3 (augmented) → 4 (orchestrated) → 5 (native)
- Market converging on: autonomous monitoring, AI synthesis, push delivery, deal-contextual, auto-updating, MCP/API-first

### Pricing
- 47% of SaaS companies exploring outcome-based pricing (2026)
- Seat-based dropped 21% → 15%. Hybrid surged 27% → 41%.
- Intercom Fin: $0.99/resolution, 67% resolution rate, 80-90% savings vs human agent
- Bessemer: "Products with soft ROI struggle at renewal. Charge for outcomes."
- Below DIY cost: $200-500/mo ($2,400-6K/yr) vs PMM time ($39-58K/yr) vs Klue ($20-40K/yr)

## Used in issue tree
- Task 5: All 7 dimensions of product form factor
