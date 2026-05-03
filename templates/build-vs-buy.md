# CLAUDE.md — Build vs. Buy

> Fill in every section before starting a session. Claude will challenge authority-based rationale and evaluate whether the capability is worth acquiring at all before comparing options.

---

## The hypothesis

Before comparing build vs. buy, answer the prior question: should we acquire this capability at all?

> "We believe [audience] is materially blocked from [outcome] because we lack [capability]. This is costing us [specific consequence — lost deals, churn, delayed expansion, other]. We know this because [evidence]. Building or buying this capability will result in [specific outcome] within [timeframe]."

**Evidence**: [quantify where possible — number of deals blocked, churn attributed, customers unable to onboard, revenue impact if known]
**What would prove this wrong**: [what result would tell you the problem is smaller than you think, or that the capability alone is not the fix]

If the primary driver is "a customer asked for it" or "a competitor has it" — state that clearly and also state what evidence beyond that single datapoint supports the investment.

---

## Market and competitive context

**How users or customers handle the absence of this capability today**: [workaround, competing tool, blocking the deal, or deferring]
**What competitors have**: [who has this, what their implementation looks like, how important it is to the buying decision]
**Whether this is a table-stakes requirement or a differentiator**: [be honest — if everyone has it, it is a hygiene requirement, not a competitive advantage; that affects the build-vs-buy calculus]
**What happens if we do not acquire this capability**: [lose deals, lose customers, stay in a smaller market — quantify if possible]

---

## Audience and pain

**Who is blocked by the absence of this capability**: [specific persona with a specific workflow, not "enterprise customers"]
**How acute is the blocker**: [every deal blocked / sometimes a factor / nice-to-have that rarely kills deals — and how do you know]
**What they are doing today instead**: [specific workaround and what it costs them]

---

## Why we are evaluating now

**What triggered this decision**: [new customer demand, scaling problem, competitive pressure, strategic bet — name it]
**Why this and not something else**: [what makes this the right investment over the alternatives we are not doing]

---

## The options under consideration

### Build
- **What building would involve**: [scope, team, rough timeline, dependencies]
- **What we would own that we would not own with a vendor**: [data, customization, IP, integration depth]
- **The honest risk**: [where build estimates typically go wrong in your org]

### Buy / vendors
- **Vendors shortlisted**: [name them — do not leave this blank]
- **What we get that we could not build ourselves, or could not build as fast**: [FILL IN]
- **Lock-in risk**: [how hard is it to switch if the vendor raises prices, gets acquired, or stops supporting us]
- **Compliance requirements they must meet**: [SOC 2, GDPR, data residency, other]

### Partner / integrate
[FILL IN or delete if not applicable]

### Do nothing / defer
- **Is this a valid option**: [yes / no — if yes, under what conditions]
- **The cost of waiting**: [what gets worse for each quarter we do not have this capability]

---

## Evaluation criteria

**What matters most in this decision** (rank these):
1. [FILL IN — e.g., time to ship]
2. [FILL IN — e.g., total cost of ownership over 3 years]
3. [FILL IN — e.g., data security and compliance]
4. [FILL IN — e.g., customizability]
5. [FILL IN — e.g., vendor lock-in risk]

**Hard requirements** (disqualifies any option that cannot meet these):
- [FILL IN]
- [FILL IN]

---

## Opportunity cost

**What we are not doing because we are doing this**: [name the projects or investments being displaced]
**Engineering capacity trade-off** (if building): [what else would that team be working on instead]
**Why this is the right use of those resources over the alternatives**: [FILL IN]

---

## How we will measure success

**What does the right decision look like in 12 months**: [capability live, at what scale, with what quality bar]
**Leading indicator** (within 90 days of acquiring the capability): [what changes in deal velocity, customer behavior, or operational metrics]
**Lagging indicator** (6–12 months): [revenue impact, churn change, market expansion — FILL IN]
**Learning threshold**: [what would tell you in 6 months that you made the wrong call, and what you would do about it]

---

## Constraints

**Budget**: [envelope or "TBD — help me think through this"]
**Timeline**: [when does not having this capability start actively hurting us]
**Team capacity** (if building): [honest assessment of available bandwidth]
**Compliance or security requirements**: [FILL IN or "none beyond standard"]
**Vendor risk tolerance**: [can you take a dependency on a startup / do you need enterprise SLA guarantees]

---

## Decisions already made

[Anything settled — e.g., "we are AWS-only", "we have an existing vendor relationship with X", "the procurement threshold requires VP approval above $X"]

---

## Output spec

**What I need**: [structured comparison with recommendation / vendor evaluation matrix / one-page decision brief for CTO / questions to ask each vendor]
**Format**: [table / narrative / decision brief]
**Audience**: [FILL IN]

---

## Working style

**How I want Claude to respond**: [recommendation with rationale / options with tradeoffs / devil's advocate on my current preference]
**Anti-patterns to avoid**: [e.g., "do not produce a generic framework", "do not treat all criteria as equally weighted", "do not hedge — give me a recommendation even if it requires assumptions"]

---

<!--
EXAMPLE:

Hypothesis: We are losing ~20% of enterprise deals at the security review stage because we do not have SSO/SAML. CRM shows 12 active opportunities where IT has flagged this as a requirement in the last 6 months. 3 of our 5 most recent enterprise churns mentioned inability to expand usage due to IT security requirements. The combined pipeline value of the 12 blocked deals is approximately $800K ARR. Building or buying SSO will unlock the majority of these and remove a top-3 objection from our enterprise ICP checklist.

Competitive context: Every competitor in our category has SSO. This is a hygiene requirement, not a differentiator. That means we should optimize for speed and cost, not build as a capability moat.

Options:
- Build: ~6 weeks for one senior engineer, full SAML + SSO implementation. We own the integration depth. Risk: scope historically grows; compliance validation takes longer than expected.
- Buy: WorkOS or Auth0. WorkOS is purpose-built for B2B auth, ~$500/month at our scale. 2 weeks to integrate. Handles the compliance and multi-IdP complexity we would otherwise build ourselves.

Hard requirements: SOC 2 Type II compliant, EU data residency option, supports Okta, Azure AD, and Google Workspace.

Decision criteria (ranked): (1) time to unblock pipeline, (2) total cost under $1K/month, (3) compliance coverage, (4) effort, (5) lock-in risk.

Recommendation I am leaning toward: Buy (WorkOS). The capability is table-stakes, the build estimate will slip, and the vendor handles compliance complexity that would otherwise require significant ongoing maintenance.

What I need: A structured comparison confirming or challenging my lean, plus 4 questions I should ask WorkOS and Auth0 before committing.
-->
