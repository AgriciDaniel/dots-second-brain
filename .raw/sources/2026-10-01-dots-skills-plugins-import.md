# Dots skills, plugins and import

Verified date: 2026-10-01
Source publication dates: unknown
Method: official documentation reviewed; short original summary

A dot uses supported plugins installed and enabled for the account; local skills require a connected computer. No documented direct skill upload to a dot.
Plugin format: root plugin.json with $schema https://agent-plugins.org/schemas/1.0.0/plugin.schema.json, name, version, description; skills in skills/<name>/SKILL.md; MCP in root mcp.json. .codex-plugin/plugin.json remains a fallback. Marketplace paths: .agents/plugins/marketplace.json (repo or home). Personal publish: ChatGPT Plugins > Personal > menu > Publish.
Desktop app Settings > Import maps another agent tool's instruction files to AGENTS.md, skills, plugins, slash commands to skills, MCP config, hooks and project memories; review custom MCP auth and hooks after.
Codex reads AGENTS.md from git root to working directory (32 KiB cap). Repo skills are available in Codex cloud tasks; personal local skills are not synced there.
Unverified: whether a personal plugin is "supported" in a dot; whether files placed in ~/.agents/skills on the dot cloud computer load.

Source: https://learn.chatgpt.com/docs/dots/computers-and-apps
Source: https://developers.openai.com/plugins/build/plugins
Source: https://learn.chatgpt.com/docs/import
Source: https://learn.chatgpt.com/docs/build-skills
Source: https://learn.chatgpt.com/docs/agent-configuration/agents-md
Source: https://learn.chatgpt.com/docs/environments/cloud-environments
