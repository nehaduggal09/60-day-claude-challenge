# 🤖 Autonomous Agent Studio

A production-style, single-page **multi-agent AI orchestration dashboard** that demonstrates how autonomous agents can plan, execute, evaluate, critique, improve, remember, and repeat until a runtime stopping condition is reached.

## 🚀 Overview

**Autonomous Agent Studio** is a vanilla HTML/CSS/JavaScript application designed to simulate a real autonomous multi-agent workflow powered by the **Claude API**.

The system dynamically orchestrates specialized agents and maintains state across iterative rounds instead of following a fixed sequence.

### Core Capabilities

* 🧠 Multi-agent orchestration
* 🔄 Real iterative evaluation loop
* 📊 Live evaluation and scoring
* 📝 Critique and improvement cycles
* 💾 Persistent round history and memory
* 🛡️ Safety monitoring
* 🔍 Final review after stopping
* 📈 Round-over-round improvement tracking
* ⚡ Retry and failure recovery
* 🌙 Responsive dark-mode interface
* 🎨 Production-style dashboard UI

---

## 🧩 Agent Architecture

The application can dynamically use the following specialized agents:

| Agent                  | Responsibility                                                                 |
| ---------------------- | ------------------------------------------------------------------------------ |
| 🗺️ **Planner**        | Breaks the objective into actionable tasks and defines the execution strategy. |
| ⚙️ **Executor**        | Produces the current solution/draft according to the plan.                     |
| 📊 **Evaluator**       | Evaluates the current draft against the selected success criteria and rubric.  |
| 🔎 **Critic**          | Identifies weaknesses, gaps, risks, and areas requiring improvement.           |
| ✨ **Improver**         | Uses the previous evaluation and critique to produce an improved draft.        |
| 🧠 **Memory Manager**  | Maintains useful information and state across iterations.                      |
| 🛡️ **Safety Monitor** | Checks the workflow for safety, reliability, and constraint violations.        |
| ✅ **Final Reviewer**   | Performs the final review once a stopping condition is triggered.              |

---

## 🔄 Autonomous Iteration Loop

The core workflow is intentionally open-ended:

```text
                ┌──────────────┐
                │    Planner   │
                └──────┬───────┘
                       ↓
                ┌──────────────┐
                │   Executor   │
                └──────┬───────┘
                       ↓
                ┌──────────────┐
                │  Evaluator   │
                └──────┬───────┘
                       ↓
                ┌──────────────┐
                │    Critic    │
                └──────┬───────┘
                       ↓
                ┌──────────────┐
                │   Improver   │
                └──────┬───────┘
                       │
                       └───────────────┐
                                       ↓
                                  Evaluator
                                       │
                              ┌────────┴────────┐
                              │ Stop Condition? │
                              └────────┬────────┘
                                       │ Yes
                                       ↓
                              ┌─────────────────┐
                              │ Final Reviewer  │
                              └─────────────────┘
```

The **Improver → Evaluator** connection creates the actual runtime loop.

There is **no predetermined number of successful rounds**.

---

## 🛑 Stop Conditions

Every iteration checks stopping conditions in the following order:

### 1. Plateau Detection

Stops when the evaluation score improves by less than a small delta for **two consecutive rounds**.

### 2. Target Threshold

Stops when the model-generated evaluation score crosses the target defined during the interview.

### 3. Hard Iteration Cap

A safety fallback prevents an unexpected workflow from running indefinitely.

The hard cap is a **safety mechanism**, not the intended workflow ending.

The dashboard displays the exact condition that terminated execution.

---

## 🧠 State Threading

The system maintains a running history of previous iterations.

Each round records:

```text
Score
Critique
Draft
Delta
Evaluation
Memory Updates
Agent Outputs
```

The state flows forward:

```text
Previous Evaluation
        +
Previous Critique
        ↓
    Improver
        ↓
 Improved Draft
        ↓
    Evaluator
        ↓
 New Evaluation
```

This allows the system to progressively improve the current draft rather than restarting every round.

---

## 🖥️ Dashboard

The interface provides a live operational view of the autonomous system.

### Dashboard Components

* 🔄 Workflow visualization
* 🤖 Active agent indicator
* 🟢 Live execution status
* 🔢 Open-ended round indicator
* 📜 Activity log
* 📊 Iteration history
* 🧾 Intermediate agent outputs
* 🧠 Memory updates
* 📈 Evaluation reports
* ↕️ Round-over-round deltas
* 🔁 Retry count
* 🛑 Stop-condition status
* 🏁 Final summary
* ⚡ Execution statistics
* 🤝 Agent performance summary

The round indicator intentionally uses an open-ended format such as:

> **Round 3 — checking stop condition…**

instead of displaying a predetermined sequence such as:

> Round 3 of 5

---

## 💬 Interview-First Workflow

Before execution, the application conducts an interactive interview.

Questions are asked **one at a time in MCQ format**.

### Interview Flow

1. **Agent Type**

   * Select the autonomous AI agent use case.

2. **Workflow Narrowing**

   * Ask progressively specific questions until the task is sufficiently defined for automation.

3. **Success Criteria**

   * Define how success should be evaluated.

4. **Stopping Condition**

   * Select the appropriate runtime termination criteria.

5. **Agent Configuration**

   * Choose automatic agent selection or customize the agent components.

Free-text input is available only through the final **Other** option where applicable.

---

## 🔌 Claude API Integration

The application is designed to communicate directly with the Claude Messages API using:

```text
https://api.anthropic.com/v1/messages
```

API requests are made using native browser `fetch()`.

Each important agent action is represented by a live model call rather than simulated or hardcoded output.

> ⚠️ **Important:** Calling a commercial API directly from a browser normally requires appropriate authentication and secure API-key handling. A production deployment should use a backend/proxy layer rather than exposing credentials in client-side JavaScript.

---

## 🛠️ Technology Stack

### Frontend

* HTML5
* CSS3
* Vanilla JavaScript

### No External Libraries

The project intentionally avoids:

* React
* Vue
* Angular
* Tailwind
* Bootstrap
* Chart.js
* Other external frontend libraries

Everything is contained inside a single HTML file.

---

## 📁 Project Structure

```text
autonomous-agent-studio/
│
└── README.md
```

The application is designed to run as a standalone HTML file.

---

## ⚙️ Execution Flow

```text
User Interview
      ↓
Workflow Definition
      ↓
Agent Selection
      ↓
Planner
      ↓
Executor
      ↓
Evaluator
      ↓
Critic
      ↓
Improver
      ↓
Stop Check
      │
      ├── Continue → Evaluator
      │
      └── Stop → Final Reviewer
                    ↓
              Final Summary
```

---

## 📊 Runtime Statistics

The dashboard can surface execution metrics such as:

* Total rounds executed
* Successful API calls
* Retry count
* Evaluation progression
* Score deltas
* Agent activity
* Execution status
* Final stopping condition
* Final review status

---

## 🔐 Reliability & Error Handling

The application includes defensive handling for runtime failures.

Expected recovery mechanisms include:

* API retry handling
* Loading states
* Error states
* Graceful workflow termination
* Retry counters
* Agent status updates
* Clear activity logging
* Final failure reporting

The UI should never silently fail when an agent call encounters an error.

---

## 🎯 Design Philosophy

Autonomous Agent Studio is built around five principles:

### 1. Real Iteration

The system should genuinely repeat model calls instead of displaying a precomputed sequence.

### 2. State Preservation

Every round builds upon information generated by previous rounds.

### 3. Model-Driven Evaluation

Evaluation, critique, and improvement outputs come from the model rather than hardcoded scoring rules.

### 4. Observable Autonomy

Users can inspect what each agent is doing while the workflow is running.

### 5. Controlled Autonomy

The system can continue improving while still having explicit stopping conditions and a safety fallback.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Open the application

Open:

```text
index.html
```

in a modern browser.

### 3. Configure API access

For actual Claude API execution, configure authentication through a secure architecture appropriate for your deployment.

---

## 🔮 Extension Ideas

Future versions could add:

* 🧩 Custom agent creation
* 🗃️ Persistent long-term memory
* 🔌 Tool calling
* 🌐 Web research agents
* 📁 File-aware agents
* 🧠 Agent-to-agent messaging
* 🔀 Parallel agent execution
* 🌳 Branching reasoning workflows
* 📡 Real-time streaming responses
* 🗂️ Workflow templates
* 💾 Exportable execution traces
* 📊 Advanced analytics
* 🔐 Backend authentication
* 👥 Multi-user workspaces
* 🧪 Automated benchmark evaluation
* 🧬 Dynamic agent spawning
* 🔁 Human-in-the-loop approval stages

---

## 🧠 Advanced Autonomous-System Prompts

The project can be extended with prompts such as:

```text
Build a hierarchical multi-agent system where a supervisor dynamically
creates and delegates tasks to specialized agents.
```

```text
Design an autonomous research system that searches multiple sources,
cross-checks evidence, identifies conflicts, and produces a cited report.
```

```text
Create a self-reflective coding agent that plans implementation,
writes code, tests it, diagnoses failures, and iteratively fixes the code.
```

```text
Build a multi-agent business analyst that converts an ambiguous business
problem into requirements, analysis, recommendations, and an implementation plan.
```

```text
Create an adaptive agent architecture where the system dynamically decides
which specialist agent should be invoked next based on the current state.
```

---

## 🏆 Final Output

**Autonomous Agent Studio** demonstrates a complete autonomous-agent architecture in a single-page frontend:

> **Plan → Execute → Evaluate → Critique → Improve → Remember → Repeat → Stop → Final Review**

The key architectural feature is the **runtime feedback loop**, where each iteration receives the previous state and performs fresh model-driven evaluation and improvement until a defined stopping condition is reached.

---

## 📌 Project Highlights

* ✅ Single self-contained HTML application
* ✅ Vanilla HTML/CSS/JavaScript
* ✅ Multi-agent architecture
* ✅ Live API orchestration
* ✅ Real iterative loop
* ✅ Runtime stopping conditions
* ✅ State threaded between rounds
* ✅ Evaluation history
* ✅ Memory management
* ✅ Retry and recovery handling
* ✅ Interactive workflow visualization
* ✅ Responsive commercial-style UI
* ✅ Final execution analytics
* ✅ Extensible autonomous-agent architecture

---

## 👨‍💻 Author
Neha Duggal 

Built as an exploration of **Agentic AI, autonomous workflows, multi-agent orchestration, prompt engineering, and AI-powered frontend systems**.
