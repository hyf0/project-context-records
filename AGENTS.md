# AGENTS.md

**This file is the single source of truth for working in this repo.** `CLAUDE.md`
is a symlink to it — never edit `CLAUDE.md` directly; edit `AGENTS.md`, and the
change reaches every tool at once.

## What this repo is

This repo *is* the **Project Context Records (PCR)** methodology. The canonical
document is `README.md`.

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
