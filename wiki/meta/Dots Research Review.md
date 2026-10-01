---
type: meta
title: "Dots Research Review"
status: evergreen
created: 2026-10-01
updated: 2026-10-01
tags:
  - meta
  - dots
  - research
---

# Dots Research Review

The dots source pack (six summaries and the [[Dots Research Map]]) was supplied on 2026-10-01. Its "verified" dates are the pack author's statements, not independent certification. This review lists what was checked independently.

## Independent checks, 2026-10-01

1. **Supported:** new tasks receive selected instructions and context, not every conversation. Automatic loading was not demonstrated. [Tasks and memory](https://learn.chatgpt.com/docs/dots/tasks-and-memory)
2. **Supported, narrower:** the cloud computer can retain state between uses; no retention duration or recovery guarantee was found. [Computers and apps](https://learn.chatgpt.com/docs/dots/computers-and-apps)
3. **Supported:** installed and enabled plugins depend on connections, permissions and environment; local skills need a connected computer. Personal-plugin use in a dot is not established. [Computers and apps](https://learn.chatgpt.com/docs/dots/computers-and-apps)
4. **Boundary:** cloud orchestration does not run local, config or plugin shell hooks. Importing settings from another agent tool is not a tested dot autoload path. [Hooks](https://learn.chatgpt.com/docs/hooks) · [Import](https://learn.chatgpt.com/docs/import)
5. **Supported for Codex cloud tasks:** repository skills are available; personal local skills are not synced. [Cloud environments](https://learn.chatgpt.com/docs/environments/cloud-environments)
6. **Correction:** the AGENTS.md 32 KiB limit is a configurable default. [AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md)
7. **Correction:** Plugins > Personal > Publish is workspace publishing and needs workspace-admin status. [Plugin packaging](https://developers.openai.com/plugins/build/plugins)

## Not verified

Plan, model, region and channel eligibility; numeric allowances; press reports; Drive account suitability; Library limits; GitHub connector behavior; MCP transports. Recheck the primary source first.

## Edits for publication

Four captures (access and limits, safety controls, storage options, skills and plugins) were edited to remove account-specific details, third-party tool names and an unverified claim about a third-party repository. Their hashes in `.raw/.manifest.json` and the source ledger match the edited files.

Sources: [[Dots Access, Plans and Limits]], [[Dots Community Resources]], [[Dots Context and Saved Schedules]], [[Dots Safety Controls and Risks]], [[Dots Skills, Plugins and Import]], [[Dots Storage Options]].
