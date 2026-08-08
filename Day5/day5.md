# Day 5: Context Engineering (Prompt Engineering Series)

> **Core Concept:** Better context yields better outputs. Large language models (LLMs) perform significantly better when provided with specific parameters regarding the user's situation, skill set, and constraints.

---

## 1. Prompt A (Without Context)

### **Prompt**
Create a 30-day learning roadmap.

Include:
- Weekly milestones
- Daily tasks
- Resources
- Projects
- Final outcome

Make it practical and beginner-friendly.

---

### **Output Received**
# 30-Day Beginner Web Development Learning Roadmap

## Weekly Milestones
- Week 1: HTML & CSS Fundamentals
- Week 2: Responsive Design & CSS Frameworks
- Week 3: JavaScript Basics
- Week 4: Final Project & Portfolio Integration

## Daily Tasks
- Days 1–5: Learn basic HTML tags, links, images, and semantic structure.
- Days 6–10: Build a basic single-page landing page using HTML/CSS.
- Days 11–15: Learn Flexbox and CSS Grid.
- Days 16–20: Introduction to JavaScript variables, loops, and DOM manipulation.
- Days 21–25: Build an interactive To-Do List app.
- Days 26–30: Polish portfolio and deploy on GitHub Pages.

## Resources
- MDN Web Docs
- freeCodeCamp
- YouTube tutorials (Traversy Media, Net Ninja)

## Final Outcome
A deployed personal portfolio website showcasing 2 basic projects.

---

## 2. Prompt B (With Context)

### **Prompt (Filled with Context)**
Create a 30-day learning roadmap.

Context:
- Current Situation: Computer Science Student / Aspirant
- Current Skills: Python basics, HTML/CSS
- Goal: Become an AI Engineer (Focus on LLM Integration & RAG)
- Available Time: 2-3 Hours per Day
- Experience Level: Beginner in AI/ML
- Preferred Learning Style: Project-based with documentation & short tutorials

Include:
- Weekly milestones
- Daily tasks
- Resources
- Projects
- Final outcome

Make it practical and beginner-friendly.

---

### **Output Received**
# 30-Day AI Engineering Roadmap (2-3 Hours/Day)

## Weekly Milestones
- Week 1: Python for AI & API Integration (OpenAI / Anthropic APIs)
- Week 2: Prompt Engineering, Structured Outputs & Chains (LangChain/LlamaIndex)
- Week 3: Vector Databases & Retrieval-Augmented Generation (RAG)
- Week 4: End-to-End AI Application Project & Deployment

## Daily Breakdown
- Day 1-3: Advanced Python Refresher (Async, Type Hinting, Pydantic) + Setting up OpenAI/Gemini API Keys.
- Day 4-7: Making raw API calls, system prompts, temperature tuning, and JSON mode outputs.
- Day 8-11: Working with LangChain/LlamaIndex basics, prompt templates, and output parsers.
- Day 12-14: Build Project 1: Command-line AI Summarizer & Extractor.
- Day 15-18: Understanding Embeddings, Chunking Strategies, and Vector DBs (ChromaDB / Pinecone).
- Day 19-21: Implementing RAG (Retrieval-Augmented Generation) on custom PDF documentation.
- Day 22-25: Build Project 2: Full-stack RAG Chatbot using Streamlit/FastAPI + Vector DB.
- Day 26-28: Evaluation, handling rate limits, error handling, and guardrails.
- Day 29-30: Refactoring code, creating GitHub documentation, and deploying on Streamlit Community Cloud / Vercel.

## Resources
- DeepLearning.AI Short Courses (LangChain & RAG)
- Official OpenAI / Anthropic Cookbook
- Pinecone / ChromaDB Documentation
- Streamlit Docs

## Final Outcome
A fully functional, deployed RAG-based AI application connected to custom documents, published on GitHub with complete documentation.

---

## 3. Comparative Analysis

### 1. Which roadmap feels more personalized?
**Prompt B** is significantly more personalized. Prompt A defaulted to a completely unrelated web development track because no topic was specified. Prompt B targeted the specific goal of **AI Engineering**, respected my existing **Python baseline**, and designed daily tasks specifically tailored to building **LLM and RAG applications** within my available daily hours.

### 2. Which roadmap would you actually follow?
I would follow **Prompt B**. Prompt A gave a generic HTML/CSS roadmap that doesn't align with my career path. Prompt B provides a structured, modern 30-day plan focusing on practical AI engineering tools (APIs, Vector DBs, RAG) with clear project deliverables.

### 3. What role did context play in improving the result?
Context played three crucial roles:
1. **Targeted Domain Alignment:** Specifying AI Engineering redirected the output from basic frontend development to modern LLM application development.
2. **Efficiency & Skill Alignment:** Stating prior Python knowledge meant the roadmap skipped introductory coding and moved straight into AI API integration.
3. **Actionable Scope:** Defining 2-3 hours per day ensured the daily deliverables were realistic, actionable, and project-driven rather than purely theoretical.

---

## Key Takeaways
- Zero-context prompts force LLMs to guess intent, often yielding generic or irrelevant results.
- Context Engineering pins down precise parameters (target outcome, skill level, hours available) to produce an immediate, tailored, and execution-ready plan.
