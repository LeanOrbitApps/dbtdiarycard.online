# dbtdiarycard.online

Marketing site for **DBT Diary Card: Skills Tracker** (Lean Orbit LLC), served by GitHub Pages at https://dbtdiarycard.online/.

- `index.html` is the free online DBT diary card: a self-contained page whose CSS and JS are inline, plus `site.css`.
- `printable-dbt-diary-card/` is the printable blank card page, with Letter and A4 PDFs. The PDFs and preview PNG are generated from `index.html`'s own print layout (Print blank card with default rows), so regenerate them if the default rows or print CSS change.
- `blog/` holds the guides. `blog/index.html` is the Guides hub (the header's Guides link). Each article lives at `blog/<slug>/index.html`, uses the `.article` styles from `site.css`, and has BlogPosting, BreadcrumbList and FAQPage schema. When you add one, add a card to `blog/index.html`, a sitemap entry, and links from related pages.
- `blog/dear-man-dbt/` also holds the DEAR MAN worksheet. `worksheet-source.html` (noindex) is the print source for `dear-man-worksheet-letter.pdf`, `dear-man-worksheet-a4.pdf` and `dear-man-worksheet.png`; regenerate them with headless Chromium (Playwright `page.pdf`, Letter and A4, backgrounds on) if the wording changes.
- `site.css` is a copy of `leanorbit.app/dbtdailydiary/site.css`, the shared look of the DBT pages.
- `app-store-badge.svg` (black) and `app-store-badge-white.svg` (white, for dark-green sections) are Apple's official US "Download on the App Store" badges. Use them unmodified for every App Store link, at least 40px tall.
- `CNAME` tells GitHub Pages which domain to serve. Don't delete it.

## Adding a page

1. Create `some-page.html`, or `some-topic/index.html` for a clean URL. Copy the `<head>`, header and footer from `index.html`, link `site.css` (or `/site.css` from a subfolder), and set the page's own `<title>`, meta description, canonical and `og:url`.
2. Add the URL to `sitemap.xml`.
3. Link to it from at least one existing page. Pages nothing links to are slow to get indexed.

Keep App Store links pointing to `https://apps.apple.com/app/id6759234731`.

## Visitors' data

The diary card stores entries in the browser's localStorage under the key `lo-dbt-diary-card-v1`. That storage belongs to this domain. If the domain ever changes, visitors would lose their saved entries, so don't change it lightly.
