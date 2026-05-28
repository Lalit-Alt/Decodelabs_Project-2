# 🎨 Project 1 — Static Webpage Design

> **DecodeLabs Industrial Training Kit · Batch 2026 · Frontend Development Track**

---

## 📌 Overview

This is **Project 1** of the DecodeLabs Frontend Development Industrial Training Program. The goal is to build a fully static webpage using only **HTML and CSS**, demonstrating mastery of semantic structure, clean layout, and separation of concerns — before moving on to dynamic, JavaScript-driven applications.

> *"Build it well, for the frontend is the only part of the system the world will ever see."*
> — DecodeLabs Engineering Mandate

---

## 🎯 Project Goal

Create a **static webpage** using HTML and CSS that demonstrates:

- Proper semantic HTML structure
- Use of headings, sections, and images
- A clean, readable, and accessible layout

---

## ✅ Requirements Checklist (Flight Checklist)

| Area | Requirement |
|---|---|
| **IA** | Logical sitemap defined before writing code |
| **HTML** | Semantic tags used (`<header>`, `<main>`, `<footer>`). One `<h1>` per page |
| **CSS** | External stylesheet only. DRY principle applied. No IDs for styling |
| **Layout** | CSS Grid for macro page structure. Flexbox for component-level alignment |
| **Assets** | Images with explicit `width` and `height` attributes to prevent layout shift (CLS) |
| **Validation** | Passes W3C Validator with zero errors. Passes Lighthouse Audit |

---

## 🛠️ Tech Stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

- **HTML5** — Semantic markup
- **CSS3** — External stylesheet, Grid, Flexbox, BEM methodology

---

## 📁 Project Structure

```
project-1-static-webpage/
├── index.html          # Main HTML file (semantic structure)
├── css/
│   └── style.css       # External stylesheet (no inline styles)
├── assets/
│   └── images/         # All image assets (AVIF/WebP preferred)
└── README.md
```

---

## 🧠 Key Concepts Applied

### Information Architecture (IA)
Structure is defined before any code is written. Content is organized for findability using Dan Brown's principles — objects are living data, and cognitive load is minimized.

### Semantic HTML (No Div Soup)
All layout regions use proper semantic landmarks:
```html
<header> → <nav> → <main> → <article> / <aside> → <footer>
```
Avoids generic `<div>` containers that carry no meaning for browsers or screen readers.

### Document Outline Hierarchy
- One `<h1>` per page (the Zero Point / page topic)
- Headings used as structural keywords, not styling tools
- Levels are never skipped (e.g., no jumping from `<h2>` to `<h4>`)

### CSS Engineering — Separation of Concerns
- **No inline styles** — ever
- All styling lives in `style.css`
- Changes in one place propagate everywhere (DRY principle)

### DRY + BEM Methodology
Components are defined once and reused:
```css
.button { padding: 1rem; border-radius: 4px; }         /* Base */
.button--primary { background: blue; }                  /* Modifier */
```

### Layout Systems
- **CSS Grid** → Macro page structure (2D)
- **Flexbox** → Micro component alignment (1D)

### Assets as Data Objects
All images include explicit dimensions to prevent Cumulative Layout Shift (CLS):
```html
<img src="hero.webp" alt="Description" width="800" height="600">
```

### Accessibility (A11Y)
- All images have descriptive `alt` text
- Color contrast ratio maintained above **4.5:1**
- All interactive elements have accessible labels

---

## 🔍 Quality Gate — Before Submitting

Code does not ship until it passes:

1. **W3C Validation** — Zero errors at [validator.w3.org](https://validator.w3.org/)
2. **Semantic Audit** — Proper landmarks (`<nav>`, `<main>`) confirmed
3. **Lighthouse Audit** — Run in Chrome DevTools, check Accessibility & Best Practices scores

---

## 🚀 How to Run

No build tools or dependencies required.

```bash
# Clone the repository
git clone https://github.com/your-username/project-1-static-webpage.git

# Navigate into the project
cd project-1-static-webpage

# Open in browser
open index.html
# OR just double-click index.html in your file explorer
```

---

## 📚 What I Learned

- How to think in **Information Architecture** before touching code
- The difference between a **sitemap** (the map) and **navigation** (the vehicle)
- Why semantic HTML matters for **SEO** and **screen readers**
- The **IPO Model** for frontend thinking: Input (Assets) → Process (CSS Engineering) → Output (Pixel-Perfect Render)
- How to debug layouts by isolating the stage: Corrupted Input? Logical Error? Rendering Failure?

---

## 🏆 Qualification

Completing this project unlocks access to **Project 2** and subsequent projects in the DecodeLabs Frontend Development track. All submissions are reviewed for quality before the badge is awarded.

---

## 🏢 About DecodeLabs

**DecodeLabs** is an industrial training organization based in Greater Lucknow, India, focused on real-world, project-based developer education.

- 🌐 [www.decodelabs.tech](https://www.decodelabs.tech)
- 📧 decodelabs.tech@gmail.com
- 📞 +91 89330 06408

---

## 📄 License

This project is built as part of the DecodeLabs Industrial Training Program (Batch 2026). All training materials are property of DecodeLabs.
