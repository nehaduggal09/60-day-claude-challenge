# Day 3: Role-Based Prompting & Persona Analysis
## Overview
This repository contains the completed tasks for Day 3: Role-Based Prompting. In this exercise, we analyze how setting specific context and assigning distinct personas (e.g., Founder vs. Developer) alters the perspective, depth, tone, and strategic recommendations provided by Claude for the exact same underlying question.
---
## The Question Tested
Query: "How should we handle technical debt in a fast-scaling tech startup product?"
---
## 1. Experimentation & Prompts
### 1.1 Control Prompt (No Role Assigned)
* Prompt:
  How should we handle technical debt in a fast-scaling tech startup product?
* Output / Response:
  Handling technical debt in a scaling startup requires balancing speed and code quality. You should identify critical bottlenecks, maintain a backlog of refactoring tasks, dedicate a percentage of sprint time (15–20%) to technical improvements, and foster engineering discipline. Establish clear metrics for debt, such as test coverage and build stability, to ensure long-term sustainability without stopping feature velocity entirely.
---
### 1.2 Founder Persona
* Prompt:
  Act as a startup Founder and CEO. How should we handle technical debt in a fast-scaling tech startup product?
* Output / Response:
  As a Founder, technical debt is a strategic leverage tool—not just code hygiene. Early on, taking on technical debt allows you to validate market fit faster than competitors. However, as you scale:
  1. Assess Business Risk: Only fix debt that directly threatens uptime, churn, or revenue.
  2. Opportunity Cost: Weigh the cost of refactoring against missing key product milestones or feature launches.
  3. ROI-Driven Engineering: Ask the engineering team to quantify debt in terms of lost productivity or customer friction before approving major rewrites.
  4. Communication: Frame tech debt cleanup to investors and stakeholders as protecting customer retention and infrastructure scalability.
---
### 1.3 Developer Persona
* Prompt:
  Act as a Senior Lead Software Developer. How should we handle technical debt in a fast-scaling tech startup product?
* Output / Response:
  From an engineering perspective, unmanaged technical debt creates brittle systems and developer burnout. Here is how we tackle it systematically:
  1. Debt Registry & T-Shirt Sizing: Catalog debt into low, medium, and high complexity items in JIRA/GitHub Issues.
  2. Dedicated Sprint Capacity: Allocate 20% of every sprint exclusively to tech debt, dependency updates, and refactoring.
  3. Automated Guardrails: Implement rigid CI/CD pipelines, automated linting, unit testing, and static code analysis (e.g., SonarQube) to prevent new bad code from entering production.
  4. Strangler Fig Pattern: Incrementally rewrite legacy services rather than attempting massive, high-risk full rewrites.
---
## 2. Comparative Analysis

| Perspective | Control (No Persona) | Founder Persona | Developer Persona |
| :--- | :--- | :--- | :--- |
| Primary Objective | Balanced technical overview | Business continuity, speed-to-market, ROI | Maintainability, stability, developer velocity |
| Tone & Stance | Neutral, advisory | Strategic, risk-tolerant, high-level | Tactical, structured, hands-on engineering |
| Key Metrics | Sprint balance, code quality | Customer churn, uptime, feature delivery speed | Test coverage, build health, deployment frequency |
| Refactoring Strategy | Periodic cleanup | Fix only when blocking revenue or growth | Continuous 20% sprint allocation & CI/CD tools |

### Key Takeaways
1. Persona Precision: Assigning a specific role shifts Claude's reasoning framework from generic best practices to domain-tailored advice.
2. Founder Focus: Focuses heavily on trade-offs, opportunity costs, and ROI.
3. Developer Focus: Focuses on concrete workflows, toolchains, architectural patterns, and team execution.
---
## 3. Tool Exploration: Claude Usage Counter
- Installed the Claude Usage Counter browser extension.
- Checked the dashboard interface to track token usage, session rate limits, and daily prompt capacity.
- Interface allows real-time monitoring of API/interface limits during heavy prompting sessions.
---
## Submission Checklist
- [x] Read about Role-Based Prompting
- [x] Tested query without role
- [x] Tested query with Founder role
- [x] Tested query with Developer role
- [x] Documented persona comparison table
- [x] Installed and explored Claude Usage Counter
- [x] Created Day3 folder and day3.md file
- [x] Prepared full content for GitHub repository push
  
