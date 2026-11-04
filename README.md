# Navjot Singh — Portfolio

Live site: https://codernav01.github.io/

A static GitHub Pages portfolio presenting Navjot Singh's data analytics, business intelligence, research projects, experience, technical writing, and résumé.

## Main files

- `index.html` — portfolio content, SEO metadata, structured profile data, and Medium article display.
- `style.css` — responsive styling and accessibility refinements.
- `Navjot-Singh-Resume.pdf` — downloadable résumé used by the site's résumé links.
- `latest-medium.json` — latest non-featured Medium article displayed on the site.
- `.github/workflows/update-medium-latest.yml` — scheduled Medium RSS refresh (every six hours) and manual refresh.
- `sitemap.xml` and `robots.txt` — basic search-engine discovery files.

## Medium publishing

The workflow reads the public RSS feed at `https://medium.com/feed/@codecosmosbynav`, skips the two pinned featured articles, and updates `latest-medium.json` with the newest remaining story. If the feed is unavailable on the website, the card links to the Medium profile instead.

To run it manually: GitHub → Actions → Update latest Medium article → Run workflow.

## Deployment

GitHub Pages publishes the `main` branch from the repository root. Changes committed to `main` are deployed by GitHub Pages.
