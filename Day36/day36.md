# 🧠 Cognitive Pattern Explorer

> A calm, interactive, psychology-inspired self-reflection experience built entirely with **HTML, CSS, and Vanilla JavaScript**.

Cognitive Pattern Explorer helps users explore how they approach everyday decisions, priorities, and thoughts through interactive scenarios.

It is designed to feel like a **calm exploration game rather than a psychological test**.

---

## ✨ Features

### 🌿 Calm / Stress Mode

Switch between two visual reflection environments:

* ☁️ Calm Mode
* ◐ Stress Mode

The interface subtly changes its visual atmosphere while keeping the experience accessible and distraction-free.

### 🧩 Chapter 1 — Discover Your Thinking Style

Users respond to everyday scenarios and explore five thinking tendencies:

* 🔎 **Analytical Thinker**
* 💭 **Emotional Intuitive**
* 🔁 **Overthinking Loop Style**
* ⚡ **Action-First Decision Maker**
* ⚖️ **Balanced Reflective Thinker**

Responses contribute to a reflective score rather than producing a clinical or psychological diagnosis.

---

### 🎯 Chapter 2 — Choose Your Priorities

Users arrange priority cards using interactive drag-and-drop.

The activity encourages users to notice:

* What attracts their attention first
* What they consider important
* How they naturally organize competing priorities

The component supports:

* Native desktop drag-and-drop
* Touch-friendly interaction
* Responsive layouts

---

### 🗺️ Chapter 3 — Map Your Thinking

Thought cards can be placed across four reflective areas:

```text
PAST → PRESENT → FUTURE → ACTION
```

This helps users notice whether their thinking naturally focuses more on:

* Previous experiences
* Current situations
* Possible outcomes
* Immediate action

---

### 📔 Final Reflection Journal

The final screen provides:

* Personalized reflective insight
* Primary emerging thinking tendency
* Percentage breakdown
* Visual score bars
* Personal reflection journal
* Save reflection functionality
* Restart / explore again option

---

## 🎨 Design Philosophy

The interface follows a calm, modern aesthetic with:

* Soft colors
* Rounded cards
* Subtle shadows
* Ambient background animations
* Smooth transitions
* Minimal visual clutter
* Responsive layouts
* Accessible controls

The goal is to make self-reflection feel **safe, exploratory, and engaging**.

---

## 🧠 Thinking Tendencies

The application uses five educational reflection categories.

| Tendency                       | Reflective Description                                                              |
| ------------------------------ | ----------------------------------------------------------------------------------- |
| 🔎 Analytical Thinker          | You often prefer facts, structure, evidence, and logical comparison.                |
| 💭 Emotional Intuitive         | You often pay attention to feelings, context, relationships, and emotional signals. |
| 🔁 Overthinking Loop Style     | You may spend more time exploring possibilities, meanings, and potential outcomes.  |
| ⚡ Action-First Decision Maker  | You often prefer taking a reasonable first step and adjusting along the way.        |
| ⚖️ Balanced Reflective Thinker | You often combine analysis, intuition, reflection, and action.                      |

These are **reflection categories, not personality diagnoses**.

---

## 🛠️ Technology

The project intentionally uses only browser-native technologies.

```text
HTML5
CSS3
Vanilla JavaScript
Native Drag & Drop API
Local Browser Storage
```

### No Frameworks

The application does **not** require:

* React
* Vue
* Angular
* Tailwind
* Bootstrap
* Node.js
* npm
* Backend
* Database
* API
* External libraries

---

## 📁 Project Structure

The complete application is contained inside one HTML file:

```text
Cognitive-Pattern-Explorer/
│
└── index.html
```

HTML, CSS, and JavaScript are all included in the same file.

---

## 🚀 How to Run

No installation is required.

### Option 1 — Open Directly

Download or clone the repository and open:

```text
index.html
```

in any modern browser.

### Option 2 — GitHub Pages

1. Push the project to GitHub.
2. Open **Settings**.
3. Select **Pages**.
4. Choose the main branch.
5. Select the root folder.
6. Save.

The application can then be accessed through GitHub Pages.

---

## 📱 Responsive Design

The interface adapts to:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📟 Tablet

The priority and timeline interactions also adapt for smaller screens.

---

## ♿ Accessibility

Accessibility considerations include:

* Keyboard-focusable controls
* Visible focus states
* Semantic HTML
* ARIA labels where useful
* Keyboard-friendly buttons
* Touch-friendly interaction
* Reduced-motion support

The application respects:

```css
prefers-reduced-motion: reduce
```

so users who prefer less animation receive a simplified experience.

---

## 🎮 Interaction Flow

```text
START
  │
  ▼
Calm / Stress Mode
  │
  ▼
Chapter 1
Discover Your Thinking Style
  │
  ▼
Scenario Choices
  │
  ▼
Chapter 2
Choose Your Priorities
  │
  ▼
Drag & Drop
  │
  ▼
Chapter 3
Map Your Thinking
  │
  ▼
Timeline Interaction
  │
  ▼
Final Reflection
  │
  ├── Thinking Style
  ├── Percentage Breakdown
  ├── Personalized Insight
  └── Reflection Journal
```

---

## 🔐 Privacy

The application is designed to work completely offline.

No external:

* APIs
* Servers
* Analytics
* Tracking services
* Authentication
* Databases

are required.

Your reflection remains inside the browser unless you manually copy or share it.

---

## ⚠️ Educational Disclaimer

**Cognitive Pattern Explorer is an educational self-reflection experience.**

It does **not**:

* Diagnose mental health conditions
* Perform clinical assessments
* Replace professional psychological support
* Determine a user's fixed personality
* Provide medical advice

The results should be treated as prompts for personal reflection rather than definitive conclusions.

---

## 🔧 Customization

The application can easily be extended by modifying the JavaScript scenario objects.

Example:

```javascript
const scenarios = [
  {
    text: "Your scenario goes here...",
    options: [
      {
        title: "Option A",
        desc: "Description...",
        weights: {
          analytical: 3
        }
      }
    ]
  }
];
```

This makes it easy to add new scenarios without changing the overall application architecture.

---

## 💡 Future Improvements

Possible future additions include:

* More interactive scenarios
* Additional reflection chapters
* Custom scenario creation
* Reflection history
* Export reflection as PDF
* More visual themes
* Dark mode
* More advanced accessibility controls
* Animated thinking-pattern visualization
* Progress history
* Shareable reflection cards

---

## 🎯 Learning Objectives

This project demonstrates practical frontend concepts including:

* DOM manipulation
* JavaScript state management
* Event handling
* Dynamic UI rendering
* Scoring systems
* Native drag-and-drop
* Touch interaction
* Responsive CSS
* CSS animations
* Accessibility
* Browser storage
* Component-style reusable JavaScript functions

---

## 📜 License

This project is intended for educational and personal learning purposes.

You are free to modify and extend the project for your own learning and portfolio experiments.

---

## ⭐ Project Concept

**Cognitive Pattern Explorer**

> *Don't label the way you think.
> Notice it. Explore it. Understand it.*

Made with ❤️ using **HTML + CSS + Vanilla JavaScript**.

## Author
Neha Duggal 
