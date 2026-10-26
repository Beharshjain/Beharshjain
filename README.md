# HARSH JAIN — DATA ANALYST

> **I don't just make dashboards. I find the decision hiding inside messy data.**

Most profiles show tools. This one shows proof first.

---

## The 60-Second Recruiter Brief

| | |
| --- | --- |
| **Role I do best** | Data Analyst — cleaning, modelling, and explaining sales / business data |
| **Proof, not promises** | One end-to-end project below, fully reproducible, with real numbers |
| **Core stack** | Power Query (M) · DAX · Power BI · Excel · Python · SQL |
| **Open to** | Data Analyst internships, data projects, and collaborations |

---

## CASE FILE 01: Sales Performance — From Messy Export to Board-Ready Dashboard

**Project:** [sales-performance-analytics-dashboard](https://github.com/Beharshjain/sales-performance-analytics-dashboard)

A multi-year retail sales export, FY2023–FY2025, that was unusable for reporting until it was cleaned and modelled.

### The mess I started with

- 9,548 raw rows with inconsistent region casing — `"north"` / `"NORTH"` / `" North "`
- 4 different date formats mixed in the same column
- ~350 exact duplicate rows from repeated export pulls
- Missing discount and customer-segment values, plus zero/negative quantity rows

### The pipeline I built

1. **Clean — Power Query (M):** standardised casing, parsed all 4 date formats with a custom `fnParseMixedDate` function, removed duplicates and invalid rows, imputed missing values, and added `GrossRevenue`, `NetRevenue`, `Profit`, `ProfitMargin`, plus Year / Quarter / Month columns.
2. **Model — DAX:** Total Revenue, Total Profit, Profit Margin %, Average Order Value, plus YoY growth, MTD / QTD / YTD, rolling 3-month revenue, and region / product rankings.
3. **Visualise — Excel dashboard:** KPI cards, revenue by region and category, monthly trend across 3 years, top 10 products, and segment / sales-rep breakdowns — all on live formulas, so the dashboard recalculates when the data changes.
4. **Reproduce — Python mirror:** the same cleaning and dashboard build is reproducible from scratch with `clean_data.py` and `build_excel_dashboard.py`, with a full data dictionary in `docs/`.

### What came out of it

- **9,115 clean rows** from 9,548 raw rows — **781 inconsistent / invalid records resolved**
- **$5.71M net revenue, $2.20M profit, ~38.6% blended margin** across FY2023–FY2025
- **Clear Nov / Dec seasonality** visible in the monthly trend
- **Central and West lead on revenue; Electronics and Office Supplies lead on category**

*These are demo-dataset results. The point is the method: swap in a real company export and the same pipeline — Power Query steps, DAX measures, dashboard layout — applies unchanged.*

---

## The Harsh Method

This is how I work on any dataset, not just this one:

1. **Clean first, analyse second.** No chart is trusted until duplicates, bad dates, and bad casing are fixed.
2. **Define the KPI before visualising it.** Revenue, profit, and margin mean nothing without an exact definition.
3. **Show the trend, then the reason.** A spike is not an insight — the region, category, or segment behind it is.
4. **End with a "so what?"** Every finding closes with what should happen next.

---

## Tools I Actually Ship With

Not a badge wall — where each tool is used in real work:

- **Power Query (M)** — the cleaning engine for messy exports
- **DAX** — time intelligence and KPI measures that don't break
- **Excel** — live-formula dashboards stakeholders can actually use
- **Power BI** — the rebuild path for the same model as a `.pbix` report
- **Python (Pandas)** — reproducible cleaning and dashboard generation
- **SQL** — querying and structuring data before it reaches a dashboard

---

## What I Won't Do

- A chart without cleaning the data behind it
- A KPI without saying exactly how it's calculated
- An insight without a clear next step

That's the difference between a report that looks nice and analysis a business can act on.

---

## GitHub Snapshot

![Harsh's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Beharshjain&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)

---

> **If your data is messy, that's my favourite kind.**
>
> Open to Data Analyst internships, data projects, and collaborations.
