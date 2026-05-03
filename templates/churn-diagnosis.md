# CLAUDE.md — Churn Diagnosis

> Fill in every section. Claude will work from your specific data, not generate a generic list of churn causes.

---

## What you are seeing

**The metric**: [churn rate, cohort, timeframe, magnitude — specific numbers]
**When it started**: [when you first noticed, and what changed around that time — product, pricing, market, team]

---

## Who is churning

**Segment or pattern**: [plan type, company size, cohort, geography — whatever cuts you have run]
**What patterns you have found**: [FILL IN]
**What you have not looked at yet**: [FILL IN]

---

## What churned customers said

**Exit survey data, cancellation reasons, CS notes, sales loss reasons**: [direct quotes where you have them]
**How much of your churned base gave a reason**: [coverage — 10% / 50% / most of them]

---

## Hypotheses

**Your current best guesses, ranked**: [state each as a testable belief with the evidence behind it]
**What you have already ruled out**: [hypotheses tested and eliminated — do not repeat that work]

---

## What data you have access to

[Product analytics, CRM, support tickets, billing system, customer interviews — what is available to work with in this session]

---

## How we will know when the diagnosis is right

**Leading indicator**: [what changes in the data within 30 days of acting on the diagnosis that tells you the cause was correctly identified]
**What a successful intervention looks like in 90 days**: [specific metric movement]
**What would tell you the diagnosis was wrong**: [FILL IN]

---

## Output spec

**What I need**: [diagnosis summary with ranked hypotheses / data analysis plan / interview guide / intervention recommendation]
**Audience**: [just me / CS team / VP / board]

---

## Working style

**Anti-patterns to avoid**: ["do not generate a generic list of churn causes — work from the data in this brief", "do not hedge every hypothesis equally — rank them by evidence strength", "identify where the evidence is thin and what one additional data point would most change the diagnosis"]

---

<!--
EXAMPLE:

What I'm seeing: Enterprise churn jumped from 8% to 14% in Q3. Affects accounts in the $30K–$80K ACV band specifically. No change in SMB churn.

When it started: First noticed in September. We changed our enterprise pricing in July (added a per-seat component).

Who is churning: Mid-market accounts, 100–500 employees, majority on the legacy flat-rate plan that got migrated to per-seat in August.

What they said: 4/7 exit surveys mention "cost increase." 2 mention "value doesn't justify the new pricing." 1 mentions a competitor.

Hypotheses (ranked):
1. Pricing change hit the 100–500 employee segment hardest because they have more seats but lower automation ROI per seat than enterprise accounts
2. The per-seat model made cost visible in a way that triggered procurement review that flat-rate didn't
3. Competitor timing is coincidental

What I need: A diagnosis of which hypothesis the data most supports, and what one interview or data pull would confirm or kill hypothesis #1.
-->
