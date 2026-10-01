---
type: concept
title: "Dot Cloud Computer"
status: developing
created: 2026-10-01
updated: 2026-10-01
tags:
  - concept
  - dots
sources:
  - "[[OpenAI Docs - Dot Cloud Computer]]"
  - "[[OpenAI Docs - Dot Integrations and Controls]]"
  - "[[Dots Storage Options]]"
---

# Dot Cloud Computer

A dot works on its own cloud computer, with its own files, software and browser sessions, separate from your device. It can keep working while your device is off, and its state can persist between periods of use.

- **No retention promise.** The documentation does not guarantee how long files stay, so this vault keeps an independent copy (see [[Vault Durability and Backup]]).
- **Separate sign-ins.** Browser sessions on the cloud computer are not your local sessions; local sign-in does not transfer.
- **Local work needs a connected computer.** Tasks on your own machine need an authorized, online computer with the app open.
- **MCP is environment-specific.** Local or project MCP servers may not be reachable from the cloud; ChatGPT supports remote HTTPS or Secure MCP Tunnel, not local stdio servers. This vault needs no MCP bridge because it is plain Markdown.

Sources: [[OpenAI Docs - Dot Cloud Computer]], [[OpenAI Docs - Dot Integrations and Controls]], [[Dots Storage Options]].
