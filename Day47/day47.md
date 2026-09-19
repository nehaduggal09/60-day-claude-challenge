# Content Intelligence Studio

AI-powered content analysis dashboard that acts as a virtual content consultant. It analyzes text and visual content using Claude and provides actionable insights for improving content quality, engagement, and platform performance.

## ✨ Features

- 🎯 One-question-at-a-time MCQ onboarding
- 📄 Text, image, screenshot, thumbnail, and transcript analysis
- 🤖 Dynamic multi-stage AI reviewer workflow
- 📊 Overall content health score
- 🔍 Detailed category-wise breakdown
- 💡 AI-generated strengths, weaknesses, and missed opportunities
- 📱 Platform-specific recommendations
- ✍️ Rewritten content variations
- 🪝 Alternative hooks and titles
- ✅ Publishing checklist
- ⚡ Live AI reviewer activity and status
- 🧠 AI reasoning behind recommendations
- 📋 Comprehensive final report
- 📈 AI-estimated performance potential
- 🔄 Before-vs-after comparison
- 🚀 Highest-impact improvement suggestions
- 💬 Further prompts for deeper optimization
- 🌙 Premium responsive dark-mode interface
- 🛡️ Loading states, retry handling, and graceful error recovery

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Claude Messages API
- Responsive UI
- No external libraries

## 🤖 AI Review Workflow

The application dynamically creates an intelligent review workflow based on the selected content type, platform, goal, and uploaded material.

Specialized AI reviewers can include:

- Content Strategist
- Platform Growth Specialist
- Audience Psychology Reviewer
- Hook & Headline Specialist
- Engagement Analyst
- Visual Content Reviewer
- Brand & Positioning Reviewer
- Conversion Reviewer
- Creator Coach
- Final Content Editor

All insights, scores, explanations, and recommendations are generated through live Claude API calls rather than hardcoded rules or canned feedback.

## 📊 Dashboard

The dashboard provides:

- Content Preview
- Overall Score
- Category Scores
- AI Reasoning
- Strengths
- Weaknesses
- Missed Opportunities
- Platform Recommendations
- Rewritten Versions
- Alternative Hooks
- Alternative Titles
- Publishing Checklist
- Reviewer Status
- Live Activity Log
- Executive Summary
- Content Health Report
- Highest-Impact Improvements
- AI Performance Potential Estimate
- Before-vs-After Comparison
- Further Optimization Prompts

## 🖼️ Visual Content Analysis

Users can upload screenshots, thumbnails, graphics, or other images. Claude analyzes the visual content directly and combines visual observations with the content strategy review.

## 🎨 UI/UX

Designed as a premium SaaS-style application with:

- Modern dark interface
- Responsive design
- Smooth animations
- Interactive visualizations
- Reviewer progress states
- Upload previews
- Score cards
- Mobile-friendly layouts
- Loading and error states
- Retry functionality

## 🚀 How It Works

1. Select the content type.
2. Select the target platform.
3. Select the primary goal.
4. Select the content you want to upload.
5. Select review criticality.
6. Upload or provide the content.
7. AI reviewers analyze the submitted content.
8. Review scores, reasoning, recommendations, rewrites, hooks, and titles.
9. Use the final executive summary and highest-impact improvements to optimize the content.

## ⚠️ API

The application communicates with the Claude Messages API:

`https://api.anthropic.com/v1/messages`

The application avoids placeholder analysis, hardcoded scoring, canned feedback, and rule-based evaluation. AI-generated insights are produced through live API calls.

For production deployment, configure API authentication and security according to the Anthropic API requirements.

## 📁 Project Structure

```text
Content-Intelligence-Studio/
└── index.html
```
## Author 
Neha Duggal 
