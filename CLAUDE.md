# CLAUDE.md — MLn Reading Club site (serves from `main` via Actions)

Two rules before any workflow:

1. **This repo is PUBLIC.** Nothing sensitive in commits or history. Never
   `git add -A` blindly — stage explicit paths.
2. **No AI-invented copy.** Week titles, summaries and descriptions are pulled
   **verbatim from the Luma event** — read
   [content-rules](docs/claude/content-rules.md) before writing any user-facing text.

| File | When |
|---|---|
| [mln](docs/claude/mln.md) | the whole workflow: Luma sync, new weeks, paper audio, recap photos, seasons, the announcement band |
| [content-rules](docs/claude/content-rules.md) | any user-facing copy |

This site was split out of Chris's personal site (`czhs/czhs.github.io`) on
2026-09-10, where it lived at `/mln/`. Those URLs still redirect here, so
**`/` and `/week-N/` must not change** — see the permalink note in the mln doc.
Paper audio still serves from the `mln-audio` release on that older repo.
