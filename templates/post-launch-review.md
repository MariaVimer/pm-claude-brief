# CLAUDE.md — Post-Launch Review

> Connect this back to the brief you wrote before building. If you cannot find the original hypothesis and success metrics, that is the first problem to fix.

---

## Connected to

**Original brief**: [link or file name of the PRD, prioritization brief, or GTM brief this reviews]
**Hypothesis from that brief**: [paste it here — the exact "we believe X will result in Y because Z" statement]
**Success metrics you committed to**: [paste the leading and lagging indicators you defined before building]

---

## What actually happened

**Leading indicator** (what you said would change in 30–60 days):
- Predicted: [FILL IN]
- Actual: [FILL IN]
- Gap: [FILL IN]

**Lagging indicator** (what you said would move in 90–180 days):
- Predicted: [FILL IN]
- Actual: [FILL IN — or "too early to measure" with a date to revisit]
- Gap: [FILL IN]

**Counter-metric** (what you were watching to make sure you were not breaking something else):
- Predicted: [no worse than X]
- Actual: [FILL IN]

---

## Was the hypothesis right?

This is the only question that matters. Not "did it ship" and not "did people use it."

**Did the underlying problem get solved for the audience you targeted?** [yes / partially / no / too early to tell]

**Evidence**: [what data tells you this]

**If partially or no — why**: [was the hypothesis wrong, was the solution wrong, was the audience wrong, or was the execution wrong? These are different problems.]

---

## What you learned

**What you now believe that you did not believe before**: [specific — not "we learned users want simplicity"]

**What assumption turned out to be wrong**: [name it explicitly]

**What you would do differently**: [in the brief, in the build, in the launch — be specific]

---

## What this changes going forward

**Decisions this affects**: [what is now different in your backlog, roadmap, or strategy because of what you learned]

**Hypotheses this invalidates**: [any other bets on the roadmap that rested on the same assumption that turned out to be wrong]

**What you are now more confident about**: [FILL IN]

---

## Loose ends

**What is still unclear**: [questions this launch raised that you have not answered]
**What you would need to resolve them**: [research, data, time]
**Whether those questions are worth pursuing**: [yes / no / later]

---

## Output spec

**What I need**: [written review for my team / exec summary / personal notes / retro facilitation guide]
**Audience**: [just me / my team / leadership / cross-functional]
**What this output will be used for**: [quarterly review / roadmap update / team learning / other]

---

<!--
EXAMPLE:

Connected to: Q3 prioritization brief (July 2024) + ROI Calculator PRD

Original hypothesis: Operations managers will use a self-serve ROI calculator to generate shareable summaries for their executive sponsors, reducing CS involvement in renewal conversations and improving NPS among enterprise accounts.

Success metrics committed to:
- Leading: 25% of active enterprise accounts generate a report within 30 days
- Lagging: Enterprise NPS improves 5+ points in Q4; CS time on manual ROI reports drops 50%
- Counter-metric: No increase in support tickets related to report accuracy

What actually happened:
- Leading: 11% of accounts generated a report in 30 days (predicted 25%)
- Lagging: NPS improved 2 points (predicted 5+); CS time on ROI reports dropped 20% (predicted 50%)
- Counter-metric: 14 tickets about report accuracy in first 3 weeks (not predicted)

Was the hypothesis right? Partially.
The problem was real — customers do want to show ROI to their sponsors. But the self-serve assumption was wrong. Users generated one report, found numbers they could not explain, and called CS anyway. The tool created work rather than removing it because users did not trust output they could not verify.

What we learned: The bottleneck is not report generation — it is confidence in the numbers. Users need to understand how the calculation works before they will share it with an executive. A self-serve tool without an explanation layer does not solve the problem.

What this changes: The "AI-assisted report" item on Q4 roadmap rested on the same assumption (users will trust AI-generated summaries). That assumption is now flagged as high-risk until we solve the confidence problem first.
-->
