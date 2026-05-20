# Kompete — Decision Log

> **What this is:** the "git log" of Kompete's strategic decisions. One row per durable decision. Each row links back to the chat entry where the decision was made and (if applicable) the artifact that codified it.
>
> **Why this exists:** when you ask in 2027 "why did we decide X?", this is the first place to look. The conversation context is in `chats/`; the decision lives here.
>
> **When to add a row:** a decision is durable if it would still matter in 6+ months *or* if reversing it would require redoing real work. Tactical choices (which library to use, what color the button is) don't belong here.

---

## Schema

| Field | Meaning |
|---|---|
| **#** | Sequential decision ID |
| **Date** | When decided |
| **Decision** | What we decided, in one sentence |
| **Why** | The reasoning (1–2 sentences) |
| **Chat** | Filename in `chats/` where the discussion happened |
| **Artifact** | Where the decision is codified (if anywhere) |
| **Tags** | For retrieval |
| **Status** | Active · Superseded · Reversed |

---

## Decisions

| # | Date | Decision | Why | Chat | Artifact | Tags | Status |
|---|------|----------|-----|------|----------|------|--------|
| 1 | 2026-05-18 | Adopt 7 durable first principles (customer-outcome-is-win, no-login, silence-between-triggers, deliver-answer-not-data, attribution-built-in, request→problem, published-online-ethics-test) | Distillation of 13 product foundation books; these are designed to hold across years as tie-breakers for every design and hiring decision | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §IV](strategy-and-principles.md) | `principles`, `product`, `foundations` | Active |
| 2 | 2026-05-18 | Year-1 success = 5 pilot customers + 3 named-public references + ≥10pp win-rate lift (not "MVP shipped") | Outcome-based OKRs replace feature-based MVP plan, per Cagan/Perri/Torres convergence | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §VI](strategy-and-principles.md) | `outcomes`, `product`, `gtm` | Active |
| 3 | 2026-05-18 | Primary moat = Counter-Positioning against Klue/Crayon's dashboard model; secondary moat = aggregate-intel data network effects | Klue/Crayon would have to cannibalize per-seat pricing + PMM-buyer relationship + dashboard UX to follow us — textbook Helmer Counter-Positioning. Needs pressure-test via "Why won't Klue copy us?" one-pager | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §V](strategy-and-principles.md) | `moat`, `counter-positioning`, `klue`, `7-powers` | Active |
| 4 | 2026-05-18 | Beachhead = $10–30M ARR Series B B2B SaaS sales orgs with 10–40 AEs, Slack + Salesforce/HubSpot, lost ≥$500K to a named competitor in last 4 quarters | Per Moore's D-Day discipline — narrow beachhead beats broad targeting; this profile is supported by the 27 interviews and matches the Counter-Positioning thesis | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §II](strategy-and-principles.md) | `beachhead`, `icp`, `chasm`, `gtm` | Active |
| 5 | 2026-05-18 | Category posture = dominate subsegment of CI in years 1–2; plant "Deal Intelligence" category-creation seeds for year 2+ (don't bet the company on category creation in Y1) | Per Dunford — category creation is high-reward, high-cost. We can't afford the market-education tax pre-Series A. Subsegment dominance first, then category move once we have references | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §III](strategy-and-principles.md) | `positioning`, `category`, `dunford` | Active |
| 6 | 2026-05-18 | Buyer reframe: sell to Sales VP (not PMM); position as "deal intelligence" (not "competitive intelligence") in customer conversations | Per Dunford — same product, different category, different buyer, different price. Sales-VP vocabulary ("deals at risk," "win rate") replaces PMM vocabulary ("battlecards," "monitoring") | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §III](strategy-and-principles.md) | `positioning`, `buyer`, `gtm` | Active |
| 7 | 2026-05-18 | Initial pricing tier hypothesis = $0 / $799 (decoy) / $1,499 (target) / Enterprise-outcome-based — pending WTP-conversation validation with 10 prospects | Per Ramanujam — current $299–499 is likely Minivation against Klue's $36K anchor. Run Van Westendorp + commitment-currency tests before committing | [2026-05-18-strategy-and-principles-doc](chats/2026-05-18-strategy-and-principles-doc.md) | [strategy-and-principles.md §I, related to upcoming WTP-study chat](strategy-and-principles.md) | `pricing`, `wtp`, `monetization`, `decoy` | Open — pending WTP study |
| 8 | 2026-05-19 | Context-tracking system = flat timestamped `chats/` + tag-based retrieval + single `decision-log.md` — no thread folders | User correction to initial proposal: folder categorization forces a primary axis that doesn't match overlapping reality of real conversations. Tags handle overlap; timestamps are the universal primary axis | [2026-05-19-operating-cortex-system](chats/2026-05-19-operating-cortex-system.md) | [chats/README.md](chats/README.md) · this file | `meta`, `memory-system`, `retrieval`, `ops` | Active |
| 9 | 2026-05-20 | Cortex extensions: chat-logger Haiku subagent + Stop-event soft-reminder hook (rate-limited hourly) + graph-builder Sonnet subagent producing derivable `graph.md`. Graph layer = derivable view on frontmatter, not separate infrastructure (defer real graph DB until 200+ chats) | Closes the Operating Cortex loop: rich frontmatter → agent maintains → hook prevents forgetting → graph-builder visualizes. Avoids GraphRAG / Neo4j over-engineering at our scale; frontmatter we have ports cleanly to a real graph DB later if needed | [2026-05-20-cortex-extensions-hook-and-graph](chats/2026-05-20-cortex-extensions-hook-and-graph.md) | `~/.claude/agents/chat-logger.md`, `~/.claude/agents/graph-builder.md`, `.claude/hooks/chat-logger-reminder.sh`, `.claude/settings.local.json`, `kompete-research/graph.md` | `meta`, `memory-system`, `agents`, `hooks`, `retrieval`, `ops` | Active |

---

## How rows get added

When a Claude session produces a durable decision, the chat entry references it as `decision-log #N` in its Decisions section, and a corresponding row gets appended to this file. The chat-source link in this table points back to the conversation where the reasoning lives.

---

*Schema version: v1, established 2026-05-19. Revise sparingly.*
