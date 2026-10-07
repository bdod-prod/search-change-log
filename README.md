# Search Change Log

A static editorial resource by Alex Rostovtsev for documenting a website edit, baseline search observations, repeat checks, uncertainty and next action without treating a before/after pattern as proof of causation.

## File structure

- `public/index.html` — complete guide, fictional Cedar Bookkeeping change record, vertical timeline, resources and author section.
- `public/worksheet.html` — blank printable change-log worksheet.
- `public/resources/worksheet.md` — downloadable Markdown worksheet with matching fields.
- `public/404.html` — noindex fallback page.
- `public/robots.txt` — allows crawling.
- `public/assets/styles.css` — local site, responsive and print styles.
- `public/assets/favicon.svg` — local favicon.

## Preview locally

```bash
python3 -m http.server 8000 --directory public
```

Open `http://localhost:8000/`. No JavaScript or build step is required.

## Editing

Edit the HTML and Markdown directly. The Cedar Bookkeeping example and timeline are explicitly fictional; keep that labelling if they are changed.

## Production configuration

Production base URL: `https://bdod-prod.github.io/search-change-log/`.

Canonical and Open Graph URLs use this base; the sitemap contains the guide and printable worksheet. Root-aware links keep the custom 404 styled at nested missing paths. `.github/workflows/pages.yml` uploads only `public/` to GitHub Pages when those files change on `main`; there is no application build step. This project is served below a path on the account's Pages host, so its local `robots.txt` does not control the host-root crawler policy.

## Rendered review — 7 October 2026

The guide and worksheet were reviewed in Chromium at desktop width, 390 px and 320 px. Links, download files, metadata, keyboard focus and absence of external runtime requests passed. The worksheet prints on two A4 pages; field labels now stay with their writing space. Print contrast and writing rules were refined. One method sentence was corrected so an answer without browsing can still be assessed, with search use recorded separately. Screen design and outbound links are unchanged. See the root `BUILD-REPORT.md` for evidence and launch status. The user selected GitHub Pages on the `bdod-prod` account.
