# Charles Agyekum — Data Analyst Portfolio

Live: **https://charles-agyekum.github.io**

A static portfolio site. One landing page and six project pages, each ending on a
recommendation a manager can act on. Every headline figure is verified against source.

## What is here

| Project | Tool | One-line result |
|---|---|---|
| DataCo Late Delivery & OTIF (flagship) | Power BI | 54.8% of orders late; First Class 95% late vs Standard 38%; $2.14M profit at risk |
| Superstore Order Fulfilment | Power BI | £12.6M sales, 11.6% margin; Tables lose £64,083 at 29% discount |
| Vrinda Store 2022 Sales | Excel | 31,047 orders cleaned (7 QA issues caught); women drive 64% of revenue |
| HR Employee Attrition | Excel | Dynamic dashboard; attrition verified at 16.12% |
| Adidas US Sales | Excel | 9,648 rows; 3 of 6 retailers drive ~72% of ~$900M |
| SQL Practice | SQL | 31 questions: joins, subqueries, CASE |

## Files

- `index.html` — landing page (hero, approach, six selected projects, contact)
- `projects/*.html` — one page per project
- `assets/screenshots/*.png` — dashboard screenshots used on the pages
- `.nojekyll` — tells GitHub Pages to serve the HTML as-is (no Jekyll build)

## How it is built

Plain HTML and CSS, no build step. Fonts (Hanken Grotesk, JetBrains Mono) load from
Google Fonts. A small inline script drives the hero particle effect and the count-up
numbers; the page reads fine with JavaScript disabled.

## Updating the site

This repo is already created and connected to GitHub. To publish a change:

```bash
git add -A
git commit -m "Describe the change"
git push
```

GitHub Pages redeploys automatically within a minute or two. See `SETUP.md` for the
one-time setup details (account, Pages settings, personal access token).

## Method

Clean first and document it. Verify every headline figure against the source
before calling a piece done. Close on a recommendation, not a description.
