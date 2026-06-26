---
layout: default
title: HR Employee Attrition — Dynamic Dashboard
---

# HR Employee Attrition — Dynamic Dashboard (Excel)

**Tool:** Excel · **Dataset:** IBM HR Employee Attrition (Kaggle) · **Built:**
May to June 2026

[← Back to home](../)

![IBM HR Employee Attrition dashboard, built in Excel](../assets/screenshots/hr-attrition.png)

## The question

For an HR lead: how much attrition is there, and which groups does it concentrate
in, so retention effort can be aimed rather than spread thin.

## What I built

A fully dynamic dashboard from the raw CSV. The build took the coded fields the
dataset ships with (Education, Job Satisfaction, Job Involvement, all stored as
numbers) and decoded them through lookup tables and a data dictionary, because you
cannot read meaning out of a code without the key.

The core move: the dataset stores attrition as a 1/0 flag, so AVERAGE of the flag
gives the rate directly, the same idea as `AVG(flag)` in SQL. That fed five pivots,
each a single clean rate, then bar and column charts with interpret-not-describe
titles, four slicers wired through Report Connections, and dynamic KPI cards using
custom number formats.

## Verified number

The headline attrition rate verified at **16.12%**.

That figure is here because of a verification catch worth keeping. A KPI first read
24.66%. The maths was not broken. A leftover slicer was filtering the scope. The
lesson stuck: before panicking about a figure, confirm what is filtering it.

## Quality assurance

The workbook carries its own QA tab and lookup tables (`tblLookUPs`) so it is
self-documenting. The QA routine checks the data before any chart is trusted.

## Skills

XLOOKUP recodes and lookup tables · data dictionary for coded fields · 1/0 flag to
rate with AVERAGE · PivotTables with manual value sort · 100% stacked charts ·
slicers and Report Connections · dynamic KPI cards with custom number formats ·
verified a claim against the data and corrected a wrong multiplier.
