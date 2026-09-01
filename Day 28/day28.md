# 🏥 Hospital Admission Readiness Simulator — Day 28

An interactive **Hospital Admission Readiness Simulator** built as part of the **60 Days Claude Challenge**.

The application simulates the workflow of a **Hospital Admission Coordinator**, helping users evaluate admission readiness, resolve administrative barriers, manage prior authorization scenarios, track risks, and understand the final admission decision.

---

## 📌 Project Overview

The Hospital Admission Readiness Simulator is a healthcare workflow simulation designed around realistic hospital admission coordination tasks.

Users can configure:

- Provider
- Attending Physician
- Diagnosis
- Admission Type
- Prior Authorization Status
- Admission Date

The simulator then generates an initial readiness assessment based on:

- Prior Authorization
- Clinical Documentation
- Physician Orders
- Insurance
- Consent
- Bed Availability

Users must complete workflow actions and resolve admission risks to improve the readiness score.

> ⚠️ **Training Disclaimer:** This is an educational simulation only. It does not provide real medical, insurance, utilization-review, or admission decisions.

---

## 🎯 Objectives

The main objectives of this project are to:

- Simulate hospital admission coordination
- Understand admission readiness workflows
- Demonstrate Prior Authorization scenarios
- Track documentation and insurance risks
- Simulate bed assignment and patient arrival workflows
- Understand the role of care coordination teams
- Demonstrate readiness scoring
- Practice resolving administrative barriers
- Simulate final admission decisions
- Explore healthcare workflow automation using JavaScript

---

## ✨ Key Features

### 🏥 Admission Setup

Users can enter:

- Provider
- Attending Physician
- Diagnosis
- Admission Type
- Prior Authorization Status
- Admission Date

Supported diagnoses:

- Acute MI
- CHF
- Pneumonia
- Elective Surgery
- Hip Fracture

Supported admission types:

- Inpatient
- Observation
- Emergency
- ICU
- Same-Day Surgery

Provider and payer names are clearly identified as **illustrative training data**.

---

## ⚕️ Observation Status Notice

When Observation is selected, the simulator displays:

> **CMS 2-Midnight Rule applies — different cost-sharing, SNF eligibility, and billing than inpatient. Medicare patients require written MOON notification.**

This highlights the difference between observation and inpatient status within the simulation.

---

## 📊 Initial Admission Readiness Analysis

The simulator generates an initial readiness score between **30% and 60%**.

The score evaluates:

| Category | Weight |
|---|---:|
| Prior Authorization | 25% |
| Clinical Documentation | 20% |
| Physician Orders | 20% |
| Insurance | 15% |
| Consent | 10% |
| Bed | 10% |

The simulator intentionally does not reveal the final admission decision during the initial analysis.

### Special Rule

A **Denied Prior Authorization + ICU admission** cannot reach 70% readiness through administrative tasks alone.

This forces the user to address the underlying authorization barrier instead of relying only on workflow completion.

---

## 🔐 Prior Authorization Workflow

The simulator supports three major PA scenarios.

### ✅ Approved

The workflow continues normally.

### ⏳ Pending

Available actions include:

- Follow Up
- Upload Documents
- Contact Physician

### ❌ Denied

Available actions include:

- Review Reason
- Contact Insurance
- Submit Appeal

A successful appeal changes the PA status from:

**Denied → Approved**

---

## 🔄 Workflow Actions

Users can complete actions to improve admission readiness:

- Assign Bed
- Verify Insurance
- Upload Documentation
- Complete Consent
- Contact Physician
- Notify Nursing
- Prepare Patient Arrival

Each completed action contributes toward resolving admission barriers.

---

## 🫀 Clinical Criteria Alerts

For **Acute MI** and **CHF**, the simulator displays a medical-necessity criteria note:

> **InterQual/Milliman thresholds apply — ensure documentation meets medical necessity standards before UR review.**

This reinforces the importance of adequate clinical documentation before utilization review.

---

## 🗓️ Admission Timeline

The simulator visualizes the admission workflow through the following milestones:

1. PA Review
2. Insurance Verification
3. Bed Assignment
4. Documentation
5. Consent
6. Patient Arrival
7. Registration
8. Clinical Assessment
9. Admission Complete

This provides a clear task-based representation of the admission journey.

---

## 🤝 Care Coordination

The simulator includes role-based care coordination cards for:

### 👨‍⚕️ Attending

Responsible for clinical orders, documentation, and physician communication.

### 📋 Case Manager

Coordinates admission readiness and administrative requirements.

### 👩‍⚕️ Nursing

Supports patient arrival, clinical preparation, and admission coordination.

### 🔎 Utilization Review

Focuses on:

- Concurrent review
- Denial risk identification
- InterQual
- Milliman

### 🏠 Discharge Planner

Supports continuity planning and downstream discharge coordination.

---

## ⚠️ Risk Tracking

The application tracks four major risk categories:

- Documentation Risk
- Insurance Risk
- Bed Risk
- Clinical Risk

Clinical risk receives additional weight for:

- Acute MI
- CHF
- ICU admissions

This helps users identify which issues require the highest priority.

---

## 📈 Governance Snapshot

When readiness reaches **75% or higher**, the simulator reveals a Governance Snapshot containing illustrative industry estimates:

- PA turnaround: **3–5 days**
- Inpatient denial rate: **~8–10% (CMS)**
- PA rework cost: **~$11/transaction (CAQH)**

These values are presented as **estimates for training purposes**, not as guarantees or patient-specific predictions.

---

## 🏁 Final Admission Decision

The simulator evaluates the completed workflow only after the required actions and risk factors have been addressed.

### ✅ Readiness ≥ 90%

The simulator displays:

**Admit — full summary**

The summary includes the completed admission workflow, resolved items, remaining risks, and readiness information.

### ⚠️ Readiness < 90%

The simulator displays:

**Not Ready**

The result identifies:

- Missing items
- Required actions
- Remaining risks
- Unresolved workflow barriers

---

## 🧪 Scenario Testing

The simulator can be restarted to test multiple admission scenarios.

Recommended scenarios include:

### Scenario 1 — Acute MI + ICU

Test high clinical risk and authorization requirements.

### Scenario 2 — CHF + Inpatient

Test medical necessity documentation and utilization review considerations.

### Scenario 3 — Pneumonia + Observation

Test observation-specific notification and workflow requirements.

### Scenario 4 — Elective Surgery + Same-Day Surgery

Test planned admission preparation.

### Scenario 5 — Hip Fracture + Emergency

Test urgent admission workflow and rapid coordination.

### PA Testing

Test:

- Approved
- Pending
- Denied
- Successful Appeal

---

## 🛠️ Technology Stack

- **HTML5**
- **Tailwind CSS CDN**
- **Vanilla JavaScript**
- No framework
- No build process
- Single self-contained HTML file

The application is designed to run directly in a modern web browser.

---

