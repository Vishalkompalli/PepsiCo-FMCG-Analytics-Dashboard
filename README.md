# PepsiCo FMCG Analytics Dashboard

> **Solving fragmented commercial visibility across regions, products, and channels for one of the world's largest FMCG companies.**

<img width="1250" height="696" alt="pepsico_1" src="https://github.com/user-attachments/assets/2b9cf4c0-dd00-406e-8161-f0db3fac91f3" />
<img width="1243" height="691" alt="pepsico_2" src="https://github.com/user-attachments/assets/01014d64-ff85-4913-93d3-25764727059a" />

---

## The Problem

PepsiCo operates across 8 global regions, multiple product lines, and three distinct categories - Beverages, Hydration, and Snacks. At that scale, a familiar but costly problem emerges: **no one has the full picture**.

Regional managers were working from siloed data. Sales performance across Africa, China, India, APAC, North America, Europe, Latin America, and the Middle East couldn't be compared in a single view. Profitability by product - Pepsi, Doritos, Gatorade, Lay's, Mountain Dew, Pepsi Zero, Tropicana - wasn't visible alongside volume and trade spend. Identifying where gross sales were leaking into trade spend, or which region was dragging down profit, required manual aggregation across spreadsheets.

The result: slow decisions, invisible margin erosion, and no way to connect commercial activity to business outcomes in real time.

---

## The Solution

I designed and built a **5-page Power BI dashboard** that consolidates PepsiCo's global sales, profitability, trade spend, and volume data into a single interactive intelligence layer - built for both executive oversight and granular operational drill-down.

The dashboard was developed end-to-end: from UX wireframing through data modelling, DAX measure development, time-intelligence calculations, Row-Level Security implementation, and final visual design.

---

## What Was Built

The bottom navigation bar tells the full story: **Executive Summary → Profitability & Channel Performance → Product Performance → Region Insights → RLS**.

---

### Page 1 - Executive Summary
The command centre. Four headline KPIs - **$44.60M Total Net Sales, $50.96M Total Gross Sales, $9.41M Total Profit, 495K Units Sold** - give leadership an immediate read on business health. A global sales trend bar chart breaks performance down by all 8 regions, and a donut chart shows regional share of Total Net Sales, with Africa leading at 20.8% ($5.70M). Three cross-page slicers (Date Range, Region, Product Name) make every view interactive and self-service.

---

### Page 2 - Profitability & Channel Performance
Where the margin story lives. This page surfaces **Profit YTD ($2.45M)** and **Profit MTD ($99.61K)** alongside a full product-level profit breakdown - all 7 products (Doritos, Gatorade, Lay's, Mountain Dew, Pepsi, Pepsi Zero, Tropicana) each contributing ~$9.4M in total profit, confirming balanced portfolio performance. Two paired bar charts compare **Total Gross Sales vs. Trade Spend by Category** and **Total Net Sales vs. Profit by Category** across Beverages, Hydration, and Snacks - making the cost of trade promotions visible against actual margin outcomes.

---

### Page 3 - Product Performance
Built for brand and category managers. Slicers let users isolate any individual product - Doritos, Gatorade, Lay's, Mountain Dew, Pepsi, Pepsi Zero, or Tropicana - and immediately see **Total Net Sales ($41.23M), Total Profit ($8.69M), and Average Discount % (0.12)**. A product sales trend area chart shows year-over-year movement (2021–2023), a category split bar compares Beverages vs. Hydration, and a regional line chart ranks all 8 markets by net sales - surfacing that Middle East ($1.7M) significantly underperforms Africa ($5.4M) for the same product.

---

### Page 4 - Region Insights
The regional deep-dive. A clustered bar chart plots **Total Gross Sales and Trade Spend side-by-side across all 8 regions**, making the relationship between revenue and promotional cost explicit - Africa leads gross sales at $6.1M with $0.9M trade spend. Two donut charts break down **Total Profit by Region** and **Total Units Sold by Region**, showing a near-even distribution across markets (~19–21% each) - signalling no single region dependency but also flagging where profit share lags unit share.

---

### Page 5 - RLS (Row-Level Security)
A production-grade access control layer built directly into the data model. RLS ensures that when deployed, regional managers only see data relevant to their market - the same dashboard serves every stakeholder without exposing data they shouldn't see. This reflects real enterprise BI deployment standards, not just a demo build.

---

## How the Problem Was Solved

| Challenge | Design Decision |
|---|---|
| No single view across 8 global regions | Unified data model with region hierarchy enabling cross-market comparison in one page |
| Trade spend impact on margin invisible | Paired gross sales vs. trade spend visuals on Profitability page make the cost of promotions explicit |
| Product performance required manual pulls | Product-level slicer with instant KPI refresh across net sales, profit, and discount % |
| Year-over-year trends not tracked | Time-intelligence DAX measures powering YTD, MTD, and year-on-year trend charts |
| No data governance for multi-region rollout | Row-Level Security (RLS) built into the model - each regional manager sees only their data |
| Stakeholder alignment before build | UX wireframes produced upfront, defining page structure and navigation logic before any development |

---

## Business Impact

- **Full commercial visibility in one report** - $44.60M in net sales, $50.96M gross, $9.41M profit, and 495K units tracked across 8 regions and 7 products simultaneously
- **Trade spend accountability** - for the first time, gross-to-net margin erosion from trade promotions is visible by category, not buried in finance reports
- **Self-service by design** - three cross-page slicers (date, region, product) mean any stakeholder can answer their own question without raising a data request
- **Enterprise-ready deployment** - RLS implementation means this isn't a prototype; it's a dashboard that can be published and used by a real multi-region commercial team
- **Proactive performance management** - year-on-year trend data (2021–2023) makes a 24% revenue decline from 2022 to 2023 visible and actionable, not discovered in hindsight

---

## Dashboard Pages at a Glance

| Page | Primary Question Answered |
|---|---|
| Executive Summary | How is the business performing globally right now? |
| Profitability & Channel Performance | Where is margin being made or lost, by product and category? |
| Product Performance | How is each brand performing across regions over time? |
| Region Insights | Which markets lead on sales, profit, and volume - and where is trade spend going? |
| RLS | Who should see what when this goes live? |

---

## Project Artefacts

| File / Folder | What It Contains |
|---|---|
| `PepsiCo_1.pbix` | Full Power BI file - data model, all DAX measures, RLS configuration, and 5 report pages |
| `PepsiCo_Project_Requirements.pdf` | Business objectives, KPI definitions, and stakeholder reporting needs |
| `Wireframes/` | UX layout sketches defining page structure and navigation logic, produced before development |
| `PepsiCo Datasets/` | Source data - sales transactions, product master (7 SKUs), region hierarchy (8 markets), category classifications |

---

## Tools & Skills

`Power BI` · `DAX` · `Time Intelligence` · `Row-Level Security (RLS)` · `Data Modelling` · `UX Wireframing` · `FMCG Domain Knowledge` · `KPI Design` · `Business Intelligence`

---

## Getting Started

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
2. Clone this repository
   ```bash
   git clone https://github.com/Vishalkompalli/PepsiCo-FMCG-Analytics-Dashboard.git
   ```
3. Open `PepsiCo_1.pbix` in Power BI Desktop
4. Ensure dataset files in `PepsiCo Datasets/` are correctly linked in the data model
5. Use the cross-page slicers (Date Range, Region, Product Name) and page navigation to explore all 5 views

---
*This is a personal project and not affiliated to PepsiCo, Inc*
*Built to demonstrate how structured analytics can turn fragmented commercial data into decisions.*
