# CLAUDE.md — Feature Validation

> Fill in every section. Claude will not tell you whether to build. It will identify the riskiest assumption and the cheapest way to test it before you commit.

---

## The idea

**What it does** (not why it is good): [one paragraph — describe the feature, not the pitch]

---

## The assumption underneath it

Every feature rests on a belief about customer behavior. State yours explicitly:

> "We believe [customer] will [do X] because [Y]."

**What would prove this wrong**: [the result that would tell you the assumption does not hold]

---

## Why you think this is worth building

Name the evidence — separate strong from weak:

- **Strong** (multiple independent sources, behavioral data): [FILL IN or "none yet"]
- **Directional** (a few interviews, one customer, logical inference): [FILL IN]
- **Weak** (gut feel, one request, someone important mentioned it): [FILL IN]

If most of your evidence is in the third column, state that explicitly. It affects what needs to happen before any build decision.

---

## Who you would build it for first

**Specific segment**: [if the answer is "everyone," that is the first problem to address]
**Why them first**: [what makes this segment the right place to validate]

---

## What you would have to believe for this to work

List the assumptions that need to be true — customer behavior, market conditions, technical feasibility, business model:

1. [FILL IN]
2. [FILL IN]
3. [FILL IN]

**The riskiest one**: [which of the above, if wrong, kills the feature entirely]

---

## The cheapest test of the riskiest assumption

**What you could do in a week to validate or invalidate it**: [not a prototype — the minimum thing that gives you a real answer]
**What result would confirm the assumption**: [FILL IN]
**What result would kill it**: [FILL IN]

---

## Opportunity cost

**What not building this costs you**: [customer impact, competitive exposure, lost revenue — be honest]
**What building this costs you**: [what you are not doing if you commit to this]

---

## How we will measure success if we build it

**Leading indicator** (30–60 days post-launch): [behavioral change that shows the assumption was right]
**Lagging indicator** (90–180 days): [business outcome]
**Learning threshold**: [what result tells you the feature is not working and what you do then]

---

## Output spec

**What I need**: [validation plan / assumption map / experiment design / go/no-go recommendation]
**Audience**: [just me / eng lead / CPO / stakeholder group]

---

## Working style

**Anti-patterns to avoid**: ["do not recommend building or not building — identify the riskiest assumption and cheapest test", "do not accept weak evidence as validation", "push back if the proposed test would not actually de-risk the key assumption"]

---

<!--
EXAMPLE:

The idea: An in-product ROI calculator that lets users input their automation stats and generates a shareable summary showing time and cost saved. Users click a button, fill in 3 fields, get a one-page PDF they can share with their manager.

The assumption: Operations managers will use a self-serve tool to quantify ROI rather than asking CS to help them build the case.

Riskiest assumption: They will trust their own numbers enough to share them upward without CS validation. If they don't trust the output, the tool sits unused.

Cheapest test: Mock the PDF output manually. Send it to 5 active users with a message saying "we're piloting this — here's what it would look like for your account, does this match reality?" If 3+ say yes and would share it, the self-serve assumption holds.

Opportunity cost of not building: CS spends ~2 hours per enterprise account per quarter building ROI summaries manually. At current scale that's ~40 hours/quarter of CS time. Building this frees that capacity.
-->
