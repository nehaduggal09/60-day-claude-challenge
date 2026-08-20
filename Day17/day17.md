# Day 17 — Vehicle Cost Analysis Dashboard 🚗📊

## 📌 Project Overview

This project is part of my **60 Days Claude AI Challenge — Day 17**.

The objective was to build a **Vehicle Cost Analysis Dashboard** using a CSV dataset and Claude AI. The dashboard analyzes fuel costs, maintenance expenses, CO₂ emissions, refueling time, vehicle age, and E85 economics.

The final dashboard is created as a **single responsive HTML file** using pure HTML, CSS, JavaScript, and SVG charts — without any external CDN.

---

## 🎯 Objectives

* Analyze vehicle operating costs from CSV data
* Compare different fuel types
* Calculate average fuel cost per kilometer
* Analyze CO₂ emissions per kilometer
* Compare maintenance costs
* Analyze refueling/recharging time
* Study vehicle age vs. running and maintenance costs
* Evaluate E85 economics
* Calculate E85 break-even price
* Generate an E85 score out of 10
* Present insights through an interactive dashboard

---

## 🚘 Vehicle Details

* **Vehicle:** [YOUR VEHICLE MODEL]
* **Fuel:** [Petrol/Diesel/CNG/E85/EV]
* **Usage:** [City/Highway/Mixed/Fleet]
* **KM/month:** [YOUR KM/MONTH]
* **Car Age:** [YOUR CAR AGE] years

---

## 📊 Metrics Calculated

### Fuel Cost per Kilometer

`Fuel_Cost_INR ÷ Distance_km`

### CO₂ Emissions per Kilometer

`CO2_emitted_kg ÷ Distance_km`

### Maintenance Cost per Kilometer

`Maintenance_Cost_INR ÷ Distance_km`

### Average Refueling/Recharging Time

`Refuel_Recharge_time_min`

### Vehicle Age Analysis

Vehicles are categorized into:

* **New:** 0–2 years
* **Mid-life:** 3–5 years
* **Aged:** 6–9 years
* **Old:** 10+ years

For every age bucket, the dashboard compares:

* Cost/km
* Maintenance/km

The user's vehicle age is highlighted on the analysis.

---

## ⛽ E85 Economic Analysis

The dashboard evaluates the E85 fuel paradox using three calculations.

### Pump Saving

`((Petrol_price − E85_price) / Petrol_price) × 100`

### Running Penalty

`((E85_cpkm − Petrol_cpkm) / Petrol_cpkm) × 100`

### Break-even Price

`(E85_mileage ÷ Petrol_mileage) × Petrol_price`

This helps determine whether the lower E85 pump price actually compensates for its running-cost penalty.

---

## 🏆 E85 Score

E85 receives a score out of **10 points** based on:

| Factor      | Points |
| ----------- | -----: |
| Cost        |      4 |
| CO₂         |      3 |
| Refueling   |      2 |
| Maintenance |      1 |
| **Total**   | **10** |

The dashboard presents the final score using an animated SVG/CSS gauge along with a one-line verdict.

---

## 📈 Dashboard Features

### KPI Cards

The dashboard contains five major KPIs:

1. Vehicle fuel cost/km
2. E85 cost/km
3. E85 premium vs Petrol
4. E85 break-even price
5. Estimated monthly vehicle cost

### Visualizations

* **SVG Bar Chart** — Cost/km by fuel type
* **SVG Doughnut Chart** — CO₂/km by fuel type
* **SVG Line Chart** — Cost/km vs vehicle age
* **Vertical Age Marker** — Highlights the selected vehicle's age
* **SVG Gauge** — E85 score out of 10
* **Interactive Hover Tooltips**

---

## 🎨 Dashboard Design

The dashboard uses a dark **navy glassmorphism** design.

### Fuel Colors

* 🟠 **E85** — Amber
* 🔵 **Petrol** — Blue
* ⚪ **Diesel** — Grey
* 🟢 **CNG** — Green
* 🟣 **EV** — Purple

The dashboard is designed to be responsive across:

**375px → 1440px**

---

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript
* SVG
* CSV Data Analysis
* Claude AI

### Technical Constraints

* No external CDN
* Pure SVG charts
* CSS inside `<style>`
* JavaScript inside `<script>`
* Single HTML dashboard
* Responsive design

---


## 🔍 Key Analysis Areas

The dashboard was reviewed for:

* Fuel cost efficiency
* Monthly running cost
* Maintenance burden
* CO₂ impact
* Refueling/recharging time
* Vehicle age impact
* E85 pump-price savings
* E85 running-cost penalty
* E85 break-even economics
* Overall E85 score

---

## 💡 Learnings

Through this task, I learned how AI can be used to transform raw CSV data into an interactive analytical dashboard.

Key learnings:

* Converting raw data into meaningful KPIs
* Performing fuel-wise aggregation
* Creating calculated financial and environmental metrics
* Understanding the difference between pump-price savings and actual running costs
* Using break-even analysis for fuel economics
* Creating responsive dashboards without external libraries
* Building SVG-based data visualizations
* Presenting analytical findings in an investor/user-friendly format
* Using Claude AI for end-to-end data analysis and dashboard generation

---

## 🚀 Challenge

**60 Days Claude AI Challenge — Day 17**

**Focus:** Vehicle Cost Analysis & E85 Economics

---

## 📌 Conclusion

The Vehicle Cost Analysis Dashboard combines **financial, environmental, maintenance, and operational metrics** into a single interactive interface.

The analysis demonstrates how structured vehicle data can be converted into actionable insights using data analytics and AI-assisted dashboard development.

---

### 👩‍💻 Created By

**Neha Duggal**

B.Tech — Computer Science Engineering (AI & ML)

#60DaysClaudeAIChallenge #Day17 #ClaudeAI #DataAnalytics #Dashboard #HTML #JavaScript #SVG #DataVisualization #VehicleAnalytics #FuelAnalysis #E85 #DataAnalyst #AI #Analytics #GitHub
