# dbtdiarycard.online

Marketing site for **DBT Diary Card: Skills Tracker** (Lean Orbit LLC), served by GitHub Pages at https://dbtdiarycard.online/.

- `index.html` is the free online DBT diary card: a self-contained page whose CSS and JS are inline, plus `site.css`.
- `site.css` is a copy of `leanorbit.app/dbtdailydiary/site.css`, the shared look of the DBT pages.
- `CNAME` tells GitHub Pages which domain to serve. Don't delete it.

## Adding a page

1. Create `some-page.html`, or `some-topic/index.html` for a clean URL. Copy the `<head>`, header and footer from `index.html`, link `site.css` (or `/site.css` from a subfolder), and set the page's own `<title>`, meta description, canonical and `og:url`.
2. Add the URL to `sitemap.xml`.
3. Link to it from at least one existing page. Pages nothing links to are slow to get indexed.

Keep App Store links pointing to `https://apps.apple.com/app/id6759234731`.

## Visitors' data

The diary card stores entries in the browser's localStorage under the key `lo-dbt-diary-card-v1`. That storage belongs to this domain. If the domain ever changes, visitors would lose their saved entries, so don't change it lightly.
