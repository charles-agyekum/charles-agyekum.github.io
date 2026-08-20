# Charles Agyekum: Risk & Finance Analytics

Live: **https://charles-agyekum.github.io**

Identity line: *Risk & finance analytics · Part-Qualified ACCA*.

A static portfolio site. One landing page and seven project pages, plus two pieces that
live in their own public repos, nine cards in all, each ending on a recommendation a
manager can act on. Every headline figure is verified against source.

**Rebuilt 30 July 2026** around the risk-and-finance identity: the Strategic Default
Pressure Index leads, and the tool-skills pieces sit behind it as method evidence.

## What is here

| Project | Tool | One-line result |
|---|---|---|
| **Strategic Default Pressure Index** (lead) | Python | Own-book commodity finance: default becomes rational at a **6.00%** premium, derived from the contract's own deduction structure. [Public repo](https://github.com/charles-agyekum/sdpi-advance-funding-risk) |
| DataCo Late Delivery & OTIF (BI centrepiece) | Power BI | 54.8% of orders late; First Class 95% late vs Standard 38%; $2.14M profit at risk |
| DataCo Late Delivery, rebuilt in pandas | Python | The same finding in code. [Notebook repo](https://github.com/charles-agyekum/dataco-late-delivery-pandas) |
| NHS Cancer Pathway: the 62-Day Standard | SQL / case study | Built on training data against a real cited NHS England benchmark; the honesty note is on the page |
| Superstore Order Fulfilment | Power BI | £12.6M sales, 11.6% margin; Tables lose £64,083 at 29% discount |
| Vrinda Store 2022 Sales | Excel | 31,047 orders cleaned (7 QA issues caught); women drive 64% of revenue |
| HR Employee Attrition | Excel | Dynamic dashboard; attrition verified at 16.12% |
| Adidas US Sales | Excel | 9,648 rows; 3 of 6 retailers drive ~72% of ~$900M |
| SQL Practice | SQL | 31 questions: joins, subqueries, CASE |

## Files

- `index.html`: landing page (hero, approach, nine project cards, contact)
- `projects/*.html`, one page per project
- `assets/screenshots/*.png`: dashboard screenshots used on the pages
- `.nojekyll` tells GitHub Pages to serve the HTML as-is (no Jekyll build)

## How it is built

Plain HTML and CSS, no build step. Fonts (Hanken Grotesk, JetBrains Mono) load from
Google Fonts. A small inline script drives the hero particle effect and the count-up
numbers; the page reads fine with JavaScript disabled.

**This site is the source of the brand, not a follower of it.** The Brand Design System
(`Thinking Memo\Gates\Brand Design System.md`) was extracted from these pages on 30 July
2026 and now binds every rendered artefact Charles ships: CV, cover letters, dashboards,
tools. When a token changes here, that gate is what the rest of the estate reads.

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
