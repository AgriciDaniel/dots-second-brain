---
type: concept
title: "Dot Skills and Plugins"
status: developing
created: 2026-10-01
updated: 2026-10-01
tags:
  - concept
  - dots
sources:
  - "[[Dots Skills, Plugins and Import]]"
  - "[[OpenAI Docs - Skills and Plugins]]"
  - "[[OpenAI Docs - Build Skills]]"
---

# Dot Skills and Plugins

A dot uses supported plugins that are installed and enabled for the account. Local skills need a connected computer. There is no documented way to upload a skill directly to a dot.

- **Skills** package reusable instructions and resources. **Plugins** can bundle skills and MCP tools. A `SKILL.md` file sitting in a folder is not proof that a runtime loaded it.
- **Plugin format:** a root `plugin.json` (name, version, description), skills in `skills/<name>/SKILL.md`, MCP in a root `mcp.json`. Marketplaces live at `.agents/plugins/marketplace.json`.
- **Import from other agent tools:** the desktop app (Settings > Import) maps another tool's instruction files to `AGENTS.md`, and also brings over skills, plugins, slash commands, MCP config, hooks and project memories. Review MCP auth and hooks afterwards.
- **AGENTS.md:** Codex reads it from the git root down to the working directory (32 KiB default, configurable). Repository skills are available in Codex cloud tasks; personal local skills are not synced there.

> [!gap]
> Unverified: whether a personal plugin counts as "supported" in a dot, and whether files in `~/.agents/skills` on the cloud computer load. Tracked in [[Open Dot Integration Tests]].

Sources: [[Dots Skills, Plugins and Import]], [[OpenAI Docs - Skills and Plugins]], [[OpenAI Docs - Build Skills]], [[OpenAI Docs - Dot Integrations and Controls]], [[Dots Community Resources]].
