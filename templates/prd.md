# CLAUDE.md — PRD

> Claude will not begin writing until the problem statement and success metric are locked. Fill in every section first.

---

## Connected to

**Problem clarity audit**: [link or file — run this first if you have not]
**Post-launch review**: [leave blank now, fill in when you run the review after launch]

---

## The hypothesis

> "We believe [audience] cannot [do X] today because [reason]. Solving this will result in [outcome]. We know this because [evidence]."

**Evidence**: [data, customer quotes, support volume, lost deals, churn reasons — note what is solid vs. thin]
**What would prove this wrong**: [FILL IN]

---

## Customer

**Who this is for**: [specific enough that someone could find them and talk to them — not "enterprise users"]
**Their situation when this problem occurs**: [FILL IN]
**How acute the problem is**: [daily / weekly / occasional — and the cost when it occurs]

---

## Success metric

**How you will know in 90 days this was the right thing to build**: [specific behavioral change + business outcome]
**Leading indicator** (30 days): [FILL IN]
**Counter-metric** (what you are watching to make sure you are not breaking something else): [FILL IN]

---

## Scope: what is in

[Core behaviors the solution must enable. Stay at the "what," not the "how." If you find yourself describing implementation, pull back.]

---

## Scope: what is out

[Explicitly named exclusions. Things people will ask for that this release will not do. This is the harder and more revealing question.]

---

## Open questions

[Decisions not yet made. Do not resolve them here — surface them so they get resolved deliberately, not by accident during build.]

---

## Constraints

[Technical, timeline, design, regulatory — real ones that engineering and design need to know upfront]

---

## Stakeholder context

**Who reviews this**: [FILL IN]
**What they will scrutinize**: [FILL IN]
**Decisions that require their sign-off**: [FILL IN]

---

## Output spec

**What I need**: [full PRD draft / problem statement only / scope definition / open questions list]
**Format**: [narrative / structured sections / one-pager]
**Audience**: [engineering / design / exec / cross-functional team]

---

## Working style

**Anti-patterns to avoid**: ["do not start writing until the problem statement and success metric are confirmed", "do not resolve open questions without flagging them", "ask what is out before asking what is in — that is usually the harder question"]

---

<!--
EXAMPLE:

Hypothesis: Operations managers at mid-market companies cannot demonstrate the ROI of their automation program to executive sponsors without manually compiling numbers from multiple sources. This causes them to underinvest in automation and makes the product vulnerable at renewal. We know this because 4/6 churn interviews cited difficulty showing leadership value, and CS spends ~40 hours/quarter manually building ROI reports for customers.

Customer: Operations managers at companies with 200–2000 employees who are accountable to a VP or C-suite sponsor for the ROI of their automation investment.

Success metric: 25% of active enterprise accounts generate a report in the first 30 days. CS time on manual ROI reports drops by 50% in Q3. NPS among enterprise accounts improves 5+ points in the following quarter.

In scope: One-click report generation from existing product data. Shareable PDF output. Basic customization (logo, date range).

Out of scope: Custom metrics, white-labeling, Salesforce integration, scheduling/automated sends, historical trend views.

Open questions: Do we need manager/executive access roles to share the report, or can the operations manager share a static PDF? Who owns the design of the report template?
-->
