---
layout: default
title: Superstore — Order Fulfilment and Profitability
---

# Order Fulfilment and Profitability (Power BI)

**Tool:** Power BI Desktop · **Dataset:** Global Superstore, 51,290 order lines,
25,728 orders, 2022 to 2023 · **Built:** June 2026

[← Back to home](../)

![Superstore Order Fulfilment dashboard, built in Power BI](../assets/screenshots/superstore.png)

## The question

The Head of Operations and the Commercial Director want to know how fast orders
are fulfilled, whether the priority and ship-mode system works, where margin is
leaking, which lines drive or drain profit, and which markets are strong or weak.

## What I built

1. **Get Data.** Loaded Orders and Returns from Excel.
2. **Power Query (ETL).** Promoted headers (Returns had them trapped in row 1),
   set date and decimal types, and added a calculated column
   `Fulfilment Days = Duration.Days([Ship Date] - [Order Date])`.
3. **Model.** Returns (1) to Orders (many) on `Order ID`, cross-filter set to
   Both so returns respond to slicers.
4. **DAX.** Seven measures: Total Sales, Total Profit, Profit Margin % (`DIVIDE`),
   Order Count (`DISTINCTCOUNT`), Avg Fulfilment Days (`AVERAGE`), Shipping Cost %
   of Sales, and Return Rate across the two tables.
5. **Visuals.** Seven KPI cards, fulfilment by ship mode, a sales and profit
   trend, a discount-versus-profit scatter, profit by sub-category, a country
   map, and a Market slicer.
6. **Narrative.** Interpret-not-describe titles plus a Key Findings panel.

## Verified headline numbers

| KPI | Value |
|---|---|
| Total Sales | £12,642,501.91 |
| Total Profit | £1,467,457.29 |
| Profit Margin % | 11.61% |
| Order Count | 25,728 |
| Avg Fulfilment Days | 3.97 |
| Shipping Cost % of Sales | 10.74% |
| Return Rate | 4.19% (1,079 of 25,728 orders) |

## Findings and recommendation

Fulfilment is healthy and uniform, around four days across every market, with
ship tiers behaving as named. There is no regional weak spot.

Sales are strong but margin is thin, 11.6% on £12.6M. The pressure point is
profitability, not volume. The leak is one sub-category: Tables sells at a 29%
average discount and loses £64,083, the only major loss-making line. That was
confirmed from two independent visuals, the sorted profit bar and the
discount-profit scatter.

Recommendation: cap or review discounting on Tables and monitor other
high-discount lines to protect margin. Fulfilment needs no intervention.

## A note on honesty

Superstore is the most over-used dataset in analytics, so this build is here to
prove the toolchain, not as the centrepiece. The differentiated piece is the
DataCo supply-chain build. I would rather show you a generic dataset handled
correctly than dress it up as something rare.

## Skills

Power Query ETL · calculated columns in M · star-schema relationship and
cross-filter direction · seven DAX measures · KPI, bar, line, scatter, map and
slicer visuals · source-verified every figure, including catching a
rounding-masked filter change on Avg Fulfilment Days.
