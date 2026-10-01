---
type: concept
title: "Vault Durability and Backup"
status: developing
created: 2026-10-01
updated: 2026-10-01
tags:
  - concept
  - obsidian
  - storage
sources:
  - "[[Dots Storage Options]]"
  - "[[Obsidian Docs - Backup]]"
  - "[[Obsidian Docs - How Obsidian Stores Data]]"
  - "[[Obsidian Docs - Plugin Security]]"
---

# Vault Durability and Backup

The dot's cloud computer keeps state between uses but promises no retention period, so the vault needs a durable home outside it and an independent backup.

- Obsidian stores notes as local Markdown and notices external edits, so agents can edit files directly. See [[Obsidian]].
- Sync is not a backup. Keep a separate, recoverable snapshot.
- Community plugins have broad access. This vault runs in Restricted mode with none.
- Git is the simplest durable home: a repository is versioned, reviewable and restorable. Obsidian Git can commit, pull and push on an interval; pause auto-commit while an agent operation is running.

Options are weighed in [[Vault Storage Options Compared]].

Sources: [[Dots Storage Options]], [[Obsidian Docs - Backup]], [[Obsidian Docs - How Obsidian Stores Data]], [[Obsidian Docs - Plugin Security]].
