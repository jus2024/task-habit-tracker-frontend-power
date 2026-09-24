# Task & Habit Tracker Frontend — Kiro Power

A [Kiro](https://kiro.dev) Power that packages project-specific context for the
**Task & Habit Tracker** app so a Kiro agent can load it on demand: the app's
layered architecture, domain rules, and accessible, responsive React + Tailwind
conventions, plus a `fetch` MCP server.

This Power was authored for the
[Kiro University Challenge](https://kiro.dev/2026/university/) and is shared here as
a standalone, public repository (Bonus Lesson 2: Package a Kiro power).

## Contents

```
.
├── plugin.json                  # Agent Plugins 1.0.0 manifest ($schema + name)
├── POWER.md                     # Power manifest/overview
├── mcp.json                     # bundled MCP servers (fetch)
└── steering/
    ├── architecture.md          # layered design and rules for changes
    ├── domain-rules.md          # task/tag/habit/streak/stats rules
    └── frontend-conventions.md  # component, form, a11y, and styling patterns
```

## Install

In the Kiro IDE: open the **Powers** panel → **Add Custom Power** → **From GitHub**
and enter this repository's URL, or **From Local Path** after cloning it.

```bash
git clone https://github.com/jus2024/task-habit-tracker-frontend-power.git
```

## Activating

Mention project keywords in chat (see `keywords` in `plugin.json`, e.g. "task habit
tracker", "habit streak", "tailwind") and Kiro loads this Power's context on demand.

## Requirements

- [uv / uvx](https://docs.astral.sh/uv/) on PATH (for the bundled `fetch` MCP server).

## License

[MIT](./LICENSE)
