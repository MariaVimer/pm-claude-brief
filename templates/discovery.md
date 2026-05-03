# CLAUDE.md — Discovery

> Fill in every section before starting a session. Claude will challenge weak hypotheses and thin reasoning before proceeding.

---

## Connected to

**Problem clarity audit**: [run this first if you are unsure how well you already understand the problem]
**PRD**: [link here once discovery informs a build decision]

---

## The hypothesis

State your core assumption as a testable belief, not a conclusion.

> "We believe [audience] experiences [specific problem] when [situation]. We believe understanding it better will enable us to [outcome]. We know this because [evidence]."

**Evidence behind this hypothesis**: [name the source — user interviews, churn data, support tickets, behavioral analytics, something else. "Our CEO thinks" is a source that requires validation, not evidence on its own.]

**What would prove this hypothesis wrong**: [FILL IN — if you can't answer this, the hypothesis is not testable]

---

## Market and competitive context

**How do users solve this problem today**: [specific workaround, competitor tool, or "nothing" — and what "nothing" costs them]
**Why we are investigating now**: [what changed — new data, new market signal, upcoming planning cycle, something else]
**Is this a problem users are aware of, or one they have normalized**: [FILL IN]

---

## Audience

Describe the specific person with this problem. Not a segment — a person.

**Role and context**: [what they do, at what kind of company, in what situation]
**What they are trying to accomplish when this problem occurs**: [FILL IN]
**How acute is the pain**: [daily friction / weekly blocker / occasional annoyance — and how do you know]
**Evidence this is a broad pattern, not a loud minority**: [number of users affected, frequency, support volume, churn correlation — something quantitative]

---

## The pain being solved

State the pain in user language, not product language.

**What specifically goes wrong or fails to happen**: [FILL IN]
**The consequence when it occurs**: [for the user personally, for their team, for their business]
**Current best workaround and why it falls short**: [FILL IN]

---

## Opportunity cost

**What are we not doing because we are doing this discovery**: [name it explicitly]
**Why this is worth the investigation time over those alternatives**: [FILL IN]

---

## Discovery scope

**The specific question we are trying to answer**: [not "understand users better" — the precise question that, if answered, enables a decision]
**What is out of scope**: [adjacent questions we are explicitly not answering now]
**Decisions already made that this discovery cannot change**: [FILL IN or "none"]

---

## How we will measure success

**What changes if this discovery goes well**: [what decision gets made, what bet gets validated or invalidated]
**Leading indicator**: [what would you see in the data or in user behavior within 30 days of acting on these findings that tells you the insight was real]
**Learning threshold**: [what result would tell you the hypothesis was wrong, and what would you do then]

---

## Constraints

**Timeline**: [when does this need to inform a decision]
**Research resources available**: [interviews, surveys, behavioral data, support logs — what you have access to]
**Known data gaps**: [what you cannot know from available sources]

---

## Output spec

**What I need from this session**: [specific artifact — research plan, interview guide, synthesis of existing data, problem statement, opportunity sizing approach]
**Format**: [narrative / structured sections / other]
**Audience**: [who reads this and what they will do with it]
**Length**: [FILL IN]

---

## Working style

**How I want Claude to respond**: [recommendation first / options with tradeoffs / challenge my framing first]
**Anti-patterns to avoid**: [e.g., "do not accept my hypothesis without questioning it", "do not produce a generic research plan", "do not hedge the synthesis"]

---

<!--
EXAMPLE (filled-in brief):

Hypothesis: We believe enterprise operations managers experience significant friction when they need to share automation results with stakeholders outside the product, because the current export options (CSV, PDF) require manual reformatting before they are presentable. We believe solving this will reduce time-to-insight for their stakeholders and increase perceived value of the product among non-user buyers. We know this because 4 of our last 6 churn interviews mentioned "hard to show value to leadership" as a contributing factor, and our CS team logs show 23 tickets in the last quarter asking for "better reporting."

Evidence: 4/6 churn interviews + 23 CS tickets in Q3. Not conclusive, but enough to investigate.

What would prove it wrong: If interviews reveal that the actual blocker is stakeholder access to the product itself (they can't log in), not the export quality — in which case we have a permissions/sharing problem, not a reporting problem.

Audience: Operations managers at mid-market companies (200–2000 employees) who own cross-functional automation workflows and are accountable to a VP or C-suite sponsor who does not use the product directly.

Pain: They run automations that save hours of manual work, but the only way to demonstrate this to their budget owner is to manually pull numbers from the product, paste them into a slide, and present it. This happens monthly during business reviews. It takes 2–3 hours. If the numbers look wrong (formatting issues, missing context), it undermines trust in the automation itself.

What I need: A 5-question interview guide targeting operations managers, focused on the reporting and value-demonstration workflow, plus a synthesis framework for categorizing what I hear.
-->
