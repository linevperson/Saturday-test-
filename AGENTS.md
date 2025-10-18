# Repository Guidelines

This repository captures lightweight Ukrainian-language documentation. Treat each file as a canonical source: keep updates focused, reversible, and easy to audit.

## Project Structure & Module Organization
- `README.md` — primary landing page; update it when high-level scope or usage changes.
- `new_page` — supplementary notes; keep it plain UTF-8 text and cross-reference from the README when appropriate.
- `.git/` — version-control metadata; never commit edits inside it.

## Build, Test, and Development Commands
No automated build or runtime pipeline exists; contributions are textual.
- `git status` — confirm the working tree is clean before starting review.
- `git diff` — self-review changes; ensure language remains consistent and typos are fixed.
- `less README.md` — spot-check rendering and spacing for Markdown sections.

## Coding Style & Naming Conventions
- Use Markdown headings in Title Case and keep paragraphs under ~80 characters per line for readability.
- Preserve existing Ukrainian phrasing; add English glosses only when essential.
- Prefer ASCII punctuation; reserve non-ASCII characters for Ukrainian text and examples.
- Commit new files with lowercase, hyphenated names (e.g., `release-notes.md`).

## Testing Guidelines
- Run `git diff --check` to catch trailing whitespace and merge-conflict markers.
- Proofread content aloud or with a spell-checker before committing.
- When adding large sections, preview locally with a Markdown viewer to verify headings render correctly.

## Commit & Pull Request Guidelines
- Follow the current history: concise, descriptive, present-tense messages (`Комміт до файлу 1`).
- Reference related issues in the body (e.g., `Refs #12`) and summarize scope plus any follow-up work.
- Attach before/after screenshots when formatting changes the Markdown layout.
- Ensure PRs mention review focus areas so teammates can validate language accuracy.

## Localization Notes
- Maintain Ukrainian as the primary language; flag any English-only sections for translation.
- Note terminology decisions inside the PR to keep translations consistent across files.
