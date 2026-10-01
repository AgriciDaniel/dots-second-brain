---
type: meta
title: "Vault Guide"
status: evergreen
created: 2026-10-01
updated: 2026-10-01
tags:
  - meta
  - guide
---

# Vault Guide

How this vault is organized and maintained.

## Layout

| Path | Purpose |
|---|---|
| `inbox/` | Drop new sources here to ingest. Never deleted automatically. |
| `.raw/` | Original captures, never edited after capture. Hashes in `.raw/.manifest.json`. |
| `wiki/hot.md` | [[hot\|Hot Cache]]: short recent context, under 500 words, never a transcript. |
| `wiki/index.md` | [[index\|Wiki Index]]: the catalog of every page. |
| `wiki/log.md` | [[log\|Wiki Log]]: completed operations, newest first. |
| `wiki/overview.md` | [[overview\|Vault Overview]]: what the vault is for. |
| `wiki/sources/` | One page per captured source, with hash and refresh date. |
| `wiki/concepts/` | Synthesized knowledge, each citing its sources. |
| `wiki/entities/` | Products, tools, people and projects. |
| `wiki/questions/` | Open and answered questions. |
| `wiki/comparisons/` | Side-by-side evaluations. |
| `wiki/canvases/` | Visual maps. |
| `wiki/meta/` | This guide and the dots research notes. |

## Note rules

- Frontmatter: `type`, `title`, `status`, `created`, `updated`, `tags` (block list). Optional `sources` with quoted wikilinks.
- Types: source, entity, concept, question, comparison, overview, meta.
- Status: seed, developing, evergreen, answered, provisional, contested, deprecated.
- Links: `[[Page]]` when the name is unique, otherwise the vault path. No links only to balance the graph.
- Callouts: `[!key-insight]`, `[!gap]`, `[!contradiction]`, `[!stale]`.
- Every claim in a concept links to a source page. No source, no claim. Missing evidence is stated as no data.
- No credentials, tokens, account details or conversation IDs, ever.

Evidence rules: [[Evidence and Status]]. Retrieval: [[Scoped Retrieval]].

## Workflows

Any agent working here follows `AGENTS.md`. The four routines:

- **Ingest:** a new file goes in `inbox/`. Copy it unchanged to `.raw/sources/`, record its SHA-256 in `.raw/.manifest.json`, write a source page, then update the affected concepts, the index, the log and the hot cache.
- **Query:** answer from the vault by [[Scoped Retrieval]], cite the pages used, and say there is no data when the vault has none.
- **Save:** keep a chosen answer, decision or session summary as a note, updating the index, log and hot cache in the same change.
- **Lint:** check for dead links, orphans, missing frontmatter and captures whose hash no longer matches.

## What stays manual

The vault never records transcripts or writes notes on its own. After meaningful work the agent offers to save the outcome, and you choose what is kept. For context at the start of a session, point your agent tool at `wiki/hot.md`.

## Working with a dot

Pass the vault path and read order in the task or saved-schedule prompt (see [[Can a dot load this vault automatically]]). The dot reads `AGENTS.md` for the same rules.
