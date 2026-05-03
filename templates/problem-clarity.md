# CLAUDE.md — Problem Clarity Audit

> Run this before starting a discovery brief, PRD, or prioritization. It tells you whether you understand the problem well enough to act, or whether you are about to build on assumptions you have not tested.

---

## The problem you think you are solving

**State it in one sentence in user language**: [not "improve the dashboard" — what the user cannot do today and why that matters]

**How long you have believed this is the problem**: [a week / a quarter / years]

**Where this belief came from originally**: [a customer call / a metric / an exec / your own experience using the product / other]

---

## Assumption map

List every belief that has to be true for your current understanding to be correct. Then rate each one.

| Assumption | Rating | Evidence |
|------------|--------|----------|
| [FILL IN] | confirmed / directional / assumed | [source] |
| [FILL IN] | confirmed / directional / assumed | [source] |
| [FILL IN] | confirmed / directional / assumed | [source] |
| [FILL IN] | confirmed / directional / assumed | [source] |

**Confirmed**: you have data from multiple independent sources
**Directional**: you have a few signals pointing this way but not conclusive
**Assumed**: you believe it but have no real evidence

---

## The load-bearing assumptions

Of everything in the table above, which assumptions, if wrong, would change your direction entirely?

**If this is wrong, we should not build what we are planning to build**:
- [FILL IN]
- [FILL IN]

**If this is wrong, we would build something different**:
- [FILL IN]

**If this is wrong, we would approach the same build differently**:
- [FILL IN]

---

## Where your understanding is thinnest

**The assumption you are least confident in but most dependent on**: [FILL IN]

**The last time you talked directly to a user who has this problem**: [date or "cannot remember"]

**Whether you have seen this problem in behavioral data, or only heard about it**: [data / qualitative only / neither]

**Who you have heard this from** — and whether they are representative:
- [Source 1]: [how representative — one customer / multiple independent customers / data across user base]
- [Source 2]: [FILL IN]

---

## The clarity decision

Based on the above, which situation are you in?

**Option A — Enough clarity to act**: Your load-bearing assumptions are confirmed or directional, and the cost of being wrong is recoverable. Move to the relevant work template.

**Option B — Act but with explicit bets**: You have directional evidence but some load-bearing assumptions are unconfirmed. You can proceed if you name the bets explicitly, set a tripwire (a result that would tell you the assumption was wrong), and commit to checking it at a defined date.

**Option C — Resolve before acting**: One or more load-bearing assumptions are pure assumptions and the cost of being wrong is high. Do not write a PRD or commit roadmap space until you have run at least one test of the riskiest assumption.

**Which option applies**: [A / B / C]

**If B — your explicit bets and tripwires**:
- Bet: [assumption you are proceeding on]
- Tripwire: [result that would tell you it is wrong]
- Check date: [FILL IN]

**If C — what you need to resolve first**:
- [the specific question that needs answering]
- [the cheapest way to answer it]
- [how long it will take]

---

## Output spec

**What I need**: [clarity audit summary / list of assumptions to test / recommendation on whether to proceed / questions for my next user interview]
**What I will do with this**: [decide whether to start a PRD / brief my team / plan a research sprint]

---

## Working style

**Anti-patterns to avoid**: ["do not tell me the problem is clear when the assumption map shows it is not", "do not generate research recommendations before identifying which assumption is most load-bearing", "push back if I am in Option C but trying to proceed as if I am in Option A"]

---

<!--
EXAMPLE:

Problem I think I'm solving: Enterprise operations managers cannot demonstrate the ROI of their automation program to executive sponsors without spending 2–3 hours manually compiling numbers.

Assumption map:
- Operations managers report to an exec who cares about ROI metrics | confirmed | 4/6 churn interviews, 3 CS notes
- The bottleneck is report generation, not understanding of the numbers | assumed | no evidence either way
- They would share an auto-generated report with an executive without verifying it | assumed | 1 design partner said yes
- CS time on ROI reports is a real cost | confirmed | CS team time-tracking shows ~40hrs/quarter
- Executives will trust a system-generated summary | assumed | never tested

Load-bearing assumptions that, if wrong, change direction entirely:
- "The bottleneck is report generation" — if wrong, we should solve the confidence/explanation problem first, not the generation problem
- "They would share without verifying" — if wrong, self-serve does not work and we need CS-assisted tooling instead

Clarity decision: Option C.
The two most load-bearing assumptions are both pure assumptions. Building a self-serve report generator on top of them risks shipping something that creates CS work instead of removing it. Need to run 3 interviews specifically probing the verification behavior before proceeding.
-->
