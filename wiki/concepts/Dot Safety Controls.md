---
type: concept
title: "Dot Safety Controls"
status: developing
created: 2026-10-01
updated: 2026-10-01
tags:
  - concept
  - dots
  - safety
sources:
  - "[[Dots Safety Controls and Risks]]"
  - "[[OpenAI Docs - Dot Integrations and Controls]]"
---

# Dot Safety Controls

**Custom rules** (Settings > Personalization > Custom rules) have four modes: act without asking, act when told, ask before acting, and hand off. Rules cannot grant app access or remove required confirmations.

- **Auto-review** checks risky actions, with a documented circuit breaker after three consecutive denials. It is described as not a deterministic guarantee, and its documentation is from Codex; applicability to dots is not stated.
- **Data:** on personal plans the "Improve the model" setting governs dot data, and limited human review is possible even when it is off.
- **Disconnecting and deleting:** disconnecting an app does not delete context already built. Deleting a dot does not delete the files, threads or app changes it made.
- **Authorization:** a request to draft is not permission to send. Notes in this vault never authorize an action. Keep credentials out of the vault.

> [!contradiction]
> Press coverage at launch reported a self-replicating prompt injection found in red-teaming and early reviewers seeing a dot send email before review. These are press reports, not official documentation; treat them as risk signals.

Install dots tooling only from official OpenAI sources.

Sources: [[Dots Safety Controls and Risks]], [[OpenAI Docs - Dot Integrations and Controls]].
