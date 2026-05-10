# 🚌 TransitPulse - Urban Bus Ridership Dashboard

**Excel · 2023–2024 · Interactive · Multi-Sheet**

> *"Behind every bus route is a pattern. TransitPulse turns 200 ridership records into decisions that move cities forward."*

---


## 📸 Dashboard Preview

| Demographics | Operations |
|:---:|:---:|
| <img src="https://raw.githubusercontent.com/Batool-Altarawneh/Excel-Dashboards/main/TransitPulse/Images/TransitPulse%20-%20Demographics.png" width="500"/> | <img src="https://raw.githubusercontent.com/Batool-Altarawneh/Excel-Dashboards/main/TransitPulse/Images/TransitPulse%20-%20Operations.png" width="500"/> |

| Recommendations |
|:---:|
| <img src="https://raw.githubusercontent.com/Batool-Altarawneh/Excel-Dashboards/main/TransitPulse/Images/TransitPulse%20-%20Recommendations.png" width="500"/> |

---

## 📖 The Story

A city's bus network is only as good as the decisions behind it. Too many buses on empty routes. Not enough on the ones that are packed. Riders who don't feel safe. Schedules that don't match when people actually travel.

**TransitPulse** was built to answer one question: *what does the data say we should do?*

Starting from raw ridership logs across 10 routes, 40 buses, and 100 unique riders , this dashboard surfaces the patterns, gaps, and opportunities hiding in plain sight. It was built entirely in **Microsoft Excel** using PivotTables, Power Pivot DAX measures, Power Query,  and interactive form controls.

---

## 📊 Dashboard Sheets

### 1. 🧑‍🤝‍🧑 Demographics
Understand *who* is riding and *where*.

| Metric | Value |
|--------|-------|
| Total Riders | **6,587** |
| Avg. Riders / Trip | **33** |
| Busiest Route | **East-West Express (1,322)** |
| Least Busy Route | **South Line (185)** |

- Rider distribution across all 10 routes
- Gender breakdown : Male 74% · Female 15% · Other 11%
- Riders by occupation : Other, Professional, Self-Employed, Unemployed, Retired, Student
- Total riders by age group : 30–39 leads with 1,474
- Peak time by occupation with AM/PM color coding
- Interactive Top 5 / Bottom 5 bus toggle with dynamic chart title

---

### 2. ⚙️ Operations
Understand *when* the system is under pressure.

| Metric | Value |
|--------|-------|
| Peak Hour | **8:57 PM** |
| Off-Peak Hour | **7:50 PM** |
| PM Riders | **64.61%** |
| AM Riders | **35.39%** |
| YoY Change | **▼ -83.50% (needs attention)** |

- Bus utilization by time range (AM / Midday / PM)
- Monthly ridership distribution — Jan 933 → Dec 5,654
- Weekday ridership — Sun & Mon are highest traffic days
- Fleet utilization breakdown across 77 buses:
  - ✅ Well-utilized: 38 buses (49.35%)
  - 🔵 Over-utilized: 20 buses (25.97%)
  - 🟠 Under-utilized: 19 buses (24.68%)
- 2023 vs 2024 year-on-year comparison

---

### 3. 💡 Recommendations
5 data-driven actions to optimise the service.

| # | Action |
|---|--------|
| 1 | Increase frequency on East-West Express & Central Line |
| 2 | Target female and non-binary riders with safety campaigns |
| 3 | Introduce off-peak discounts for students and retirees |
| 4 | Align schedules with occupational peak times |
| 5 | Evaluate or reassign bottom 5 underperforming buses |

---

## 🗂️ Dataset

| File | Description | Rows |
|------|-------------|------|
| `Facttable_ridership.csv` | Core ridership log — BusID, Date, Time, NumberOfRiders, RiderID | 200 |
| `Dim_buses.csv` | Bus details — BusID, RouteID, BusNumber, Capacity | 40 |
| `Dim_demographics.csv` | Rider profiles — Age, Gender, Occupation | 100 |
| `Dim_routes.csv` | Route info — RouteName, Start/End Location, TripFee, Schedule | 10 |

### Data Model (Star Schema)
```
                    Dim_buses
                        |
Dim_demographics ── Facttable_ridership ── Dim_routes
```

### Routes Covered
| Route | From | To | Fee |
|-------|------|----|-----|
| East-West Express | Eastside | Westside | $13 |
| Central Line | Downtown | Uptown | $50 |
| Airport Express | Airport | Downtown | $37 |
| University Line | University | Tech Park | $19 |
| Suburban Line | Suburbia | Downtown | $33 |
| City Shuttle | City Center | City Hall | $19 |
| Market Line | Central Market | Farmers Market | $18 |
| Beachfront Route | Beachside | Harbor Point | $19 |
| North Circular | North Station | Circular Quay | $31 |
| South Line | South Park | Old Town | $29 |

---

## 🛠️ Built With

| Tool | Purpose |
|------|---------|
| Excel PivotTables | Data aggregation per route, bus, rider |
| Power Pivot (DAX) | Custom measures : Peak Time, Utilization %, YoY |
|Power Query | Filtering, Sorting,Custom Columns|
| Form Controls (Radio Buttons) | Top 5 / Bottom 5 bus toggle |
| Conditional Formatting | AM/PM color coding, data bars |
| VBA Macro | Learn More button , Recommendations sheet |

---

## 🚀 How to Use

1. Download `TransitPulse.xlsx`
2. Open in **Microsoft Excel 2016 or later**
3. Enable **Power Pivot** add-in if prompted
4. Navigate using the sheet tabs at the bottom:
   - `Dashboard` — Demographics view
   - `Operations` — Operational metrics
   - `Recommendations` — Action plan
5. Use the **Top / Bottom radio buttons** to toggle bus performance
6. Click **Learn More** on the key insight card to open recommendations
7. Click **Back to Dashboard** to return

---

