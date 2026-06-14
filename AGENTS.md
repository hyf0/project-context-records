# AGENTS.md

**This file is the single source of truth for working in this repo.** `CLAUDE.md`
is a symlink to it — never edit `CLAUDE.md` directly; edit `AGENTS.md`, and the
change reaches every tool at once.

## What this repo is

This repo *is* the **Project Context Records (PCR)** methodology. The canonical
document is `README.md`.

## This repo dogfoods PCR

It uses its own methodology: design decisions live as records under
`.agents/docs/`, one topic per file, cross-linked with relative Markdown links.
The methodology itself is `README.md`.

When working here:
- **Read first.** If a record covers what you're touching, read it before acting.
- **Record as you go.** When a design decision is made here, write it down as a
  record — proactively, and whenever a human asks.
- **Keep it fresh.** If a change affects a record, update it in the same change.
- **Provenance.** An unstamped line is AI-accumulated: challenge and verify it
  freely. A `[VOUCHED @handle]` stamp (on a line, or at the top of a file) means a
  human vouched for it — treat it as settled; reopen or re-verify only on new
  evidence, a changed constraint, or a human's say-so. Add a stamp only on a
  human's explicit instruction; reading past a line, or not objecting, is not one.

## Translations must stay in sync

`README.md` (English) is the source of truth. `README.zh-CN.md` is a translation
of it and must track it **exactly**:

- **Any change to `README.md` must update `README.zh-CN.md` in the same change.**
  A translation that has drifted from the canonical English is worse than none —
  it silently misinforms the reader.
- When the two disagree, `README.md` wins; fix the translation to match it.
- Keep these **identical and untranslated** across both files: the coined terms
  (Project Context Records / PCR, Context Engineering, ADR, the provenance stamp),
  every URL, and the paste-in adoption block in the "How to use" section. Translate
  the surrounding prose, not the canonical snippet.
