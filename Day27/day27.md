# Prior Authorization Story Simulator — Day 27

An interactive, story-driven healthcare education simulator that explains the Prior Authorization (PA) process through Rahul's healthcare journey.

## Overview

The Prior Authorization Story Simulator transforms a complex healthcare administrative workflow into an interactive eight-scene story.

Users follow Rahul, a patient diagnosed with Rheumatoid Arthritis, while Priya, a healthcare operations specialist, explains each stage of the Prior Authorization process in beginner-friendly language.

StarCare Health is used only as an illustrative example payer for educational purposes.

## Story Chapters

### 1. Doctor Visit
Rahul visits City Medical Center. Dr. Patel diagnoses him with Rheumatoid Arthritis and prescribes Humira.

### 2. Insurance Roadblock
Dr. Patel's office submits the Prior Authorization directly to StarCare Health.

Workflow:

Provider → PA Request → Payer

No pharmacy is involved in this illustrative workflow. Once approved, the PA is saved on file.

### 3. What Is Prior Authorization?
Priya explains PA in plain language.

The story explains that step therapy is not simply bureaucracy because, for aggressive diagnoses, treatment delays can potentially affect disease progression.

The simulator references the AMA 2023 Prior Authorization Physician Survey regarding treatment delays.

### 4. Insurance Review
Priya explains what StarCare Health checks:

- Eligibility
- Clinical documentation
- ICD-10 diagnosis match
- Step therapy history

Each requirement is explained in beginner-friendly language.

### 5. Denial
The PA is denied because step therapy documentation is missing.

The simulator emphasizes:

Denial ≠ Permanent

Priya explains that additional documentation or an appeal may be possible depending on the applicable process.

The system-side explanation includes the scenario statement that PA denials can require 2+ staff hours for physician offices to resolve.

### 6. Appeal
Rahul's healthcare team gathers:

- Supporting documents
- Letter of Medical Necessity
- Clinical justification
- Formal appeal submission

### 7. Approval
The appeal succeeds.

The PA is approved by StarCare Health. A reference number is issued and the approval is saved on file.

Within this scenario, no repeat PA is needed for Humira.

### 8. Takeaways

Patient Perspective:

- What PA means
- Why insurance reviews treatment
- Why documentation matters
- What denial means
- How appeals work
- How PA can affect treatment timelines

System Perspective:

- Denial rate
- Appeal rate
- Resolution time
- Administrative workload

## Key Features

- Interactive eight-scene healthcare story
- Rahul displayed on the left
- Priya displayed on the right
- Doctors and narrators displayed as centered italic text
- Two choices after every scene
- Choice-dependent dialogue
- Append-only chat feed
- Dynamic chat bubbles
- Progress bar
- Restart functionality
- Alternative dialogue paths
- Beginner-friendly healthcare explanations
- Responsive healthcare education design
- Single-file HTML application

## Technical Implementation

The application is built using:

- HTML5
- Tailwind CSS CDN
- Vanilla JavaScript

No framework or build step is required.

Every new chat bubble must be created using:

document.createElement()

and added using:

appendChild()

The chat container must never use:

innerHTML =

This ensures that the conversation feed remains append-only.

## PA Workflow

Doctor Visit
↓
Diagnosis
↓
Prescription
↓
PA Request
↓
Payer Review
↓
Eligibility Check
↓
Clinical Documentation
↓
ICD-10 Diagnosis Match
↓
Step Therapy Review
↓
Denial
↓
Appeal
↓
Approval
↓
Treatment Progression

## Project Structure

Day27/
│
├── prior-authorization-story-simulator.html
├── day27.md

## Learning Outcomes

After completing the simulator, users should understand:

1. What Prior Authorization is.
2. Why providers submit PA requests.
3. How provider-to-payer PA workflows work.
4. Why insurance eligibility is checked.
5. Why clinical documentation matters.
6. What ICD-10 diagnosis matching means.
7. What step therapy means.
8. Why missing documentation can cause a denial.
9. Why denial does not necessarily mean the end of the process.
10. What an appeal involves.
11. What a Letter of Medical Necessity is.
12. How a PA can ultimately be approved.
13. Why approval reference numbers matter.
14. How patients experience PA.
15. How healthcare organizations track PA performance.

## Healthcare Operations Metrics

### Denial Rate

Denied Requests / Total Requests × 100

### Appeal Rate

Appealed Cases / Denied Cases × 100

### Resolution Time

The amount of time required to resolve a Prior Authorization issue.

These metrics help healthcare organizations understand administrative workload and process performance.

## Design System

The application follows a beginner-friendly healthcare education design system.

Design principles:

- Clean healthcare interface
- Patient-centered storytelling
- Clear visual hierarchy
- Beginner-friendly language
- Distinct patient and specialist perspectives
- Interactive dialogue
- Progressive navigation
- Visible progress tracking
- Responsive layout
- Educational focus

## Character Design

### Rahul

Role: Patient

Position: Left

Rahul represents the patient perspective and asks questions that help users understand the PA process.

### Priya

Role: Healthcare Operations Specialist

Position: Right

Priya explains PA, insurance review, documentation, step therapy, denials, appeals, approvals, and healthcare system metrics.

### Doctors and Narrators

Doctors and narrators appear only as centered italic text and never as chat bubbles.

## Interactive Mechanics

After every scene, the user receives two choices.

Example:

Choice 1: Ask Priya why the PA is required.

Choice 2: Ask what happens if the PA is denied.

The selected choice changes the following dialogue.

After completing the story, users can restart it and explore another dialogue path.

## Progress Bar

The simulator tracks progress across all eight chapters:

1 → 2 → 3 → 4 → 5 → 6 → 7 → 8

The progress bar updates as the user advances.

## Testing Checklist

- [ ] Application loads correctly
- [ ] Landing screen works
- [ ] Rahul appears on the left
- [ ] Priya appears on the right
- [ ] Doctors/narrators appear as centered italic text
- [ ] Chat bubbles are dynamically created
- [ ] Chat container does not use innerHTML
- [ ] Two choices appear after every scene
- [ ] Choices work correctly
- [ ] Progress bar updates
- [ ] Scene 1 works
- [ ] Scene 2 works
- [ ] Scene 3 works
- [ ] Scene 4 works
- [ ] Scene 5 works
- [ ] Scene 6 works
- [ ] Scene 7 works
- [ ] Scene 8 works
- [ ] Final takeaways appear
- [ ] Restart works
- [ ] Alternative dialogue paths work
- [ ] Desktop layout works
- [ ] Mobile layout works
- [ ] Single HTML file works

## Screenshots

Important screenshots should cover:

- Home screen
- Doctor visit
- Insurance roadblock
- What is PA explanation
- Insurance review
- Denial
- Appeal
- Approval
- Final takeaways
- Alternative dialogue path

Store screenshots inside the screenshots/ folder.

## Day 27 Learnings

### Prior Authorization Is a Workflow

PA involves multiple participants and multiple steps rather than being just a form.

### Documentation Matters

Missing information can result in a denial and may require additional work to resolve.

### Denial Is Not Always Permanent

Depending on the situation and applicable process, additional documentation or an appeal may provide a path toward resolution.

### Appeals Require Operational Effort

Appeals can involve documentation, coordination, clinical information, and staff time.

### Patient and System Perspectives Differ

Patients experience PA primarily through treatment access and possible delays.

Healthcare organizations also monitor PA through denial rates, appeal rates, resolution times, and administrative workload.

### Interactive Storytelling Improves Understanding

Converting a complex healthcare workflow into a patient story makes the process easier for beginners to understand.

### Interactive Choices Improve Engagement

Two choices after every scene encourage users to explore different dialogue paths.

## How to Run

1. Open prior-authorization-story-simulator.html.
2. Use a modern web browser.
3. Start the interactive story.
4. Follow Rahul's healthcare journey.
5. Read Priya's explanations.
6. Select one of the two choices after every scene.
7. Complete all eight chapters.
8. Review the final takeaways.
9. Restart the story.
10. Explore a different dialogue path.

## Disclaimer

This project is an educational simulation and does not provide medical or insurance advice.

Rahul and Priya are fictional characters.

StarCare Health is an illustrative example used only for this simulator and does not represent an actual insurance company or real insurance case.

The simulator should not be used to make real medical, insurance, or treatment decisions.

## Reference

The simulator references the AMA 2023 Prior Authorization Physician Survey to explain the potential treatment delays and administrative burden associated with Prior Authorization.

For real-world healthcare decisions, users should consult qualified professionals and current official payer policies.

## Future Improvements

Potential future enhancements include:

- Multiple patient scenarios
- Different diagnoses
- Pharmacy benefit workflows
- Electronic Prior Authorization
- Realistic payer policy variations
- Denial reason analytics
- Appeal success-rate simulation
- Healthcare operations dashboard
- Real-time KPI visualization
- Accessibility improvements
- Screen-reader optimization
- More branching story paths
- Scenario comparison
- Learning progress tracking
- Exportable learning reports

## Day 27 Challenge

60 Days of Claude Challenge — Day 27

Project: Prior Authorization Story Simulator

Focus:

Healthcare × Interactive Storytelling × Web Development × Education × Healthcare Operations

## Final Outcome

The Prior Authorization Story Simulator transforms a complex healthcare administrative process into an interactive patient journey.

Doctor Visit → PA Request → Insurance Review → Denial → Appeal → Approval → Final Takeaways

This project demonstrates how interactive web development and storytelling can make complex healthcare workflows easier to understand.
