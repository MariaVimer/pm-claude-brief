# PM Brief — Context-First AI Collaboration for Product Managers

## What this skill does

When you invoke `/pm-brief`, Claude walks you through loading structured context before any PM work begins. It enforces the discipline of "brief before prompt" — the habit that separates a PM who ships the right things from one who ships things efficiently for no good reason.

The skill works in two modes:
- **Start a session**: populate a CLAUDE.md from a template for your current problem type
- **Review a brief**: audit an existing CLAUDE.md and challenge it before work begins

---

## Why this exists

Most PMs use Claude the way they use Google — a quick question, a generic answer. The problem is not Claude's capability; it is missing context. Claude does not know your product, your market, your users, or what actually constitutes value in your specific situation. Without that context, every response is generic.

But there is a deeper problem than missing context. A PM can write a complete, well-structured brief for the wrong thing. A brief that loads context efficiently does not prevent you from building something nobody needs, building something because an executive requested it, or shipping something with no way to know afterward whether it worked.

This skill is designed to fix both problems. It forces context before prompting. It also challenges the premise of the work before any work begins.

---

## The brief-writing discipline

A brief is a decision document, not a work order. Before any task begins, it must be able to answer one question: **should we be doing this at all?**

Fill in every section below before starting a session. Claude will read the brief, and if the hypothesis is weak, the rationale is "because someone important asked for it," or the success criteria are missing, Claude will push back before proceeding.

---

### 1. The hypothesis

State your core assumption as a testable belief, not a conclusion.

> "We believe [audience] experiences [specific problem] when [situation]. We believe solving it will result in [outcome]. We know this because [evidence]."

This is the most important section. If you cannot write this sentence with real evidence, you are not ready to build. "Our CEO wants this" or "a customer requested it" is not a hypothesis — it is a source. Sources require validation.

**What Claude will do if this is weak**: stop and ask you to defend it before proceeding. One customer request, one executive opinion, or one gut feeling does not constitute a validated problem worth building for.

---

### 2. Market and competitive context

- What does the market look like for this problem? Is it a crowded space or a gap?
- How do users solve this today — with a competitor, a workaround, or nothing?
- What does "nothing" cost them? (If doing nothing is fine, building something is not justified.)
- Why now? What has changed — in the market, in user behavior, in your product's position — that makes this the right moment?

---

### 3. Audience

Describe the specific person who has this problem. Not a segment. A person.

- What is their role and context?
- What are they trying to accomplish when they hit this problem?
- How acute is the pain? Is this a daily friction or a once-a-quarter annoyance?
- How do you know? (Interview data, behavioral data, support volume, churn analysis — name the source.)

Generic audience definitions ("enterprise users," "SMBs," "operations teams") are not sufficient. If you cannot describe a real type of person with a real problem in their language, the brief is not ready.

---

### 4. The pain being solved

State the pain in user language, not product language.

- What specifically goes wrong, takes too long, or fails to happen?
- What is the consequence when this problem occurs — for the user personally, for their team, for their business?
- Is this a problem users are aware of, or one they have normalized?

"Users want a better dashboard" is not a pain. "Finance managers spend 3 hours every Monday manually pulling data from three systems to produce a report their VP reads for 5 minutes" is a pain.

---

### 5. Why we are the right ones to solve it

- Does this fit our product's existing motion, or does it require us to go somewhere new?
- What do we have — distribution, data, trust, integrations — that makes our solution better positioned than alternatives?
- What are we not building because we are building this? (The opportunity cost must be named.)

---

### 6. Prioritization rationale

- Why this, over everything else we could be doing?
- What framework or evidence drove the ranking — customer data, revenue analysis, strategic alignment, something else?
- If the answer is "our CEO / a big customer / the sales team asked for it" — stop. That is a source, not a reason. What does the evidence say about the size, frequency, and cost of this problem across your user base?

---

### 7. How we will measure success

Name the metrics before the work begins, not after.

- **Leading indicator**: what changes in user behavior within 30–60 days of shipping that would tell you the problem is being solved? (Not "number of users who clicked the feature." What behavior downstream of that click shows value?)
- **Lagging indicator**: what business outcome should move in 90–180 days if you were right?
- **Counter-metric**: what are you willing to accept might get worse if you optimize for this? Naming it shows you have thought about tradeoffs.
- **Learning threshold**: what result would tell you that you were wrong, and what would you do then?

If you cannot answer these before building, you will not be able to learn from what you ship.

---

### 8. Constraints and decisions already made

- Time, team, budget, technical limits — what cannot change?
- What has already been decided that Claude should treat as fixed?
- What is explicitly out of scope?

---

### 9. Output spec

- What specific artifact do you need from this session?
- Who is the audience for that artifact — their role, their level of detail tolerance, what they will do with it?
- What does done look like — format, length, tone?

---

## How Claude will challenge weak briefs

Claude will not proceed with a brief that has these failure patterns:

**Weak hypothesis**
> "We want to build X." → Not a hypothesis. What problem does X solve, for whom, based on what evidence?

**Authority-based rationale**
> "The CEO / a big customer / Sales asked for this." → A request is not a validated problem. Requests require interrogation: how many users have this problem, how acute is it, what does it cost them, have we seen it in data beyond anecdotes?

**Missing success criteria**
> "We'll know it worked when users adopt it." → Adoption of what? Toward what end? A feature can have 80% adoption and produce zero business value. Name the behavioral change and the downstream outcome you are trying to cause.

**Assumed audience**
> "Enterprise customers want this." → Which ones? In what context? How do you know it is a broad pattern and not a loud minority?

**Opportunity cost blind spot**
> Not naming what you are not building. Every roadmap decision is a tradeoff. If you cannot name what you are deprioritizing to do this, you have not made a real prioritization decision.

---

## How to use the skill

### Starting a new brief

```
/pm-brief start [problem-type]
```

Problem types: `discovery`, `prioritization`, `gtm`, `build-vs-buy`, `roadmap`

Claude will load the template, walk you through each section, and challenge any section where the reasoning is thin before proceeding to the actual work.

### Reviewing an existing brief

```
/pm-brief review
```

Claude will read your CLAUDE.md and surface:
- Hypothesis gaps (missing evidence, authority-based rationale)
- Audience or pain point vagueness
- Missing success metrics
- Unstated opportunity costs
- Output spec gaps

### Loading context at session start

Drop your CLAUDE.md in your project folder. Every Claude Code session in that folder loads it automatically.

If you are on claude.ai: paste the contents as your first message with the prefix "Before we begin, here is the session context:"

---

## Tech stack recommendation

You do not need new tools.

| Tool | Purpose | Why |
|------|---------|-----|
| **Claude Code** (CLI) | Primary interface | CLAUDE.md loads automatically per project folder; persistent filesystem context |
| **GitHub** | Template library | Version control, team sharing, fork-to-customize |
| **Plain markdown** | Everything | No lock-in, works in VS Code, Obsidian, Notion, GitHub |
| **VS Code or Cursor** | Editing briefs + work | Edit CLAUDE.md alongside deliverables in the same window |
| **Obsidian** (optional) | Personal context library | Accumulate product, user, and market notes over time; pull into briefs |

What you do not need: a plugin, a Project, a database, a SaaS tool, an MCP server, or automation. The discipline is the system. The files are the memory.

---

## Marketplace metadata

**Skill name**: `pm-brief`
**Category**: Productivity / Product Management
**Trigger phrases**: "start a brief", "load context", "pm brief", "help me write a CLAUDE.md", "set up context for", "/pm-brief"
**Author**: see repo README
**Repo**: see repo README
