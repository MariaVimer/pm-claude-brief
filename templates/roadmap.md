# CLAUDE.md — Roadmap

> Fill in every section before starting a session. Claude will challenge roadmaps that are lists of requests rather than defensible strategic choices, and will flag items without validated hypotheses or success criteria.

---

## The hypothesis behind this roadmap

A roadmap is not a list of things to build. It is a statement of what you believe will create value, and why, and how you will know if you were right.

> "We believe that if we execute on [the 2–3 themes or bets in this roadmap], we will [specific business outcome] within [timeframe]. We know this because [evidence — research, data, customer insight, market analysis]."

**What this roadmap is optimizing for**: [the one metric or outcome that matters most this period — retention, revenue, activation, market expansion, something else]
**What it is explicitly not optimizing for**: [what you are trading off to focus here]

---

## Market and competitive context

**What is happening in the market that makes this roadmap the right response now**: [competitive shifts, customer behavior changes, new technology, regulatory pressure — something external that validates the direction]
**What competitors are doing**: [relevant recent moves that your roadmap should account for]
**Where the market is going that you are betting on**: [the forward-looking assumption your roadmap is built on]

---

## Audience

**Who this roadmap is primarily for** (the user you are building for, not the stakeholder reading the document): [specific persona with specific needs]
**What their most important unsolved problems are right now**: [not your backlog — their reality]
**How you know**: [research recency, data source, confidence level]
**Who is NOT the primary audience for this roadmap period, and why**: [naming this is how you hold the line against single-customer capture]

---

## The strategic bets

For each major theme or bet on the roadmap, state the hypothesis:

**Bet 1**: [theme or initiative]
- Hypothesis: We believe [outcome] because [evidence]
- Audience: [who benefits]
- Why now: [what makes this the right timing]

**Bet 2**: [theme or initiative]
- Hypothesis: [same format]

**Bet 3** (if applicable): [same format]

Any item that cannot be framed as a testable hypothesis — with evidence — should be challenged before it goes on the roadmap.

---

## The items

### Committed (decided, not up for debate this cycle)
| Item | Quarter | Why it is committed | Success metric |
|------|---------|-------------------|----------------|
| [item] | [Q] | [evidence or prior commitment] | [specific metric] |

### Under consideration (where input is needed)
| Item | Source | Evidence of problem at scale | Estimated impact | Priority hypothesis |
|------|--------|------------------------------|-----------------|-------------------|
| [item] | [who surfaced it + how many independent sources] | [data, not just request] | [FILL IN] | [FILL IN] |

**Source discipline for items under consideration**: For each item, state whether the evidence is:
- Validated: multiple independent sources, behavioral data, quantified impact
- Directional: a few interviews, one strong customer, logical inference
- Request without validation: one customer, one exec, one team — worth noting, not sufficient for roadmap commitment alone

### Explicitly deprioritized (important to document)
| Item | Why deprioritized | What it would take to reprioritize |
|------|------------------|----------------------------------|
| [item] | [evidence-based reason] | [FILL IN] |

Documenting deprioritizations is as important as documenting commitments. It is how you defend the roadmap when someone asks "why isn't X on here?"

---

## Opportunity cost

**What we are not doing because we are doing this**: [name the most significant deprioritizations]
**Why those tradeoffs are defensible**: [FILL IN — if you cannot explain this clearly, the prioritization is not done yet]
**Who will push back and what you will tell them**: [FILL IN]

---

## How we will measure success

For the roadmap as a whole:

**Leading indicators** (what changes in the first 60 days of execution that tells you the direction is right):
- [FILL IN]

**Lagging indicators** (what business outcomes move in 6 months if the bets are correct):
- [FILL IN]

**Counter-metrics** (what you are watching to ensure the roadmap is not creating new problems while solving old ones):
- [FILL IN]

**Learning threshold** (what would cause you to revise a bet mid-cycle, and what the process for that is):
- [FILL IN]

---

## Constraints

**Engineering capacity**: [teams, cycle length, known gaps]
**Design and research capacity**: [FILL IN]
**External commitments** (customer promises, contract obligations, event deadlines): [FILL IN or "none"]
**Dependencies on other teams or systems**: [FILL IN or "none"]
**Time horizon**: [period covered and how confidence degrades over time — e.g., "Q3 is committed, Q4 is directional, beyond that is aspirational"]

---

## Stakeholder context

**Who reviews or challenges this roadmap**: [FILL IN]
**Their primary lens** (revenue, technical health, customer satisfaction, strategic positioning): [FILL IN]
**Anticipated objections and how to address them**: [FILL IN]
**What you will not compromise on, and why**: [FILL IN]

---

## Output spec

**What I need**: [roadmap narrative / table / exec summary / customer-facing version / talking points / other]
**Format**: [prose / structured sections / slide outline / other]
**Audience for the output**: [team / VP / exec / customers / investors]
**Tone**: [internal / external-facing]
**Length**: [FILL IN]

---

## Working style

**How I want Claude to respond**: [draft first / challenge my bets first / structure then draft]
**Anti-patterns to avoid**: [e.g., "do not accept items without a validated hypothesis", "do not soften the deprioritization rationale", "do not produce a generic roadmap that could belong to any product"]

---

<!--
EXAMPLE:

Roadmap hypothesis: We believe that if we (a) close the enterprise compliance gap (SSO, audit logs) and (b) make cross-team collaboration native rather than bolted-on, we will reduce enterprise churn from 18% to under 12% in H2 and open the expansion motion from single-team to multi-team deployments. We know this because: compliance gaps appear in 60% of enterprise churn interviews; the top expansion blocker cited by CS is "can't get the second team on the same workspace without IT involvement."

Market context: Two competitors shipped SSO in Q1. We are now below the table-stakes line for enterprise. Multi-team collaboration is not yet solved by any competitor in our category — it is a 12-month window before it becomes a crowded feature.

Primary audience: Enterprise operations teams (the buyer) and the IT administrators who gatekeep their rollout.

Strategic bets:
1. Close compliance gap (SSO + audit logs): Validated — churn data + blocked pipeline. Q3.
2. Multi-team workspaces: Directional — CS qualitative data, no quantitative evidence yet. Q4.

Under consideration: AI automation assistant. Source: CPO preference + 1 design partner. Evidence: request without validation. Will not commit to roadmap until we have 5+ independent customer interviews confirming the problem it solves.

Success metrics:
- Leading (60 days): 10+ enterprise accounts enable SSO; 3 CS expansion conversations opened on workspace consolidation
- Lagging (6 months): Enterprise NRR improves 6+ points; average accounts-per-customer increases from 1.0 to 1.4
-->
