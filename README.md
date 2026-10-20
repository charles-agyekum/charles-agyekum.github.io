# Charles Agyekum: risk and finance analytics

Live site: https://charles-agyekum.github.io

A static portfolio with one landing page and seven project pages. It also links to two pieces that live in their own public repos, so there are nine project cards in all.

The Strategic Default Pressure Index comes first. It is built on my own cocoa credit book. The other pieces use public datasets and show the method in Excel, Power BI, SQL and Python.

## What is here

| Project | Tool | Result |
|---|---|---|
| Strategic Default Pressure Index (lead) | Python | On my own cocoa book, default pays above a 6.00% premium. [Public repo](https://github.com/charles-agyekum/sdpi-advance-funding-risk) |
| DataCo supply chain: late delivery & OTIF risk | Power BI | 54.8% of orders late; First Class 95% late against 38% for Standard; $2.14M of profit at risk |
| DataCo late delivery, rebuilt in pandas | Python | The same finding in code. [Notebook repo](https://github.com/charles-agyekum/dataco-late-delivery-pandas) |
| NHS cancer pathway: the 62-day standard | SQL | Training data measured against NHS England's 62-day standard, with the data's limits set out |
| Superstore: order fulfilment & profitability | Power BI | £12.6M sales at an 11.6% margin; Tables lose £64,083 at a 29% discount |
| Vrinda Store: 2022 sales dashboard | Excel | 31,047 orders cleaned, with 7 data quality issues caught; women drive 64% of revenue |
| HR employee attrition: dynamic dashboard | Excel | Attrition checked at 16.12% |
| Adidas US: interactive sales dashboard | Excel | 9,648 rows; 3 of 6 retailers hold about 72% of c.$900M |
| SQL practice: joins, subqueries & CASE | SQL | 31 worked questions |

## Files

- `index.html` is the landing page.
- `projects/*.html` holds one page per project.
- `assets/screenshots/*.png` holds the dashboard screenshots.
- `.nojekyll` tells GitHub Pages to serve the HTML as it is, with no Jekyll build.

## How it is built

Plain HTML and CSS, with no build step. The fonts, Hanken Grotesk and JetBrains Mono, load from Google Fonts. A small inline script runs the hero animation and the number count-up, and every page still reads without JavaScript.

My CV, letters and dashboards share one visual style, which was first drawn from these pages in July 2026.

## Method

I clean the data first and log each change. Every headline figure is checked against its source before a piece counts as done, and each piece ends on a recommendation.
