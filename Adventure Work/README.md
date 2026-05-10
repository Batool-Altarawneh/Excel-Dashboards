# 🚲 Adventure Works: Sales Analysis Dashboard
**Excel · 2005–2008 · Interactive · Multi-Sheet**

> *"From raw transactional data to a fully interactive executive dashboard — built entirely in Excel."*

---

## 📸 Dashboard Preview

| Detail Dashboard | Time Analysis |
|---|---|
| ![Detail Dashboard](<Images/Detail Analysis.png>) | ![Time Analysis](<Images/Time Analysis Dashboard.png>) |

---

## 📖 The Story

Adventure Works is a fictional bicycle company ,and the backbone of Microsoft's sample datasets. Behind the scenes sits a star-schema database: **29,000+ internet sales transactions**, spanning four years, six countries, and hundreds of products.

The challenge? Turn all of that into something a sales manager can act on in under 60 seconds.

No Power BI. No Python. No external tools. Just Excel.

The result is a dark-themed, fully interactive multi-sheet dashboard that answers the questions that actually matter:

- Which products are driving the most profit  and which customers are buying them?
- Is the business growing year over year, or just getting busier?
- When does revenue peak  by month, by weekday, by quarter?
- How does pricing strategy (above vs. below $150) affect the bottom line?

---

## 📊 What's Inside

### 🗂️ Sheets Overview

| Sheet | Purpose |
|-------|---------|
| `Detail Dashboard` | High-level snapshot : top products, top customers, inventory, gender split, geo map |
| `Time Analysis` | Deep-dive into revenue trends by year, month, weekday, and quarter |
| `Product Analysis` | Product-level profitability and inventory breakdown |
| `Customer Analysis` | Customer demographics, age groups, and geographic contribution |
| `Analysis 2` | Supporting pivot tables and calculations |

---

### 📦 Dataset Structure

Built on a classic star schema with 6 tables:

| Table | Description |
|-------|-------------|
| `FactInternetSales` | Core transactions : quantity, revenue, cost, profit per order line |
| `DimProduct` | Product catalog : names, categories, pricing type, standard cost |
| `DimCustomer` | Customer profiles : demographics, age, gender |
| `DimGeography` | Sales territory : country, city |
| `DimSalesTerritory` | Territory groupings mapped to countries |
| `DimDate` | Full date dimension : year, month, quarter, weekday |

---

## 🔍 Key Insights Built Into the Dashboard

### 💰 Revenue & Profitability
- **$11.02M** total revenue across 2005–2008
- **41.57%** profit margin on **$6.44M** in costs
- **2007 was the peak year**  $11.26M in revenue, nearly double 2006
- **Jun, May & Mar** alone accounted for **55.79%** of 2008 profit

### 🏆 Products
- Top-5 products generated **$1.71M**  vs. $2.87M from all others combined
- **606 available products**, only **101 sold**  505 unsold inventory items flagged
- **Black** is the most profitable color at **$1.49M**
- Products priced **above $150** account for **93.89%** of total profit

### 👥 Customers
- **1,115 total customers** with an average age of **45**
- **50+ age group** contributed **41.12%** of all profit
- **Female riders** slightly edge out males  53.73% vs 46.27%
- **USA and Australia** together drove **60.08%** of profit

### 📅 Time Patterns
- **Weekdays** generate **71.29%** of revenue vs weekends
- **Wednesday and Thursday** are the strongest days
- **Q2 ($2.53M)** consistently outperforms Q1 ($2.03M)
- **73.5%** of all revenue came from just two highlighted years

---

## ⚙️ Interactive Features

| Feature | How It Works |
|---------|-------------|
| 📅 **Year Filter** | Click any year (2005–2008) to filter all visuals |
| 🌍 **Country Filter** | Filter by Australia, Canada, France, Germany, UK, USA |
| 📆 **Month Filter** | Toggle individual months to explore seasonal trends |
| 🔘 **Revenue / Profit / Transaction toggle** | Switch the time-series chart metric instantly |
| ❌ **Clear Filter button** | Reset everything with one click |
| 🔗 **Dashboard navigation** | Switch between Time Analysis and Detail Dashboard |

---

## 🛠️ Built With

- **Microsoft Excel** : PivotTables, PivotCharts, slicers, form controls
- **Power Pivot** : data model, DAX measures, cross-table relationships
- **DAX Measures** : dynamic KPIs, profit margin, % contribution, rank calculations
- **Conditional Formatting** : visual indicators and dynamic highlights
- **VBA** : navigation buttons and filter controls

---



## 🚀 Getting Started

1. **Clone or download** this repository
2. Open `Adventure Work.xlsx` in **Microsoft Excel** (2016 or later recommended)
3. If prompted, **Enable Content** and **Enable Data Model**
4. Navigate between sheets using the tabs at the bottom
5. Use the **Year**, **Country**, and **Month** filters to explore the data

> ⚠️ Power Pivot features require Excel with the **Power Pivot add-in enabled**. Go to `File → Options → Add-ins → COM Add-ins → ✅ Microsoft Power Pivot for Excel`

---


## 📄 License

This project uses the Adventure Works dataset provided by Microsoft for educational and demonstration purposes.

