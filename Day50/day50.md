# 🛡️ Defend Your Experience

> An adaptive AI interview simulator that challenges users to confidently defend every claim they make about their experience.

## 🚀 Overview

**Defend Your Experience** is an interactive AI-powered interview preparation application designed to test how well you can defend your own experience.

Instead of simply reviewing a resume or asking generic interview questions, the application extracts meaningful claims from your uploaded material and turns them into personalized interview challenges.

The AI acts as a **skeptical interviewer** — asking deeper follow-up questions based on your previous answers, identifying vague claims, questioning missing evidence, and helping you build stronger, more confident responses.

### 🎯 Core Objective

The goal is **not to improve your resume**.

The goal is to help you confidently answer:

> **"You said you did this. Now prove it."**

## ✨ Key Features

- 🤖 **Adaptive AI Interviewer**
  - Generates personalized questions from the user's own experience.
  - Continuously adapts based on previous answers.
  - Creates deeper follow-up questions instead of using a fixed questionnaire.

- 🧠 **Claim-Based Defense**
  - Identifies meaningful claims from uploaded documents.
  - Challenges vague, exaggerated, or unsupported statements.
  - Tests whether the user can explain their actual contribution.

- 🔍 **Intelligent Follow-Ups**
  - Every answer influences the next question.
  - Explores decisions, challenges, outcomes, tools, metrics, and ownership.
  - Simulates realistic interviewer pressure.

- 📊 **Defense Progress Tracking**
  - Tracks interview progress.
  - Displays confidence indicators.
  - Visualizes defended vs. weak experiences.

- 📋 **Final Defense Report**
  - Shows well-defended experiences.
  - Highlights claims that need improvement.
  - Identifies weak evidence and vague explanations.
  - Provides actionable recommendations.

- 📁 **Drag & Drop Uploads**
  - Upload resumes, portfolios, project documents, bios, research, performance reviews, and other experience documents.

- 💾 **Local Session History**
  - Saves interview sessions locally.
  - Allows users to revisit previous practice sessions.

- 📤 **Export Support**
  - Export interview results and Defense Reports for future preparation.

- 📱 **Responsive Design**
  - Optimized for desktop, tablet, and mobile screens.

- ⚡ **Graceful API Error Handling**
  - Handles temporary API failures and rate limits.
  - Provides fallback states instead of breaking the experience.

- 🎨 **Premium Interactive UI**
  - Modern interview dashboard.
  - Progress visualization.
  - Confidence indicators.
  - Interactive cards and transitions.
  - Clear empty states and onboarding.

## 🧩 How It Works

### 1️⃣ Upload Your Experience

Upload a document containing your experience, such as:

- Resume
- LinkedIn profile
- Portfolio
- Project description
- Research paper
- Startup story
- Freelance work
- Performance review
- Professional bio

### 2️⃣ Extract Claims

The application identifies meaningful statements such as:

- Technologies used
- Projects completed
- Responsibilities
- Achievements
- Metrics
- Leadership experiences
- Problem-solving experiences
- Business impact
- Research contributions

### 3️⃣ Start the Defense

The AI interviewer challenges one claim at a time.

Example:

> **Claim:** "Built an AI-powered recommendation system."

The interviewer may ask:

> "What exactly did you build yourself, and what parts were handled by existing libraries or APIs?"

### 4️⃣ Go Deeper

Your answer determines what comes next.

The AI can challenge:

- Why you chose a specific approach
- Your exact contribution
- Technical decisions
- Problems encountered
- Alternative solutions
- Results and metrics
- Failure points
- Trade-offs
- Real-world impact

### 5️⃣ Receive Your Defense Report

At the end of the session, the application analyzes your performance and identifies:

**🟢 Strongly Defended**
  
Claims you explained clearly with specific evidence.

**🟡 Needs More Evidence**
  
Claims where your explanation was partially convincing.

**🔴 Weakly Defended**
  
Claims that were vague, unsupported, or difficult to explain.

## 🛠️ Technology Stack

- **HTML5**
- **CSS3**
- **JavaScript**
- **Anthropic Messages API**
- **LocalStorage**
- **File APIs**
- **Responsive UI**
- **Drag & Drop API**

## 🤖 AI Architecture

The application uses the **Anthropic Messages API directly from the HTML application**.

No custom backend is required.

The AI is responsible for:

1. Understanding uploaded experience.
2. Extracting meaningful claims.
3. Generating personalized interview questions.
4. Evaluating responses.
5. Selecting intelligent follow-ups.
6. Identifying weak evidence.
7. Tracking defense quality.
8. Generating the final Defense Report.

The application is designed to run inside an **Anthropic HTML artifact environment**, where authentication is handled automatically.

## 🔐 Privacy

User sessions and history can be stored locally using browser **LocalStorage**.

The application does not require users to manually enter an API key.

## 📈 Defense Metrics

The interface can track metrics such as:

| Metric | Purpose |
|---|---|
| Defense Score | Overall ability to defend experience |
| Confidence | Self-reported / AI-estimated confidence |
| Claims Defended | Successfully explained claims |
| Weak Claims | Claims requiring more preparation |
| Evidence Strength | Specificity and credibility of answers |
| Follow-up Depth | How deeply the user handled questioning |

## 🎨 User Experience

The application follows a premium interview-dashboard experience with:

- Clear onboarding
- Interactive interview cards
- Dynamic progress indicators
- Confidence visualization
- Claim-level status indicators
- Adaptive questioning
- Session history
- Final report dashboard
- Responsive layouts
- Helpful empty states
- Error recovery states

## 📂 Suggested Project Structure

```text
defend-your-experience/
│
├── index.html
└── README.md
``` 
## 🔮 Future Enhancements

🎙️ Voice-based mock interviews
⏱️ Real-time interview pressure mode
👔 Interviewer personality presets
🏢 Company-specific interview simulations
📚 Topic-wise defense practice
📊 Advanced performance analytics
🔁 Spaced-repetition practice for weak claims
🧑‍💼 Technical and HR interview modes
📝 AI-generated answer improvement suggestions
🏆 Multi-session performance trends

## 👨‍💻 Built With

HTML • CSS • JavaScript • Anthropic AI • LocalStorage

## Author 
Neha Duggal 
