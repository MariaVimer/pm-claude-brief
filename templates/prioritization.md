# CLAUDE.md — Prioritization

> Fill in every section before starting a session. Claude will challenge authority-based rationale and missing success criteria before proceeding.

---

## Connected to

**Problem clarity audit**: [link or file — run this first for any item you are not confident you understand]
**Post-launch review**: [leave blank now, fill in when you review the outcome of the top items]

---

## The hypothesis

For each item under serious consideration, state the belief driving it:

> "We believe building [item] will result in [specific outcome] for [audience], because [evidence]."

If the answer to "why are we considering this?" is "a customer asked for it" or "our sales team wants it" or "the CEO mentioned it" — that is a source, not a validated reason to build. State what evidence beyond a single request supports the priority.

---

## Market and competitive context

**What the market looks like for the top candidates**: [are these table-stakes features, differentiators, or nice-to-haves in the current landscape]
**What competitors have shipped recently that affects this ranking**: [FILL IN or "not applicable"]
**What users do today when these problems are unsolved**: [workarounds, competing tools, or nothing — and what that costs them]

---

## Audience

**Who are we primarily building for in this prioritization cycle**: [specific user type with a specific context — not "enterprise customers"]
**How do we know their priorities**: [research, interviews, behavioral data, support volume — name the source and recency]
**Who is NOT the primary audience for this cycle, even if they are loud**: [name them — this is how you defend against single-customer capture]

---

## The candidate list

| Item | Source | Evidence of problem at scale | Estimated impact | Estimated effort |
|------|--------|------------------------------|-----------------|-----------------|
| [item] | [who surfaced it] | [data, not anecdote] | [FILL IN] | [FILL IN] |

**Source discipline**: For each item, distinguish between:
- Validated problem (multiple independent sources, behavioral data, or quantified impact)
- Directional signal (a few interviews, one strong customer, logical inference from data)
- Request without validation (one customer, one exec, one sales rep — worth noting, not sufficient alone)

Items in the third category should not be ranked as if they are in the first.

---

## Prioritization criteria and weighting

**Framework**: [RICE / ICE / value vs. effort / MoSCoW / other — or "help me choose"]
**How to weight the criteria for this cycle**: [e.g., "retention impact matters more than reach because we are in a churn-reduction quarter, not a growth quarter"]
**What "high impact" means in our context right now**: [calibrate to your actual business situation, not generic definitions]

---

## Opportunity cost

**What are we explicitly not building if we commit to the top items**: [name the things being deprioritized]
**Why that tradeoff is defensible**: [FILL IN — if you cannot explain why the deprioritized items can wait, you have not made a real decision]
**Who will push back on the deprioritizations and what you will tell them**: [FILL IN]

---

## Constraints

**Engineering capacity**: [teams, cycle length, known gaps]
**Already committed items** (not up for debate): [FILL IN or "none"]
**Hard dependencies or sequencing requirements**: [FILL IN or "none"]
**External commitments that create deadline pressure**: [customer commitments, contract obligations, events — FILL IN or "none"]

---

## How we will measure success

For the top 2–3 items, state the success criteria before committing:

**Leading indicator** (what changes in user behavior within 30–60 days of shipping):
- [item 1]: [FILL IN]
- [item 2]: [FILL IN]

**Lagging indicator** (what business outcome moves in 90–180 days if we were right):
- [item 1]: [FILL IN]
- [item 2]: [FILL IN]

**Learning threshold** (what result would tell you the prioritization was wrong):
- [FILL IN]

If you cannot state these before building, you will not be able to evaluate whether the prioritization was correct.

---

## Output spec

**What I need**: [ranked list with scores / recommendation with rationale / defense document for stakeholders / other]
**Format**: [table / narrative / both]
**Audience**: [VP review / eng planning / customer QBR / just me]
**What happens after this output**: [what decision gets made with it]

---

## Working style

**How I want Claude to respond**: [recommendation first / show scoring then recommend / challenge my ranking before accepting it]
**Anti-patterns to avoid**: [e.g., "do not treat all sources as equally valid", "do not accept 'the CEO wants it' as sufficient rationale", "do not hedge the final recommendation"]

---

<!--
EXAMPLE:

Hypothesis: Building SSO will reduce churn among our $50K+ ACV accounts because 3 of our 5 most recent enterprise churns cited "IT security requirements" as a blocker to expanding usage beyond the initial team. This is also the #1 item on our enterprise ICP checklist that we currently cannot check.

Source discipline:
- SSO: Validated — 3 churn interviews + blocked in 12 active expansion conversations (per CRM data)
- Audit log export: Directional — mentioned in 2 interviews, 1 contract requirement from a F500 deal
- AI automation assistant: Request without validation — CPO wants it, 1 design partner interested, no behavioral evidence of the problem yet

Opportunity cost: Deprioritizing the mobile app (requested by 40 individual users in NPS survey) and the Salesforce integration (requested by Sales). Mobile app users represent <5% of revenue. Salesforce integration has no validated pipeline attached.

Success metrics for SSO:
- Leading: 3+ enterprise accounts enable SSO within 60 days of launch
- Lagging: Enterprise NRR improves by 5+ points in the quarter following launch
- Learning threshold: If fewer than 2 accounts enable it in 90 days, the problem was IT policy, not SSO specifically — revisit
-->
