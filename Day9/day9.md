# Day 9: NutriScope Development & Comparative Analysis

## Executive Summary
This project details the iterative design, architecture, and feature evolution of **NutriScope**, a full-featured, single-file HTML client-side application for personal micro-nutrient and energy tracking. NutriScope translates standard biometrics into precision macro and micronutrient targets while providing real-time data visualisations and dynamic dietary recommendations.

---

## 1. System Architecture & Tech Stack

NutriScope is architected as a lightweight, reactive Single Page Application (SPA) requiring zero backend infrastructure. 

- **Frontend Framework:** Vanilla HTML5 / ES6 JavaScript (reactive DOM updates on state change)
- **Styling & UI:** Tailwind CSS (loaded via CDN) with custom dark mode theme (`slate-900` / `slate-800` card aesthetics)
- **Data Visualisation:** Chart.js for doughnut charts and target completion meters
- **BMR & TDEE Calculations:** Mifflin-St Jeor Equation
  $$\text{BMR (Male)} = 10 \times \text{weight (kg)} + 6.25 \times \text{height (cm)} - 5 \times \text{age (yrs)} + 5$$
  $$\text{BMR (Female)} = 10 \times \text{weight (kg)} + 6.25 \times \text{height (cm)} - 5 \times \text{age (yrs)} - 161$$
- **Storage:** Local in-memory state array with dynamic calculation pipeline

---

## 2. Directory Structure

To maintain clean repository organization, all files related to Day 9 are structured under the `Day9` folder:

```text
Day9/
├── nutriscope_mvp.html         # MVP build (20 foods, core tracking)
├── nutriscope_enhanced.html    # Enhanced build (60 foods, CSV, risk analysis)
├── mvp_screenshot.png          # Browser capture of MVP interface
├── enhanced_screenshot.png     # Browser capture of Enhanced interface
└── day9.md                     # Technical documentation & project learnings
```
## 3. Detailed Feature Comparison: MVP vs. Enhanced

| Feature Category | MVP Version (`nutriscope_mvp.html`) | Enhanced Version (`nutriscope_enhanced.html`) |
| :--- | :--- | :--- |
| **Food Database** | 20 hardcoded Indian and global staples | Expanded 60-item food database + Custom CSV import |
| **Micronutrients Tracked** | 6 Key Micros (Fiber, Iron, Calcium, Vit C, Vit D, Vit B12) | 13 Micros (Added Potassium, Sodium, Zinc, Magnesium, Folate, Vit A, Vit E) |
| **Meal Planning** | Single daily cumulative log | 2-Day side-by-side comparative meal planner tabs |
| **Risk Analysis** | Simple deficiency listing | Clinical-grade health risk alerts with critical threshold warnings |
| **Data Persistence** | Resets upon page reload | `localStorage` persistence for persistent user state |
| **Recommendations** | Food additions based on dietary preference | Context-aware recommendations + absorption synergy advice |
| **Educational Layer** | Standard metrics display | Interactive tooltips, scientific disclaimers, and verifiable sources |

---

## 4. Key Takeaways & Learnings

1. **Incremental Prompt Engineering:** Starting with a minimal functional spec (MVP) ensures a solid architectural core before layering complex features like multi-day tabs or CSV parsers.
2. **Client-Side Data Processing:** Heavy multi-nutrient calculations and interactive charts can run entirely in the browser at zero latency without server overhead.
3. **Bioavailability Synergies:** Modern nutrition tools must account for nutrient interactions (e.g., Vitamin C facilitating non-heme Iron absorption) rather than raw totals alone.
