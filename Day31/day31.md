# AI Supply Chain Control Tower — GitHub README

## Day 31 — AI Operations & Supply Chain Control Towers

An interactive **AI Supply Chain Control Tower simulation** that puts the player in the role of a **Head of Operations** managing real-time supply chain disruptions.

The application simulates a modern operations control center where users monitor live alerts, prioritize incidents, make corrective decisions, and observe the impact of those decisions on business KPIs.

---

## 🚀 Project Overview

**AI Supply Chain Control Tower** is a browser-based operational decision-making simulator designed to demonstrate how supply chain leaders respond to disruptions under time pressure.

The player receives continuously generated operational alerts such as:

* 🚨 Port Congestion
* 🚨 Supplier Delay
* 🚨 Truck Breakdown
* 🚨 Warehouse Running Out of Stock
* 🚨 Customs Inspection
* 🚨 Demand Spike
* 🚨 Factory Machine Failure
* 🚨 Weather Disruption
* 🚨 Wrong Inventory Count
* 🚨 Damaged Shipment

Each disruption has a different urgency, business impact, and set of possible corrective actions.

The objective is to **maximize operational performance before the three-minute simulation ends**.

---

## 🎯 Objectives

The simulation focuses on:

* Real-time operational decision making
* Supply chain disruption management
* Incident prioritization
* Risk assessment
* Cost vs. service-level trade-offs
* Inventory management
* Transportation management
* Customer satisfaction protection
* Revenue protection
* Decision making under time pressure

---

## 🎮 Gameplay

The player assumes the role of:

> **Head of Operations**

During the simulation, multiple incidents appear simultaneously.

For every incident, the player must evaluate:

1. What is happening?
2. How urgent is the problem?
3. What is the potential business impact?
4. Which corrective action provides the best outcome?
5. Is the action worth its operational cost?

The simulation rewards decisions that protect service levels, customers, inventory, transportation efficiency, and revenue.

---

## 📊 Live KPIs

The dashboard continuously tracks:

| KPI                       | Description                                              |
| ------------------------- | -------------------------------------------------------- |
| Service Level %           | Measures the ability to fulfill customer demand on time  |
| Customer Satisfaction     | Represents customer experience and service reliability   |
| Inventory Health          | Tracks inventory availability and balance                |
| Transportation Efficiency | Measures transportation network performance              |
| Operating Cost            | Tracks the financial impact of operational decisions     |
| Revenue Protected         | Estimates revenue preserved through successful decisions |
| Score                     | Overall operational performance                          |
| Remaining Time            | Countdown for the three-minute simulation                |

Every decision can influence one or more KPIs.

---

## 🚨 Operational Alerts

The application randomly generates different supply chain disruptions.

### Port Congestion

Ships are delayed because of congestion at a major port.

Possible responses include:

* Rerouting
* Expediting
* Air freight
* Delaying the decision

### Supplier Delay

A critical supplier cannot deliver materials on schedule.

Possible responses include:

* Use Backup Supplier
* Expedite Shipment
* Increase Production
* Ignore

### Truck Breakdown

A transportation vehicle becomes unavailable.

Possible responses include:

* Reroute Trucks
* Transfer Inventory
* Expedite Shipment
* Delay Decision

### Warehouse Running Out of Stock

Inventory is approaching a critical shortage.

Possible responses include:

* Transfer Inventory
* Expedite Shipment
* Approve Air Freight
* Increase Production

### Customs Inspection

A shipment is delayed because of additional customs inspection.

Possible responses include:

* Wait
* Expedite
* Reroute
* Air Freight

### Demand Spike

Unexpected demand creates pressure on available inventory.

Possible responses include:

* Increase Production
* Transfer Inventory
* Expedite Shipment
* Use Backup Supplier

### Factory Machine Failure

Production capacity suddenly decreases.

Possible responses include:

* Increase Production Elsewhere
* Use Backup Supplier
* Transfer Inventory
* Delay Decision

### Weather Disruption

Severe weather affects transportation routes.

Possible responses include:

* Reroute Trucks
* Air Freight
* Transfer Inventory
* Delay Decision

### Wrong Inventory Count

A warehouse reports an inaccurate inventory quantity.

Possible responses include:

* Verify Inventory
* Transfer Inventory
* Expedite Shipment
* Ignore

### Damaged Shipment

A shipment arrives damaged and cannot fully satisfy demand.

Possible responses include:

* Replacement Shipment
* Air Freight
* Backup Supplier
* Ignore

---

## ⚡ Player Actions

The simulation includes actions such as:

* **Expedite Shipment**
* **Use Backup Supplier**
* **Reroute Trucks**
* **Increase Production**
* **Transfer Inventory**
* **Approve Air Freight**
* **Ignore**
* **Delay Decision**

Each action has different consequences.

Some actions provide immediate benefits but increase operating cost.

Other actions may have lower immediate costs but create additional future risk.

---

## 🧠 Decision Logic

The game is designed around operational trade-offs.

### Good Decisions

Correct decisions can:

* Increase the score
* Improve service level
* Improve customer satisfaction
* Improve inventory health
* Improve transportation efficiency
* Protect revenue
* Reduce future operational risk

### Poor Decisions

Incorrect decisions can:

* Reduce KPIs
* Increase operating cost
* Reduce customer satisfaction
* Increase disruption risk
* Reduce protected revenue
* Lower the overall score

Some decisions also create **delayed consequences**, forcing the player to think beyond the immediate incident.

---

## ⏱️ Difficulty Progression

The simulation lasts:

> **3 Minutes**

As the simulation progresses:

* Alerts appear more frequently
* More incidents remain active simultaneously
* Decision pressure increases
* Multiple disruptions can overlap
* The player must prioritize incidents instead of solving everything immediately

This creates a realistic control-tower environment where operational leaders must continuously reassess priorities.

---

## 🖥️ User Interface

The application uses a premium dark operations-center design.

### Visual Design

* Dark background
* Blue highlights
* Cyan accents
* Red critical alerts
* Orange medium-priority alerts
* Green success indicators
* Glowing KPI cards
* Animated cards
* Smooth transitions
* Hover effects
* Pulse animations for critical incidents
* Responsive dashboard layout

The interface is inspired by modern logistics and enterprise operations control centers.

---

## 📡 Event Log

A live event log records operational activity during the simulation.

Examples include:

* New disruption detected
* Incident prioritized
* Action selected
* KPI changed
* Shipment expedited
* Backup supplier activated
* Transportation rerouted
* Delayed consequence triggered
* Incident successfully resolved

This allows players to review how their decisions affected the operation.

---

## 🔊 Sound Toggle

A visual **Sound Toggle** is included in the interface.

No external audio files or audio APIs are required.

The toggle is designed as a UI feature that could be connected to audio feedback in a future version.

---

## ⏸️ Pause System

The simulation includes a **Pause** button.

When paused:

* Countdown stops
* Alert generation stops
* Player can review the current dashboard
* Simulation can be resumed

---

## ❓ Help / Instructions

A dedicated Help / Instructions modal explains:

* Player role
* Objective
* KPI meanings
* Alert priorities
* Available actions
* Decision strategy
* Scoring concept
* How the simulation ends

This makes the application accessible even to users who have no previous supply chain experience.

---

## 🏁 End-of-Game Dashboard

When the timer reaches zero, the simulation generates a final performance dashboard containing:

### Final Score

Overall operational performance score.

### Performance Grade

Possible grades:

* **A+**
* **A**
* **B**
* **C**
* **D**

### Final KPIs

The final values of:

* Service Level
* Customer Satisfaction
* Inventory Health
* Transportation Efficiency
* Operating Cost
* Revenue Protected
* Score

### Performance Statistics

* Total Alerts Resolved
* Correct Decisions
* Wrong Decisions
* Operational Performance Summary

A **Play Again** button allows the player to restart the simulation and attempt to improve the previous score.

---

## 🛠️ Technology Stack

The application is intentionally lightweight and completely self-contained.

### Frontend

* HTML5
* CSS3
* Vanilla JavaScript

### No Frameworks

The project does **not** use:

* React
* Vue
* Angular
* Bootstrap
* Tailwind CSS

### No External Services

The application does **not** require:

* Backend servers
* APIs
* Databases
* Authentication
* External JavaScript libraries
* Build tools
* Package managers

---

## 📦 Offline Support

The entire application is contained inside a single HTML file.

Therefore:

```text
AI-Supply-Chain-Control-Tower.html
```

can be opened directly in a browser.

No internet connection is required after the file has been generated.

---

## 📁 Project Structure

Recommended Day 31 GitHub structure:

```text
Day31/
│
├── AI-Supply-Chain-Control-Tower.html
├── day31.md
```

---

## ▶️ How to Run

### Step 1

Download or clone the repository.

### Step 2

Open the `Day31` folder.

### Step 3

Open:

```text
AI-Supply-Chain-Control-Tower.html
```

in any modern web browser.

### Step 4

Click **Start Simulation**.

### Step 5

Read the operational alerts.

### Step 6

Prioritize the most urgent incidents.

### Step 7

Select the corrective action with the best operational trade-off.

### Step 8

Monitor the KPI changes.

### Step 9

Continue managing disruptions until the timer reaches zero.

### Step 10

Review the final performance dashboard.

### Step 11

Use **Play Again** to improve the score.

---

## 🧩 Recommended Decision Strategy

A strong operational strategy is to evaluate incidents using:

### 1. Urgency

How quickly will the problem become critical?

### 2. Customer Impact

Will customers experience delays or stockouts?

### 3. Revenue Impact

How much revenue could be lost if the problem remains unresolved?

### 4. Cost

How expensive is the corrective action?

### 5. Future Risk

Could ignoring the issue create a larger disruption later?

### 6. Network Impact

Does the incident affect one shipment or an entire supply chain node?

A useful prioritization principle is:

```text
Critical Customer Impact
        ↓
Revenue Risk
        ↓
Time Sensitivity
        ↓
Network Impact
        ↓
Operational Cost
```

---

## 📈 Learning Outcomes

This project demonstrates practical understanding of:

* Supply chain operations
* Control tower concepts
* Incident management
* Operational KPIs
* Risk prioritization
* Transportation management
* Inventory management
* Supplier management
* Production planning
* Customer service management
* Cost optimization
* Decision-making under uncertainty
* Interactive dashboard design
* Gamification
* Frontend development

---

## 💡 Key Learnings

### Supply Chain

A supply chain control tower provides centralized visibility into operational disruptions and enables faster decision-making.

### Prioritization

Not every alert deserves the same response. The best operational decision depends on urgency, customer impact, financial impact, and available resources.

### Trade-offs

The cheapest decision is not always the best decision.

For example:

```text
Air Freight
↓
High Cost
↓
Fast Recovery
↓
Higher Customer Protection
```

while:

```text
Standard Shipment
↓
Lower Cost
↓
Slower Recovery
↓
Potential Service-Level Risk
```

### Real-Time Decisions

Operations teams frequently need to make decisions with incomplete information and limited time.

### KPI Relationships

A single operational decision can influence multiple KPIs simultaneously.

For example:

```text
Expedite Shipment
        ↓
Higher Operating Cost
        ↓
Higher Service Level
        ↓
Higher Customer Satisfaction
        ↓
More Revenue Protected
```

---

## 🔮 Future Improvements

Potential future enhancements include:

* AI-powered recommendation engine
* Machine-learning disruption prediction
* Real-time logistics APIs
* Interactive supply chain map
* Geographic visualization
* Supplier risk scoring
* Predictive inventory forecasting
* Demand forecasting
* Advanced scenario simulation
* Multiplayer operations mode
* Leaderboards
* Historical performance analytics
* Dynamic pricing impact
* Carbon-emission tracking
* Warehouse capacity visualization
* Transportation network optimization
* AI-generated operational recommendations

---

## 🎯 Project Goal

The ultimate goal of the project is to demonstrate how an **AI-enabled Supply Chain Control Tower** can transform raw operational alerts into actionable decisions.

The simulation combines:

```text
Real-Time Visibility
        +
Operational Intelligence
        +
Decision Making
        +
KPI Monitoring
        +
Risk Management
        =
Supply Chain Control Tower
```

---

## 🏆 Challenge Information

**Challenge:** 60 Days Claude AI Challenge
**Day:** 31
**Topic:** AI Operations & Supply Chain Control Towers
**Project:** AI Supply Chain Control Tower
**Role:** Head of Operations
**Difficulty:** Intermediate
**Estimated Build Time:** ~75 minutes
**Technology:** HTML + CSS + Vanilla JavaScript
**Deliverable:** GitHub Commit URL

---

## 📸 Screenshots

Recommended screenshots to include in the repository:

1. Main Control Tower Dashboard
2. Live KPI Cards
3. Critical Operational Alert
4. Multiple Active Alerts
5. Decision / Action Selection
6. Live Event Log
7. Final Performance Dashboard
8. Final Score and Grade

---

## 🔗 GitHub Submission

After completing the project:

1. Create the `Day31` folder.
2. Add the generated HTML application.
3. Add `day31.md`.
4. Add screenshots.
5. Commit the changes.
6. Push the changes to GitHub.
7. Submit the GitHub commit URL.

---

## 👩‍💻 Author

**Neha Duggal**

Built as part of the **60 Days Claude AI Challenge — Day 31**.

---

## ⭐ Final Takeaway

**AI Supply Chain Control Tower** demonstrates how a modern operations leader can monitor disruptions, prioritize incidents, evaluate trade-offs, and protect business performance through fast, data-driven decisions.

> **Monitor → Prioritize → Decide → Recover → Measure → Improve**

