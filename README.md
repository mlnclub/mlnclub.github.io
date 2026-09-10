# MLn Reading Club

The club's website: <https://mlnclub.github.io>

A weekly ML 'n related topics reading group in Pittsburgh, meeting at CASI.
The calendar is on Luma: <https://luma.com/mln>

## How it is built

Jekyll. `.github/workflows/deploy.yml` builds on every push to `main` and
publishes `_site` to the `gh-pages` branch, which is what Pages serves.

This site was split out of the personal site it used to live on as `/mln/`, so
it still carries that site's al-folio plumbing (`_includes/head.liquid`, the
`_sass` tree, `_plugins/`) — trimmed to what these pages actually render with.
The old `/mln/` and `/mln/week-N/` URLs redirect here.

- `_data/mln.yml` — the single source of truth. Every card on the landing page
  and every `/week-N/` page is rendered from it, and all copy is pulled
  verbatim from the matching Luma event. It also holds `seasons:`, the season
  recap reel, and `notice:` (the announcement band under the masthead, which
  hides itself once its `expires` date passes).
- `_pages/mln.html` — the landing page and its grid logic; one thin
  `_pages/mln_weekN.md` stub per week, each just front matter.
- `_layouts/mln_base.liquid` — the shell. `_layouts/mln.liquid` — a week page.
- `_includes/mln_*.liquid` — cards, season dividers, the recap reel, and all
  of the CSS.

Paper audio is not committed; it is served from a GitHub release.

## Local preview

```
bundle install
bundle exec jekyll serve
```
