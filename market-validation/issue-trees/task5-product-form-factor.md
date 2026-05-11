# Issue Tree: What Should the Product Actually Feel Like?

**Root question:** How does an AI-native CI product defeat all 7 conversion barriers through its form factor?

---

## The Answer in One Line

**The product has no dashboard. It is an agent that does the work of a competitive analyst and delivers finished outputs into the tools teams already use.**

---

## The 7 Design Principles (one per barrier)

```
Barrier                         Design Principle
─────────────────────────────   ──────────────────────────────────────────
1. "Nice to have"            →  Price below DIY ($299-499/mo). Self-serve entry.
2. Can't attribute revenue   →  Track CI-assisted deals inside the product. ROI writes itself.
3. No urgency               →  Trigger-based delivery tied to active deals. Intelligence IS the urgency.
4. Buyer journey broken      →  Self-serve at $0-499/mo. Below manager approval. Expand when proven.
5. DIY is "good enough"      →  Do what ChatGPT can't: monitor, connect to deals, push, remember.
6. Behavioral change         →  Zero new tools. Intel arrives in Slack/email/CRM. Nothing to learn.
7. Wrong category            →  Position as "deal intelligence" not "competitive intelligence."
```

---

## Dimension 1: Push vs Pull

**Pattern: Nudge, don't notify. Three-tier severity.**

| Severity | Channel | CI Trigger Example | Timing |
|----------|---------|-------------------|--------|
| Critical | Slack DM / phone | Competitor undercuts pricing on YOUR active deal | Immediate |
| Warning | Slack channel | Competitor launches feature you lack | Same day |
| Info | Weekly digest email | Competitor blog post, job posting change | Weekly batch |

**Evidence:**
- PagerDuty achieves 98% noise reduction via intelligent grouping + severity tiers
- Gong fires Slack alerts for competitor mentions and deal risks — event-driven, not scheduled
- Momentum.io: auto-creates deal-specific Slack channels enriched with Gong insights — reps work deals FROM Slack

**Design rule:** Between triggers, the product is SILENT. This defeats alert fatigue.

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## Dimension 2: Agent vs Dashboard (Autopilot vs Copilot)

**The Sequoia framework:**

| | Copilot (tool) | Autopilot (work) |
|---|---|---|
| What it sells | The tool | The work done |
| Who does the work | Human, assisted by AI | AI, supervised by human |
| Revenue model | Seat-based | Outcome-based |
| Moat | UI/UX | Data + workflow depth |
| CI example | Dashboard with AI summaries (Klue today) | Agent that monitors, writes battlecards, pushes to rep (the opportunity) |

**Key Sequoia quote:** "If you sell the tool, you're in a race against the model. If you sell the work, every model improvement makes your service faster and harder to compete with."

**Current CI tools = copilots evolving from dashboards.** The opportunity = leapfrog to autopilot.

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## Dimension 3: Embedded / Headless — No Primary UI

**The product should have NO primary interface the user visits.**

| Surface | Role | What it delivers |
|---------|------|-----------------|
| Slack/Teams | Primary delivery | Alerts, answers to competitive questions, deal coaching |
| CRM (Salesforce/HubSpot) | Embedded panel | Competitive context for active deals, auto-populated fields |
| Email | Digest + critical alerts | Weekly summary, time-sensitive pricing changes |
| Gong/Chorus | Real-time detection | Competitor mention → instant Slack follow-up with battlecard |
| MCP/API | Infrastructure | Feed CI into any AI tool the company uses |
| Admin panel | PMM only | Configure competitors, approve battlecard drafts, see usage |

**Evidence:**
- Salesforce Headless 360 (2026): "Slack becomes the surface, Salesforce becomes the brain. Humans barely log in."
- Crayon MCP Server: ZoomInfo integrated — reps get deal-specific CI instantly in Slack
- Clearbit: automatic CRM enrichment, no separate login ever

**Design rule:** If a sales rep ever has to "log in" to the CI tool, you've already failed.

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## Dimension 4: Trigger-Based Delivery

**Intelligence fires on events, not schedules.**

### Deal-Stage Triggers (from CRM)
- Competitor tagged on opportunity
- Deal stalls >X days against specific competitor
- Deal moves to negotiation (pricing comparison moment)

### Conversation Triggers (from Gong)
- Competitor mentioned by prospect
- Pricing objection raised
- "We're also looking at..." detected

### Market Triggers (from monitoring)
- Competitor pricing page changes
- Competitor launches feature/product
- Competitor raises funding / acquisition
- Competitor review sentiment shifts

### Internal Triggers
- Battlecard >45 days old (median staleness threshold per Crayon)
- Win rate drops against specific competitor
- New rep joins team (onboarding trigger)

**The ARISE GTM workflow (concrete example):**
1. Agent detects competitor pricing change
2. Identifies 3 affected active deals in CRM
3. Alerts those 3 AEs with specific talking points
4. Sends PMM a draft battlecard update for approval (5-minute task)
5. Approved update propagates to all sales tools immediately

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## Dimension 5: Zero Behavioral Change

**The "flow of work" principle: enter the user's workflow like a raft on a river.**

**Evidence that push-based delivery solves adoption:**
- Klue Compete Agent (push to Slack/Salesforce): **72% adoption** vs 34% median
- Klue Compete Agent results: **28% win rate increase, 12x ROI, 243 Deal Tips auto-sent**
- Standard battlecards (pull-based): only 26% adoption, 65% outdated

**The zero-change checklist:**

| Requirement | Why |
|------------|-----|
| Deliver in Slack/Teams/email | Where reps already live |
| Attach to deal workflows | Surface during deal progression, not as separate activity |
| Zero training | Agent messages must be self-explanatory |
| Auto-update | No manual maintenance by anyone |
| Contextual | Relevant to THIS deal, THIS competitor, RIGHT NOW |
| Answer, not data | "Say this, not that" — not "here's what changed" |

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## Dimension 6: The Competitive Landscape Is Converging Here

**AI CI Maturity Model:**

| Level | Name | Who's here |
|-------|------|-----------|
| 1 | Manual | Most $5-50M companies today |
| 2 | AI-Assisted | Companies using ChatGPT for ad-hoc CI |
| 3 | AI-Augmented | Klue/Crayon with AI features |
| 4 | AI-Orchestrated | Klue Compete Agent, ARISE GTM |
| 5 | AI-Native | **The opportunity — nobody's here yet at scale** |

**New entrants converging on the same vision:**
- **Steve (hiresteve.ai):** autonomous agent → monitor → synthesize → push battlecards → capture win/loss → feedback loop
- **Parano.ai (from EUR89/mo):** change detection, no dashboards, push summaries to Slack
- **RivalSense (from $45/mo):** affordable CI, 80+ sources, transparent pricing
- **ARISE GTM:** CI operating system for HubSpot, deploys in 2-4 weeks

**All converge on:** autonomous monitoring, AI synthesis, push delivery, deal-contextual, auto-updating, MCP/API-first.

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## Dimension 7: Pricing That Defeats "Nice to Have"

**The market is shifting:**
- 47% of SaaS companies exploring outcome-based pricing (2026)
- Seat-based dropped from 21% → 15%
- Bessemer: "Products with soft ROI struggle at renewal. Charge for outcomes."

**The template: Intercom Fin**
- $0.99 per resolution. 67% resolution rate. 80-90% savings vs human.
- You only pay when value is delivered.

**Recommended CI pricing architecture:**

| Tier | Price | What you get | Purpose |
|------|-------|-------------|---------|
| Free | $0 | 1-2 competitors, weekly email digest | Land. Get into the org. |
| Team | $299-499/mo | 5-10 competitors, Slack, auto battlecards, deal alerts | Below DIY cost. Below approval threshold. No-brainer. |
| Enterprise | Base + outcome component | Unlimited competitors, CRM, deal coaching, MCP/API. Plus per-competitive-deal-won pricing. | Align revenue with customer outcomes. Defeat ROI objection. |

**Why $299-499/mo works:**
- Below DIY cost (PMM time = $3-5K/mo equivalent)
- Below Klue/Crayon ($1.5-3.5K/mo)
- Below manager approval threshold at most companies
- Clear ROI: one saved deal/quarter pays for 2+ years

Source: [src-ai-native-product-form-factor](../sources/src-ai-native-product-form-factor.md)

---

## THE EXPERIENCE: Day in the Life

### Sales Rep
1. Opens Slack. Message from CI agent: "CompetitorX dropped Enterprise pricing 20%. You have 3 active deals against them. Here are updated talking points for each."
2. On a Gong call, prospect mentions CompetitorX. After call, gets Slack DM: "I heard CompetitorX on your Acme call. Their weakness is Y. Here's a customer proof point from a similar win."
3. Doesn't think about competitive intelligence. Just receives help winning deals.

### PMM
1. Gets Slack notification: "CompetitorX launched new feature. I've drafted an updated battlecard. Review and approve?" Clicks approve. 5 minutes.
2. Checks weekly dashboard: 47 competitive questions answered, 12 battlecards served, 3 deals coached. Win rate against CompetitorX: 58% (up from 42%).
3. Doesn't spend 15 hours/week on manual research.

### VP of Sales
1. Weekly digest: "CompetitorX dropped pricing (3 deals affected, all reps notified). CompetitorY hired 4 enterprise AEs in EMEA. Your win rate against CompetitorX improved 8% this quarter."
2. Makes strategic decisions. Doesn't ask "do we even use our CI tool?"

---

## HOW THIS MAPS BACK TO ALL 7 CONVERSION BARRIERS

| Barrier | How this product form defeats it |
|---------|--------------------------------|
| 1. Vitamin | $299-499/mo + outcome pricing. ROI self-evident from usage data. |
| 2. Attribution | Tracks CI-assisted deals, win rate by competitor, battlecard usage. Attribution built in. |
| 3. No urgency | Trigger-based alerts tied to active deals CREATE urgency. "Your deal is at risk." |
| 4. Buyer journey | Self-serve entry <$500/mo. PMM or AE starts without VP approval. Expand when value proven. |
| 5. DIY good enough | Monitors continuously, connects to CRM deals, pushes at right moment, maintains history. ChatGPT can't. |
| 6. Behavioral change | Zero. Intel arrives in Slack/email/CRM. Nothing new to learn or log into. |
| 7. Wrong category | Positioned as "deal intelligence" / "competitive revenue protection." Sold to Sales VP, not PMM. |

---

## THE META-INSIGHT

**Klue and Crayon built the right product for the wrong era.** They built dashboards with AI features — copilots for PMMs. The product that wins is an autopilot for revenue teams: no dashboard, no login, no behavioral change. An agent that does the work and delivers finished outputs where people already live.

**The product is not competitive intelligence. The product is competitive advantage, delivered automatically.**
