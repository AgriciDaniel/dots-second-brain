---
type: question
title: "Can a dot load this vault automatically"
status: answered
created: 2026-10-01
updated: 2026-10-01
tags:
  - question
  - dots
sources:
  - "[[OpenAI Docs - Dot Tasks and Memory]]"
  - "[[Dots Context and Saved Schedules]]"
---

# Can a dot load this vault automatically?

**No, not as documented on 2026-10-01.** A new task receives only the context the dot passes for that work. Automatic loading of a folder, `AGENTS.md` outside Codex environments, or a personal plugin in a dot is not documented.

**What works:** name the vault path and the read order (Hot Cache, then Wiki Index) inside each task and saved-schedule prompt, and keep a standing instruction in the dot's own notes. Explicit retrieval with a supplied path was tested and worked; automatic discovery was not.

Desktop agent tools that support session-start context can be pointed at [[hot|Hot Cache]]; see [[Vault Guide]].

Evidence: [[Dot Context and Memory]], [[OpenAI Docs - Dot Tasks and Memory]].
