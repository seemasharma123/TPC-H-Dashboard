# 📊 TPC-H Global Sales Intelligence Dashboard

A dynamic, interactive Power BI report built to explore global sales performance across products, customer segments, and nations — powered by the industry-standard TPC-H benchmark dataset.

---

## 📌 Short Description

The TPC-H Global Sales Intelligence Dashboard is a multi-page analytical Power BI report designed to help users explore over **$229 billion in sales transactions** spanning **7 years**, **25 nations**, and **5 market segments**. The dashboard covers key dimensions including revenue trends, product performance, geographic outliers, and customer segment behavior. It is intended for data analysts, business intelligence professionals, and students who want to explore end-to-end sales analytics using a real-world-style transactional dataset.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 📊 **Power BI Desktop** | Main platform for report development and visualization |
| 🔄 **Power Query** | Data transformation and cleaning layer |
| 🧠 **DAX (Data Analysis Expressions)** | Calculated measures for YTD, MTD, QTD, YoY%, LY Sales, and averages |
| 🗃️ **Data Modeling** | Relationships built across ORDERS, LINEITEM, CUSTOMER, PART, SUPPLIER, NATION, and REGION tables |
| 📁 **File Format** | `.pbix` for development · `.pdf` for static preview |

---

## 🗂️ Data Source

**Source:** [TPC-H Benchmark Dataset](https://www.tpc.org/tpch/) — Transaction Processing Performance Council (Ad Hoc)

A standard industry benchmark that simulates a real-world decision support system for global sales and distribution analytics. The dataset contains fully synthetic transactional data and does not represent any real company.

**Core tables used:**

| Table | Description |
|-------|-------------|
| `ORDERS` | Order-level data — dates, customers, and order totals |
| `LINEITEM` | Line-level detail — quantity, revenue, discount, and parts |
| `CUSTOMER` | Customer demographics and market segment classification |
| `PART` | Product names and part types |
| `SUPPLIER` | Supplier information linked to parts and nations |
| `NATION` / `REGION` | Geographic hierarchy for country and continent-level analysis |

---

## ✨ Features & Highlights

### 🔴 Business Problem

Global sales organizations deal with massive transactional datasets spanning dozens of countries, hundreds of product types, and multiple customer segments — yet drawing clear insights from this data remains a challenge. Key questions like:

- Which nations generate the highest revenue per order?
- Does a higher volume of orders always translate to higher revenue?
- Which customer segment drives the most sales — and why?
- How has revenue trended month-over-month and year-over-year?

…are difficult to answer quickly without an interactive visual layer on top of the raw data.

---

### 🎯 Goal of the Dashboard

To deliver a clean, interactive intelligence tool that:
- Gives executives a single-page summary of global sales health
- Enables analysts to drill into product, segment, and geographic performance
- Surfaces hidden patterns (like geographic outliers or flat YoY growth) that raw tables miss
- Supports time intelligence analysis with YTD, MTD, QTD, and YoY comparisons

---

### 🖥️ Walkthrough of Key Visuals

**Page 1 — Overview**
Navigation hub showing the full 6-page report structure with clearly labeled sections for easy exploration.

**Page 2 — Executive Summary**

Top-line KPIs at a glance:

| Metric | Value |
|--------|-------|
| 💰 Total Revenue | $229.58 Billion |
| 📦 Total Orders | 1.5 Million |
| 📊 Total Quantity Sold | 153.08 Million |
| 🧾 Average Order Value | $153,051.54 |
| 🗓️ Date Range | 1992 – 1998 |

Includes a **revenue by year** bar chart, a **monthly trend line** (1992–1995), and a **regional revenue share** breakdown across Africa, America, Asia, Europe, and the Middle East. The **Top 10 Customers** bar chart identifies high-value accounts by revenue contribution.

**Page 3 — Product Analysis**
A detailed table of parts by name, revenue, quantity, and average order value — alongside a **Top 10 Parts Type** horizontal bar chart. A **scatter plot** of Total Revenue vs. Total Quantity by nation reveals geographic outliers (Iraq and Algeria punch well above their weight in revenue per unit sold).

**Page 4 — Segment Analysis**
A five-segment comparison (Automobile, Furniture, Building, Household, Machinery) showing total revenue per segment and a **nation-level breakdown** table with revenue and parts supplied. A horizontal bar chart compares average order values across all segments.

**Page 5 — Performance Analysis**
Full time intelligence view with a drillable table showing **YTD, MTD, QTD** values per year and month. A side-by-side **YoY% comparison** table tracks each month's growth or decline against the prior year.

**Page 6 — Metric Explorer**
An interactive toggle visual letting users switch between **Total Revenue**, **Total Quantity**, and **YoY%** — displayed simultaneously across nations and market segments for flexible, on-demand analysis.

---

### 💡 Business Impact & Insights

- **📉 Revenue growth was nearly flat** — averaging less than 0.3% annually across 1992–1997, signaling a mature, stable market with limited organic growth. This insight is critical for setting realistic forecasting benchmarks.

- **🌍 Iraq and Algeria are high-value outliers** — both nations generate disproportionately high revenue relative to their order quantities, suggesting higher-priced transactions or a premium product mix. These markets deserve targeted attention.

- **🚗 Automobile leads in revenue through volume, not price** — the segment generates ~$46bn (the highest of all five), yet its average order value ($153.16K) is nearly identical to Machinery ($153.03K). The gap is driven entirely by order volume, not spending per order.

- **📦 No single product dominates** — the top 18 parts names are tightly clustered within a $300K revenue range, meaning no single SKU is a revenue risk or crown jewel. Product diversification is strong.

- **📅 1996 was the most volatile year** — monthly YoY% swings ranged from **+1.49% (August)** to **-1.50% (January)**, the widest variation in the entire dataset. Understanding what drove August's spike could inform future seasonal strategy.

- **🌐 Africa and the Middle East together contribute ~39.8%** of total global revenue — a combined dominance that may surprise stakeholders who default to focusing on Western markets.

---
## 📌 Notes

- 1998 data covers **January through August only** and has been excluded from year-on-year comparisons to prevent skewed trend analysis.
- All revenue figures are in **USD**.
- The TPC-H dataset is **fully synthetic** and does not represent any real company's performance.
