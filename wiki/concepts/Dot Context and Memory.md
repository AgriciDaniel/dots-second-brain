---
type: concept
title: "Dot Context and Memory"
status: developing
created: 2026-10-01
updated: 2026-10-01
tags:
  - concept
  - dots
sources:
  - "[[Dots Context and Saved Schedules]]"
  - "[[OpenAI Docs - Dot Tasks and Memory]]"
---

# Dot Context and Memory

A dot starts with relevant ChatGPT memory and keeps its own notes about preferences, decisions and ongoing work. Those notes are separate from ChatGPT memory and are not a transcript.

> [!key-insight]
> Each new task receives only the instructions and context the dot passes for that work, not every earlier conversation. To use this vault, a task or schedule prompt must name the vault path and the read order. See [[Scoped Retrieval]].

## Saved schedules

A saved schedule states what to check or update, when (with time zone and optional end date), which changes deserve a notification and where results go. Event triggers work only where the connected service supports event monitoring. Pausing a dot does not cancel its schedules.

## For cloud coding work

Create the Codex cloud environment (repository and setup) before asking a dot for cloud coding tasks.

Sources: [[Dots Context and Saved Schedules]], [[OpenAI Docs - Dot Tasks and Memory]].
