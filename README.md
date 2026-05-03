# PM Claude Brief — Templates & Discipline for Product Managers

A GitHub repo of CLAUDE.md templates for product managers, organized by problem type. Drop the relevant template in your project folder, fill it in, and Claude has the context it needs to do useful work.

---

## The problem this solves

Claude is capable. The bottleneck is not the model — it is missing context. When a PM opens a new session without loading context, Claude defaults to generic advice. It does not know your product, your users, your constraints, or the decisions already made. The output looks professional and is largely useless.

The fix is simple: a CLAUDE.md file that loads context automatically. Claude Code reads it at session start. You never have to paste the same background paragraph twice.

---

## Why templates + a skill, not a plugin or Project

The plugin/Project route builds a dependency. You need a setup, a server, or a SaaS account. It is the right call if you are building a tool for a team of 50. It is overkill if you are one PM trying to develop a better habit.

Templates + a skill work at a different surface area:

- **Templates** are portable context. A CLAUDE.md is a markdown file. It lives in a folder, gets committed alongside your work, and can be shared as a Slack snippet or a Notion block. No tool required to read it.
- **The skill** encodes the meta-discipline. It teaches the brief-writing habit — how to populate the template, what questions to answer before prompting, what a good output spec looks like. That habit transfers even if you switch tools.
- **Low ceremony = high adoption.** A PM who will not install a plugin will copy a markdown file. The bar matters.

If you later want to build this into a team tool with a UI, a database, and a shared context library, the templates become the schema. You have not locked yourself into anything.

---

## Tech stack recommendation

You do not need new tools to use this repo.

| Tool | Purpose | Notes |
|------|---------|-------|
| **Claude Code** (CLI) | Primary interface | CLAUDE.md in your project folder loads automatically at session start |
| **GitHub** | Template library | Fork this repo, customize templates to your product/company, share the fork with your team |
| **Plain markdown** | Everything | Works in VS Code, Obsidian, Notion, GitHub, and everywhere else |
| **VS Code or Cursor** | Editing briefs + work | Edit your CLAUDE.md alongside deliverables in the same window |
| **Obsidian** (optional) | Personal context library | Accumulate notes about your product, users, and strategic context over time; pull relevant sections into CLAUDE.md when starting new work |

**What you do not need**: a plugin, a Project, an MCP server, a database, a SaaS tool, or automation. The discipline is the system.

If you are not using Claude Code and are using claude.ai instead: paste your CLAUDE.md contents as the first message in each session, prefixed with "Before we begin, here is the session context:"

---

## Template index

| Template | Use when |
|----------|---------|
| [`templates/discovery.md`](templates/discovery.md) | User research, problem framing, opportunity sizing, JTBD |
| [`templates/prioritization.md`](templates/prioritization.md) | Ranking features, backlog grooming, roadmap tradeoffs, RICE/ICE |
| [`templates/gtm.md`](templates/gtm.md) | Launch planning, positioning, pricing, channel strategy, enablement |
| [`templates/build-vs-buy.md`](templates/build-vs-buy.md) | Vendor evaluation, make-or-buy decisions, partnership analysis |
| [`templates/roadmap.md`](templates/roadmap.md) | Roadmap narrative, stakeholder alignment, planning cycles |

---

## How to use a template

1. Find the template for your problem type in `templates/`
2. Copy it to your working folder as `CLAUDE.md`
3. Fill in every section — delete nothing, leave no placeholder blank
4. Open Claude Code in that folder. Context loads automatically.
5. Start working, not explaining.

If you use Claude Code's `/pm-brief` skill (see `SKILL.md`), it will walk you through the fill-in interactively and flag gaps before work begins.

---

## Contributing

Add a template by opening a PR with:
- The template file in `templates/`
- A row in the table above
- At least one example of a filled-in brief (as a comment block at the bottom of the template)

---

## License

MIT. Copy, fork, modify, redistribute. No attribution required.
