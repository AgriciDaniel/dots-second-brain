---
type: comparison
title: "Vault Storage Options Compared"
status: developing
created: 2026-10-01
updated: 2026-10-01
tags:
  - comparison
  - storage
sources:
  - "[[Dots Storage Options]]"
  - "[[Obsidian Docs - Backup]]"
---

# Vault Storage Options Compared

Where can a dot's vault live durably? Snapshot as of 2026-10-01.

| Option | Durable | Versioned | Agent can write | Notes |
|---|---|---|---|---|
| Dot cloud computer | Not guaranteed | No | Yes | Working copy only; no documented retention period |
| ChatGPT Library | Yes | No | Upload | Automatic Library search; 100 GB stated for Pro |
| Google Drive sync | Yes | Drive history | Via sync | Requires a Google Workspace domain; personal Gmail is not supported |
| ChatGPT GitHub app | n/a | n/a | No | Live, read-only search; not a synced index |
| Git repository + Obsidian Git | Yes | Yes | Yes, with scoped access | Reviewable history; pause auto-commit during agent operations |

**Recommendation:** keep the vault in a Git repository as the source of truth, work on a copy on the cloud computer, and keep an independent backup. Pushing from the dot with scoped access is still an open test (see [[Open Dot Integration Tests]]).

Sources: [[Dots Storage Options]], [[Obsidian Docs - Backup]]. Background: [[Vault Durability and Backup]].
