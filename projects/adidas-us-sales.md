---
layout: default
title: Adidas US — Interactive Sales Dashboard
---

# Adidas US — Interactive Sales Dashboard (Excel)

**Tool:** Excel · **Dataset:** Adidas US Sales, a sample dataset, 9,648 rows ·
**Built:** May 2026

[← Back to home](../index.md)

## The question

For an Adidas US sales manager: which retailers, regions, products and sales
methods drive revenue and profit, to inform partner negotiations, stock allocation
and channel strategy.

## Cleaning first

A `=UNIQUE()` audit on Retailer, Region, Sales Method and Product came back clean,
no variants or stray spaces. I documented that check in the sheet under a
consistency block, so anyone opening the file can see the data was validated before
the build. Curated does not mean assumed. Verify, then build.

## What I built

Five pivot charts, with three slicers (Retailer, Region, Product) and an Invoice
Date timeline, all wired through Report Connections so every chart filters at once.
I tested it on Region = West and confirmed all charts re-filtered correctly,
including the Top-10 cities.

Grand total revenue: $899,902,125.

## Findings

Three retailers, West Gear, Foot Locker and Sports Direct, drive close to
three-quarters (around 72%) of revenue, so any partnership trim should come from
the weaker tail, not the top. Sales channels are balanced, roughly Online 38%,
Outlet 34%, In-store 28%, so a shift online should be tested against profit per
channel, not units alone. The product-by-retailer matrix shows Men's Street
Footwear over-indexing at Foot Locker and West Gear, which tells you where to route
surplus stock.

## Why I can talk over it

In procurement I made weekly route-to-buyer decisions on surplus stock. The
product-by-retailer matrix here is that same decision in another industry: where do
I send excess so it actually sells.

## Skills

PivotTables and PivotCharts · combo, pie, bar and line charts · Top-N value
filters · cross-tab analysis · slicers, timeline and Report Connections · dashboard
layout · insight interpretation.
