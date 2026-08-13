# Day 10 - Personal Portfolio Website

This repository contains the Day 10 submission for building a modern, single-file responsive Personal Portfolio Website using **HTML5**, **Tailwind CSS (CDN)**, and **Vanilla JavaScript**.

---

## 📑 Overview

The goal of Day 10 is to create a complete, responsive personal portfolio website with zero build tools, relying on Tailwind CSS via CDN and client-side JavaScript for interactive features.

### ✨ Key Features:
- 🌙 **Dark / Light Mode Toggle:** Smooth color transitions using Tailwind CSS `dark:` variant and local storage persistence.
- ⌨️ **Dynamic Typing Animation:** Custom Vanilla JS typing effect in the hero section.
- 📱 **Fully Responsive Layout:** Designed for desktop, tablet, and mobile screens with an accessible mobile navbar menu.
- ⚡ **Interactive Skill Bars & Tech Cards:** Clean layout highlighting core skills, tools, and project showcase.
- 📬 **Contact Form Interface:** Fully styled form with direct social/email links.
- 🔍 **SEO & Accessibility:** Included metadata, structured semantic HTML tags, and smooth scrolling (`scroll-smooth`).

---

## 🛠️ Tech Stack & Tools

- **Markup:** HTML5
- **Styling:** Tailwind CSS (via CDN) & Custom CSS Keyframes
- **Scripting:** Vanilla JavaScript (ES6+)
- **Icons:** FontAwesome v6 (CDN)
- **Deployment Options:** Vercel / Netlify / GitHub Pages

---
# 🧠 Key Learnings & Takeaways

Below is the complete key learnings summary for your `day10.md` or submission report in a single container:

---

## 📑 Learnings Breakdown

### 1. Tailwind CSS CDN & Rapid Prototyping
- **No-Build Configuration:** Learned how to extend Tailwind's theme directly via the `tailwind.config` script block in HTML without installing Node.js dependencies or setting up PostCSS.
- **Utility-First Styling:** Utilized responsive prefixes (`sm:`, `md:`) and dynamic state modifiers (`hover:`, `focus:`, `dark:`) to construct a sleek, modern UI entirely in HTML.

### 2. Dark/Light Theme Switching with State Persistence
- **Class-Based Dark Mode:** Implemented dark mode by toggling the `.dark` class on the root `<html>` element using JavaScript.
- **LocalStorage State:** Learned how to preserve the user's preferred theme across page reloads using browser `localStorage` (`localStorage.setItem('color-theme', theme)`).

### 3. Pure Vanilla JavaScript Interactivity
- **Custom Typing Effect:** Built an asynchronous-like loop using dynamic string slicing (`substring()`) and `setTimeout` to cycle through job titles without relying on heavy external libraries like Typed.js.
- **DOM Event Handling:** Managed mobile navigation menu state and interactive dark-mode icon swapping using native Event Listeners.

### 4. Responsive & Accessible Web Architecture
- **Mobile-First Navigation:** Designed a collapsible mobile navbar alongside a clean desktop layout.
- **Semantic HTML & SEO:** Structured sections using proper tags (`<section>`, `<nav>`, `<header>`, `<footer>`) and added essential `<meta>` tags for search engine optimization.
- **Smooth Navigation:** Applied `scroll-smooth` to the HTML root for seamless section-to-section jumping via navbar links.

---

