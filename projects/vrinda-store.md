---
layout: default
title: Vrinda Store — 2022 Sales Dashboard
---

# Vrinda Store — 2022 Sales Dashboard (Excel)

**Tool:** Excel · **Dataset:** Vrinda Store, a sample fashion e-commerce dataset,
31,047 orders · **Built:** May 2026

[← Back to home](../)

![Vrinda Store 2022 Sales dashboard, built in Excel](../assets/screenshots/vrinda.png)

## The question

For the owner of an online fashion retailer: who buys, what they buy, where,
through which channel, and how that changed across 2022, to inform 2023 targets,
inventory and channel spend.

## Cleaning first

I ran a `=UNIQUE()` pass on every categorical column before building anything.
That surfaced seven data-quality issues:

| Issue | Where | Fix | Why it mattered |
|---|---|---|---|
| Trailing space in header | `Channel ` | retyped | broke pivot and slicer field matching |
| Abbreviations | Gender: W and M | IF-recode to Women / Men | would have split each chart into four bars |
| Text-as-number | Qty: "One", "Two" | IF-recode to 1 / 2 | text will not SUM, so totals break |
| Mixed case | `kurta` lowercase | PROPER | looked unprofessional |
| Case inconsistency | ship-state spellings | PROPER | tidy grouping |
| Case inconsistency | ship-city spellings | PROPER | tidy grouping |
| Hidden space confirmed | header | `=LEN(H1)-LEN(TRIM(H1))` | proved the space before fixing it |

The quantity column spelling out "One" and "Two" as text is the trap most people
miss. It looks fine and silently breaks every total.

## What I built

Five pivot-driven charts answering the six homework questions, with three slicers
(Month, Channel, Category) wired through Report Connections. The Month slicer is
deliberately not connected to the trend chart, so the twelve-month trend stays
intact while the categorical charts filter.

Total revenue across 31,047 orders: ₹21,176,377.

## Findings

Women drove 64% of 2022 revenue, concentrated in two womenswear categories, Set
and Kurta, and two states, Maharashtra and Karnataka. Amazon was the dominant
channel at roughly a third of sales, with Flipkart and Myntra following. Both
sales and order volume declined steadily through the year, peaking in March and
bottoming in December.

With revenue leaning on one state, one channel and one customer segment, I would
flag that dependence as the risk to watch before setting 2023 targets.

## Skills

Data cleaning (TRIM, PROPER, IF-recode) · UNIQUE-based QA · PivotTables · combo
charts with a secondary axis · Top-N value filters · slicers and Report
Connections · stakeholder narrative.
