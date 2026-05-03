# A way to build the right thing

Templates for PMs working with Claude. Before Claude helps you write a spec, rank a backlog, or plan a launch, it makes you answer whether you should be doing it at all.

---

## What this is

Five CLAUDE.md templates, one per common PM problem type. You copy the right one into your project folder, fill it in, and Claude loads it automatically when you start a session.

The templates ask harder questions than most briefs do: what is your hypothesis, what evidence do you have, who specifically has this problem, what does success look like in 90 days. If your answers are thin, Claude will say so before doing any work.

The goal is to stop building things on a hunch, because someone important asked, or because you can. And start building things because there is a real problem worth solving.

---

## Templates

| Template | Use when |
|----------|---------|
| [`templates/discovery.md`](templates/discovery.md) | User research, problem framing, opportunity sizing |
| [`templates/prioritization.md`](templates/prioritization.md) | Ranking features, backlog tradeoffs, roadmap decisions |
| [`templates/gtm.md`](templates/gtm.md) | Launch planning, positioning, pricing, enablement |
| [`templates/build-vs-buy.md`](templates/build-vs-buy.md) | Vendor evaluation, make-or-buy decisions |
| [`templates/roadmap.md`](templates/roadmap.md) | Roadmap narrative, stakeholder alignment, planning cycles |

---

## How to use one

1. Copy the template for your problem type into your working folder as `CLAUDE.md`
2. Fill in every section
3. Open Claude Code in that folder — it picks up the file automatically
4. Start working

---

## Tools you need

Claude Code, a text editor, and this repo. That is it.

| Tool | Why |
|------|-----|
| Claude Code (CLI) | Loads CLAUDE.md automatically at session start |
| VS Code or Cursor | Edit the brief and your work in the same window |
| Obsidian (optional) | Good place to keep running notes about your product and users that you pull from when filling in a brief |

---

## Contributing

Add a template by opening a PR with the file in `templates/`, a row in the table above, and at least one filled-in example in a comment block at the bottom of the template.

---

## License

MIT.
