# 🏥 Prior Authorization Workflow Simulator

> **Day 26 — 60 Days of Claude Challenge**

An interactive, gamified healthcare workflow simulator designed to demonstrate how the **US Prior Authorization (PA)** process works across patients, providers, and payers.

The application transforms a traditionally complex healthcare administrative process into an engaging **drag-and-drop learning experience**, allowing users to move patient cases through different stages of the prior authorization journey.

---

## 📌 Project Overview

Prior Authorization is a process used by health insurance companies to determine whether certain medical services, procedures, tests, medications, or hospital admissions meet predefined coverage and medical-necessity requirements.

This project simulates that workflow in an easy-to-understand visual environment.

Users can:

- Select different patient scenarios.
- Move cases through workflow stages.
- Evaluate medical necessity.
- Collect required documentation.
- Submit authorization requests.
- Simulate payer review.
- Handle approval, pend, denial, appeal, and peer-to-peer review.
- Track elapsed days.
- Monitor workflow efficiency.
- Learn what happens at every stage.
- Review a final workflow summary.

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Understand the basic Prior Authorization lifecycle.
2. Visualize responsibilities of patients, providers, and payers.
3. Learn why documentation is important in PA requests.
4. Understand medical necessity evaluation.
5. Simulate payer decision-making.
6. Demonstrate what happens after an approval or denial.
7. Understand the role of appeals and peer-to-peer reviews.
8. Gamify healthcare workflow education.
9. Build an interactive application without frameworks.
10. Practice frontend development using Vanilla JavaScript.

---

## ✨ Key Features

### 🧑 Patient Scenarios

The simulator includes multiple realistic healthcare scenarios:

- 🏥 Elective Surgery
- 🧠 MRI
- 💊 Specialty Medication
- 🚑 Inpatient Admission

Each scenario contains its own clinical context, requested service, diagnosis, insurance information, required documents, and potential workflow outcomes.

---

### 🛣️ Three Workflow Lanes

The workflow is divided into three major participants:

#### 🧑 Patient

Patient-related activities such as:

- Patient intake
- Clinical information
- Supporting information

#### 👨‍⚕️ Provider

Provider-related activities such as:

- Medical necessity evaluation
- Documentation collection
- Prior authorization request preparation
- Submission

#### 🏦 Payer

Payer-related activities such as:

- Request review
- Medical necessity determination
- Approval
- Pend
- Denial
- Appeal handling
- Peer-to-peer review

This structure helps users understand which participant is responsible for each stage.

---

## 🖱️ Drag-and-Drop Workflow

The application uses native HTML5 drag-and-drop functionality.

Users can:

1. Select a patient scenario.
2. Pick up the case card.
3. Drag it to the appropriate workflow stage.
4. Complete the stage.
5. Read the educational explanation.
6. Continue to the next stage.

The workflow is intentionally designed to feel like a game rather than a static educational diagram.

---

## 🧾 Prior Authorization Document Collection

The simulator includes an interactive document collection stage.

Depending on the scenario, users may need to collect documents such as:

- Patient demographics
- Insurance information
- Physician order
- Clinical notes
- Diagnosis documentation
- Imaging results
- Laboratory results
- Medication history
- Treatment history
- Conservative treatment documentation
- Supporting medical records

Users must collect the required documentation before submitting the authorization request.

The application visually tracks:

- Required documents
- Collected documents
- Remaining documents
- Submission readiness

---

## 🩺 Medical Necessity Evaluation

Medical necessity is an important part of Prior Authorization.

The simulator provides an educational step explaining that payers may evaluate information such as:

- Diagnosis
- Symptoms
- Clinical history
- Previous treatments
- Treatment response
- Physician recommendation
- Diagnostic findings
- Applicable coverage criteria
- Requested service or medication

The goal is not to make an actual medical determination, but to demonstrate how clinical information can influence the authorization workflow.

---

## 📤 Submission to Payer

Once the required documentation has been collected, users can submit the PA request.

The simulator validates whether the request is ready for submission.

This teaches an important workflow concept:

> A complete and well-supported request can reduce avoidable administrative delays.

---

## 🏦 Payer Review Outcomes

The simulator supports multiple payer outcomes.

### ✅ Approval

The requested service is approved.

The simulator displays:

- Approval status
- Educational explanation
- Celebration animation
- Updated workflow progress
- Final workflow summary

---

### ⏳ Pend

A payer may place a request on **pending** status when additional information or clarification is required.

The simulator explains why a request might be pended and allows the user to continue the workflow.

---

### ❌ Denial

A request can be denied for reasons such as:

- Insufficient documentation
- Medical-necessity concerns
- Coverage requirements
- Missing information
- Failure to meet applicable criteria

The simulator uses denial as an educational opportunity rather than simply ending the experience.

---

### 🔄 Appeal

After a denial, users can enter an appeal workflow.

The application demonstrates how additional supporting information may be used to challenge a decision.

---

### 👨‍⚕️ Peer-to-Peer Review

The simulator also demonstrates the concept of **peer-to-peer review**, where a treating clinician may discuss the case with an appropriate payer medical reviewer.

This helps users understand that certain authorization decisions can involve additional clinical review.

---

## 📊 Progress Tracker

A visual journey tracker is displayed across the top of the application.

It tracks the patient's movement through the PA workflow.

The tracker provides:

- Current stage
- Completed stages
- Remaining stages
- Overall progress
- Workflow position

This makes the entire authorization lifecycle easier to understand.

---

## 📅 Days Elapsed Counter

The application includes a simulated **Days Elapsed** counter.

As the case moves through the workflow, elapsed time is updated to demonstrate how administrative delays can accumulate.

This makes the simulator more realistic and helps users understand the importance of:

- Complete documentation
- Timely submission
- Prompt responses
- Efficient communication

---

## ⚡ Efficiency Score

The simulator includes an **Efficiency Score**.

The score represents how efficiently the user completes the workflow.

Actions that can influence efficiency include:

- Correct stage progression
- Complete documentation
- Avoiding unnecessary delays
- Responding appropriately to payer outcomes
- Completing the workflow efficiently

The score provides a gamified element and encourages users to learn the workflow while improving their performance.

---

## 📚 Educational Explanations

The simulator does not simply move the case forward.

After important workflow actions, users receive educational explanations describing:

- What happened
- Why the step matters
- Who is responsible
- What information is required
- What can cause delays
- What the next step is

This turns the application into an interactive educational tool.

---

## 🎉 Approval Celebration

When a case reaches approval, the simulator displays a celebration animation.

The purpose is to provide:

- Immediate feedback
- Gamification
- Visual confirmation
- Positive reinforcement

The approval state is also reflected in the final workflow summary.

---

## 📋 Workflow Summary

After completing a case, the application generates a workflow summary.

The summary can include:

- Patient scenario
- Requested service
- Final outcome
- Days elapsed
- Efficiency score
- Documents collected
- Workflow stages completed
- Educational conclusion

This gives users a complete overview of their simulated PA journey.

---

## 🔄 Restart / New Patient

The application supports two important controls:

### 🔄 Restart

Restarts the current patient scenario from the beginning.

### ➕ New Patient

Allows the user to select and simulate a different healthcare scenario.

This makes it possible to compare how different services can follow different authorization paths.

---

# 🛠️ Technology Stack

The application intentionally uses a simple frontend stack.

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | UI design, responsive layout, animations |
| Vanilla JavaScript | Workflow logic and interactions |
| HTML5 Drag & Drop API | Case movement |
| JavaScript Arrays/Objects | Scenario and workflow data |

### No frameworks were used.

The application does **not** require:

- React
- Vue
- Angular
- Bootstrap
- Tailwind
- Node.js
- npm
- Webpack
- Vite
- Backend server

---

# 📦 Technical Requirements

The application satisfies the following requirements:

- ✅ Single HTML file
- ✅ Self-contained
- ✅ HTML + CSS + Vanilla JavaScript
- ✅ No external dependencies
- ✅ No CDN
- ✅ No build step
- ✅ No backend
- ✅ No localStorage
- ✅ Workflow state stored in JavaScript memory
- ✅ Responsive design
- ✅ Drag-and-drop interaction
- ✅ Editable scenario data
- ✅ Fully functional controls

---
### 🚀 Future Improvements

Possible future versions could include:

👤 Multiple user roles
🏥 Provider dashboard
🏦 Payer dashboard
📊 Advanced analytics
📈 Workflow performance charts
⏱️ More detailed SLA simulation
🔔 Notification system
📄 PDF document simulation
🧾 Realistic authorization forms
🧠 More complex medical-necessity rules
🔄 Automated appeal workflows
💬 Provider-payer messaging
🏆 Leaderboards
⭐ Achievement badges
🎯 Difficulty levels
🧪 Additional healthcare scenarios
📱 Progressive Web App support
♿ Improved accessibility
🌐 Multi-language support
---
