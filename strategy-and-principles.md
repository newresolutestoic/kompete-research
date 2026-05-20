# Kompete — Strategy & Principles

> **Status:** v1 draft · 2026-05-18 · *the operating document.*
>
> **Purpose:** the single source of truth for what Kompete is, who it's for, why it'll win, and how we work. Every hire reads this before joining. Every design decision is tested against it. Every investor conversation references it.
>
> **What this replaces:** ad-hoc roadmap thinking, scattered design rules, implicit positioning. This is the trace-up artifact — if a decision doesn't fit here, the decision is wrong (or this doc is wrong; either way it gets resolved here).
>
> **Synthesis basis:** 13 product foundation books + 27 customer interviews + 5 issue trees. See `memory/product-foundations/` for the underlying reading.

---

## I. The Strategy Stack

Adapted from Melissa Perri's strategy deployment framework. Four layers. Each layer must connect logically to the next, or we're in the build trap.

### 1. Vision *(2029 — three years out)*

> **A sales rep wakes up on a Tuesday. Their first Slack notification isn't a meeting reminder — it's Kompete, telling them that overnight, CompetitorX dropped Enterprise pricing 20%, and three of their active deals are now at risk.** The message contains a single sentence they can say on their 10am call, a customer proof point that beats CompetitorX's argument, and an inline "✓ I used this" button. They tap it, hit the call, and save the deal.
>
> They never think about competitive intelligence. They just keep winning deals they would have lost.
>
> In 2029, this is true for 500+ B2B SaaS sales orgs. Kompete is the default deal-intelligence layer for mid-market revenue teams — the thing that runs in the background, watches the world, and delivers competitive advantage automatically.

### 2. Strategic Intent *(by 2029)*

- **Default deal-intelligence layer for $10–50M ARR B2B SaaS sales orgs.** 500+ paying customers.
- **Defensible moat:** Counter-Positioning against Klue/Crayon's dashboard model, plus a compounding aggregate-intel dataset no competitor's single-tenant architecture can match.
- **Outcome-aligned revenue model:** majority of revenue tied to measurable customer outcomes (deals saved, win-rate lift), not pure seat-based pricing.
- **Operating model:** product-led organization per Perri/Cagan — outcome-owning teams, weekly customer touchpoints, Product Kata cadence.

### 3. Year-1 Product Initiative *(by April 2027)*

> **Prove that Slack-native trigger-based competitive intelligence produces measurable win-rate improvement at 5 pilot customer teams within 6 months — and convert ≥3 of them into named, public, willing-to-reference customers.**

Year-1 success is not "shipped MVP." It's "5 pilots with measurable outcomes + 3 reference-able customers." Anything else is build-trap thinking.

### 4. Options & Tests *(this quarter)*

The next 90 days are pure discovery + concierge-seeded validation:

- **10 Mom-Test-compliant outreach calls** to target Sales VPs → recruit 5 pilot teams.
- **Clickable Slack-bot prototype** with hand-curated competitor intel → run in front of 5 Sales VPs; look for "when can I have this?"
- **WTP study** (Van Westendorp + commitment currency) → price the Pro tier on data, not on what feels right.
- **"Why won't Klue copy us?" one-pager** → pressure-test the Counter-Positioning thesis.
- **Whole-Product gap map** → identify which augmented-layer pieces (battlecard library, onboarding flow, success motion) must ship in MVP.

---

## II. The Beachhead — who Kompete is for

Adapted from Geoffrey Moore's D-Day strategy. **One narrow niche, defended absolutely, before any expansion.**

### Target customer (the precise definition)

| Dimension | Specification |
|---|---|
| **Company size** | $10–30M ARR, Series B or bootstrap-equivalent |
| **Sector** | B2B SaaS in competitive markets (martech-adjacent, fintech SaaS, HR tech, dev tools) |
| **Sales team** | 10–40 AEs, named-account programs |
| **Tech stack** | Slack + Salesforce or HubSpot |
| **Buying authority** | Sales VP (primary), supported by PMM (secondary) |
| **Compelling pain trigger** | Lost ≥$500K to a named competitor in the past 4 quarters |
| **Current state** | Considered Klue/Crayon → balked at price OR using ChatGPT + manual spreadsheets |

If a prospect doesn't fit *all* of these, they're not the beachhead — they're a distraction. We say no to good-looking customers who fall outside the niche.

### Whole product *(non-negotiables for pragmatist buyers)*

| Layer | Must include from day 1 |
|---|---|
| Core | The AI agent + Slack + CRM integration |
| Expected | SSO, basic analytics, English docs, simple admin |
| **Augmented** *(the gap)* | Battlecard starter library (top 20 SaaS competitors pre-curated), 5-day onboarding playbook, customer success contact, training videos, ROI dashboard |
| Potential | Public 12-month roadmap |

The Augmented layer is **as important as the core**. Visionaries fill gaps themselves; pragmatists won't. We build it now, not after launch.

---

## III. Positioning — the obvious-awesome statement

Adapted from April Dunford. The positioning is not a tagline; it's the *context* that makes our value obvious to the right buyer.

> **For** $10–30M B2B SaaS sales teams losing deals to named competitors,
> **who are tired of** Klue's dashboards their reps never log into, ChatGPT's hallucinated competitor research, and battlecards that go stale within a week,
> **Kompete is** an AI agent that monitors competitors continuously and delivers deal-specific intelligence directly into Slack and CRM at the moment a rep can act on it,
> **unlike** Klue (which requires logins your reps won't make), ChatGPT (which can't monitor or attach to live deals), or manual processes (which don't scale past one PMM),
> **so that** sales reps act on competitive context within 24 hours of a stage change, win rates against named competitors improve measurably, and PMMs spend 80% less time maintaining battlecards.
> **Why now:** dashboards are dying, AI agents are the new interface, and outcome-based pricing aligns vendor and buyer.

### Category posture

**Year 1–2:** Dominate a subsegment of the existing Competitive Intelligence category. *Don't* fight Klue for the broad CI shelf; out-execute them in our beachhead.

**Year 2+:** Begin planting language for a new category — *"Deal Intelligence"* — that frames us against revenue intelligence (Gong, Clari) rather than CI tools. Phase the category move; don't bet the company on it in year 1.

### Buyer reframe

Klue/Crayon sell to PMM. Kompete sells to Sales VP. Same product, different category, different price, different conversation. **Every customer interaction uses Sales-VP language**: "deals at risk," "your reps closing more deals," "win rate against [their #1 competitor]" — never "competitor monitoring" or "battlecards." The vocabulary *is* the positioning.

---

## IV. The Seven First Principles

These are the durable principles — designed to be tie-breakers when two reasonable options conflict, and rejection criteria when something feels off but we can't name why. **Post these where every team member can see them.**

### 1. The customer outcome is the win condition.

Not features shipped. Not dashboards lit up. Not press coverage. We measure success by whether our customers win more deals against named competitors. If they don't, nothing we shipped matters.

*This rules out:* feature-based roadmaps, output velocity metrics, launching things without outcome measurement.

### 2. If a user has to log in, we failed.

Every login is a friction signal that we got the form factor wrong. Our default surfaces are Slack, CRM, and email — places sales teams already live. New dashboards are an admission of defeat. The admin panel is for PMM configuration only; everyone else operates from where they already are.

*This rules out:* "the Kompete app," browser-tab dashboards, login-required UX for end-users, anything that treats the dashboard as the product.

### 3. Silence between triggers.

Alerts compete with attention. We earn each one. Default to silent; speak only when speaking changes the customer's next action. False positives destroy trust faster than missed positives — one bad alert per week destroys the loop.

*This rules out:* "engagement-driven" notifications, daily digests by default, batch-send alerts to multiple reps unconditionally, sending anything we wouldn't bet a customer relationship on.

### 4. Deliver the answer, not the data.

A rep mid-call doesn't need a 2-page battlecard. They need a sentence they can use. The complete answer ships inside the message; clicking out is a design failure. *Knowledge in the world, not in the head.*

*This rules out:* link-out heavy messages, "see more in dashboard" CTAs, message templates that require interpretation, any UX that puts cognitive load on a stressed sales rep.

### 5. Attribution is built in, not bolted on.

We measure what we move. Every alert tracks whether the rep acted, whether the deal advanced, whether the customer renewed. ROI is observable from day 1 — not retrofitted at renewal. This is also our switching-cost compounding mechanism: the longer a customer uses Kompete, the more attribution data they accumulate.

*This rules out:* "we'll add analytics later," guessing at ROI, claiming impact without measurement, untracked feature launches.

### 6. Every customer request becomes a problem before it becomes a backlog item.

Customer says "add feature X" → we ask "what problem does X solve?" → we test the problem, then design solutions, then ship. We are not order-takers. Stakeholder dictation is the build trap's #1 entry point.

*This rules out:* feature-request-driven roadmaps, "the customer asked for it so we built it" reasoning, prioritization by request volume.

### 7. Would we be embarrassed if the competitor saw exactly what we scraped about them?

Competitive intelligence must remain on the right side of the line — public information, respectful aggregation, no dark patterns. The published-online test: if a journalist wrote a story about exactly how Kompete works, would we be proud or hide it? If hide-it, don't ship it.

*This rules out:* private-data scraping, login-required scraping at scale, deceptive collection, opaque AI-output sourcing, anything that erodes the long-term credibility of the CI category.

---

## V. The Moat Thesis

Adapted from Hamilton Helmer's 7 Powers. Kompete is at the Origination stage; the two Powers available to us *now* are **Counter-Positioning** and **Cornered Resource**.

### Primary moat: Counter-Positioning against Klue/Crayon

Klue and Crayon are *dashboards*. Their entire business model is built around:
- Per-PMM-seat pricing
- PMM as primary buyer
- Dashboard UX as the product surface
- "Competitive Intelligence" as the analyst category they own

To match Kompete's autopilot model, they would have to:
1. Cannibalize per-seat pricing (autopilot doesn't have a PMM "seat" in the same way)
2. Disrupt their PMM-buyer relationship (autopilot's primary buyer is Sales VP)
3. Re-architect from dashboard-first to message-first
4. Retrain their sales force on a new value proposition and new buyer
5. Re-pitch their TAM and category to investors and analysts

**Each of these is rational for them to refuse.** Klue/Crayon will likely "add AI features" to their dashboards, but they will not truly counter-position themselves. This is textbook Counter-Positioning — the same pattern Vanguard exploited against active fund managers, Netflix against Blockbuster, AWS against IBM.

### Secondary moat: Cornered Resource via aggregate intel dataset

As Kompete grows, the multi-tenant intelligence layer accumulates aggregate competitive signal that no single customer (and no single-tenant competitor architecture) can match:
- Pricing changes detected within hours because we have eyes everywhere
- Win/loss patterns by competitor compiled across customer base
- Predictive signals from aggregate behavior

This must be **designed into v1 architecture**, not retrofitted. Single-tenant data architecture forfeits this moat permanently.

### Tertiary moats *(compounding from year 2+)*

- **Switching costs:** accumulated battlecards, attribution history, custom trigger configs, rep behavioral habit (per Hook Model).
- **Network economies:** cross-customer benchmarks ("Your win-rate vs CompetitorX is below the average of 47 other customers tracking them") create user value that grows with customer count.
- **Brand:** decades of effort; not a year-1–3 lever, but consistent voice now compounds later.

### What we explicitly do NOT claim as moat

"Better UX," "first-mover advantage," "founder insight," "lower price." None of these are Barriers competitors can't cross. Don't pretend they are.

---

## VI. Year-1 Outcome OKRs

Replacing feature-based MVP planning. Each KR is a customer outcome, not a shipped artifact.

### Objective: Prove the autopilot deal-intelligence thesis works for our beachhead.

| KR | Target by April 2027 |
|---|---|
| **KR1** — Pilot customers signed | 5 sales teams (5–20 AEs each), all in beachhead profile |
| **KR2** — Reference-able customers | ≥3 named, public, willing-to-reference within 6 months of go-live |
| **KR3** — Win-rate impact | ≥10pp average win-rate improvement vs named top-3 competitors across pilots |
| **KR4** — Rep adoption | ≥70% of pilot AEs actively engaging with Kompete within 30 days of rollout |
| **KR5** — Trigger precision | ≥80% of alerts marked relevant by receiving rep, within first 30 days |
| **KR6** — Commercial validation | ≥1 paid commitment ($) from non-pilot customer based on pilot references |
| **KR7** — PMM time-to-battlecard | Battlecard maintenance time reduced from baseline ≥80% at pilot customers |

We do not track shipped-feature counts. We do not track velocity. We do not track lines of code. If a metric tracks output, it does not appear here.

---

## VII. Operating Disciplines — what happens every week

The Monday-morning practices that prevent slow drift into feature-factory mode. These are sacred — not subject to "we're too busy this week."

| Discipline | Cadence | Source |
|---|---|---|
| **Weekly customer touchpoints** | ≥2 customer conversations per week, every week, recorded as snapshots | Torres |
| **Product Kata review** | Every Monday: Direction → Current → Next Target → Next Step | Perri |
| **OST update** | Weekly: prune dead branches, add learnings, re-prioritize | Torres |
| **Mom-Test discipline** | Every conversation ends with explicit commitment-currency advancement | Fitzpatrick |
| **Outcome language audit** | Weekly: every artifact (slack, email, doc) framed as outcome not feature | Cagan, Perri |
| **Trigger precision review** | Weekly: review all alerts shipped to pilots, score relevance, fix root causes | Eyal |
| **WTP-driven pricing** | Quarterly: re-test willingness-to-pay; no discounting without restructuring tier | Ramanujam |
| **Whole-product gap audit** | Monthly: what augmented-layer pieces are missing for the next pragmatist sale? | Moore |
| **Counter-Positioning watch** | Quarterly: has Klue/Crayon shifted? Is the moat still valid? | Helmer |
| **Ethics published-online test** | Every shipped feature: would we be embarrassed if a journalist wrote about exactly how this works? | Eyal, Cagan |

### Non-negotiables for the first hire(s)

Pre-committing before any role is posted (per EMPOWERED):

| Practice | Commitment |
|---|---|
| **Weekly 1:1s** | 30 min, sacred, never rescheduled, dev-focused not status |
| **30/90/365 coaching plan** | Written before role is posted |
| **PM job description** | Written in outcome-language ("Owns [outcome] for [segment]") — never "ships features" |
| **Eng-manager comp** | Tied to customer outcomes + engineering health (uptime, deploy frequency) — never to feature throughput |
| **Hire for character** | Veto trumps competence — would we want this person coaching others in 18 months? |

---

## VIII. The "We Don't Do This" List

The discipline of saying no. Each rejection is justified by a principle above.

| We don't | Because |
|---|---|
| Ship a dashboard as primary UX | Principle 2 ("If a user has to log in, we failed") |
| Send daily-by-default digest emails | Principle 3 ("Silence between triggers") |
| Send Slack messages with "click here for more" link-outs | Principle 4 ("Deliver the answer, not the data") |
| Discount to close deals | Lehrskov-Schmidt — chronic discounting destroys price perception |
| Hire engineers as cost center / outsourced | TRANSFORMED — engineering must be in customer calls |
| Price below "what we can charge" because it feels safer | Ramanujam — Minivation is the most common failure mode |
| Adopt SOC 2 / procurement-heavy enterprise motion before pilot proof | Beachhead discipline — visionary motion now, pragmatist motion later |
| Compete head-to-head with Klue on "CI dashboard features" | Obviously Awesome — fight on shelf-we-define, not theirs |
| Add a customer-requested feature without translating it to a problem | Principle 6 — we are not order-takers |
| Talk to investors in feature-roadmap language | Cagan — frame milestones as outcomes, not features |
| Scrape private/login-gated data at scale | Principle 7 — published-online test fails |

---

## IX. What Changes This Document

This is a living artifact, but **deliberately resistant to change**. Updates trigger:

| Trigger | What gets updated |
|---|---|
| New customer-interview insight | OST and Options & Tests (section I.4) |
| Pilot result | Year-1 OKRs (section VI) and Strategic Intent if material (section I.2) |
| Klue or Crayon strategic move | Moat Thesis (section V) |
| Material pricing learning | Beachhead profile + positioning (sections II, III) |
| Hiring expansion | Operating Disciplines (section VII) |

What **doesn't** change without deliberate review:
- The 7 First Principles (section IV). These should hold for years.
- The Vision (section I.1). Changes ~once a decade.
- The Counter-Positioning thesis (section V). Changes only if validated wrong.

---

## X. Where this fits

| Artifact | Role |
|---|---|
| **This document** | The operating doc — read by all, referenced everywhere |
| `task5-product-form-factor.md` | The product hypothesis — child of this doc |
| `mvp-demo-plan.md` | The execution plan — must be rewritten to outcome-language per Section VI |
| `ci-thesis-analysis.md` | The supporting evidence — feeds this doc's positioning |
| `objection-playbook.md` | The sales script — must align with positioning (Section III) |
| `memory/product-foundations/*` | The reading basis — 13 books that produced this doc |
| `interviews/` | The raw signal — Mom-Test audit pending |

---

*Sources: synthesis from Cagan trilogy (INSPIRED, EMPOWERED, TRANSFORMED), Hooked (Eyal), Design of Everyday Things (Norman), Predictably Irrational (Ariely), Cold Start Problem (Chen), The Mom Test (Fitzpatrick), Continuous Discovery Habits (Torres), Monetizing Innovation (Ramanujam & Tacke), The Pricing Roadmap (Lehrskov-Schmidt), Obviously Awesome (Dunford), Crossing the Chasm (Moore), 7 Powers (Helmer), Escaping the Build Trap (Perri). Full notes in `~/.claude/projects/-Users-main-Documents-Kompete/memory/product-foundations/`.*
