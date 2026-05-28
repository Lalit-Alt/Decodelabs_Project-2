# 📱 Project 2 — Responsive Web Layout

> **DecodeLabs Industrial Training Kit · Batch 2026 · Frontend Development**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Design-4CAF50?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

This project is **Project 2** of the DecodeLabs Frontend Development Industrial Training Program. The goal is to build a fully **responsive webpage** that gracefully adapts across all screen sizes — from mobile phones to large desktop monitors — using pure HTML and CSS, with zero reliance on frameworks.

The core philosophy: **Content is like water. It should take the shape of its container.**

---

## 🎯 Goal

Build a responsive webpage that works across different screen sizes using CSS media queries, responsive navigation, and proper spacing and alignment.

---

## ✅ Implementation Checklist

- [x] Viewport meta tag — `width=device-width, initial-scale=1`
- [x] Mobile-First base CSS strategy
- [x] Layout using **CSS Grid** (macro structure) & **Flexbox** (micro components)
- [x] Fluid units — `%`, `rem`, `vw`
- [x] Fluid Typography using `clamp()`
- [x] Hamburger / Popover navigation for mobile (No JS required)
- [x] Accessible touch targets (minimum `44px × 44px`)
- [x] User-controlled zoom — WCAG compliant (up to 500%)

---

## 🛠️ Key Concepts Applied

### 📐 Mobile-First Strategy
CSS is written for mobile screens first. Complexity is added progressively using `min-width` media queries as the viewport expands.

```css
/* Base styles → Mobile Core */
.container {
  display: flex;
  flex-direction: column;
}

/* Tablet → Layout Enhancements */
@media (min-width: 768px) {
  .container {
    flex-direction: row;
  }
}

/* Desktop → High-Res Assets */
@media (min-width: 1024px) {
  ...
}
```

### 🏗️ Architectural Harmony — Grid + Flexbox
- **CSS Grid** → The "house" (macro page layout: header, sidebar, main, footer)
- **Flexbox** → The "furniture" (micro component alignment: cards, nav items, buttons)

```css
/* Grid for the layout */
.page-layout {
  display: grid;
  grid-template-columns: 250px 1fr;
  grid-template-rows: auto 1fr auto;
}

/* Flexbox for the components */
.card-grid {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}
```

### 🔤 Fluid Typography with `clamp()`
```css
h1 {
  font-size: clamp(1rem, 2.5vw, 2rem);
  /* Min: 1rem → Ideal: 2.5vw → Max: 2rem */
}
```

### 🍔 Hamburger Navigation (Popover API — No JS)
```html
<button popovertarget="nav-menu">☰</button>
<nav id="nav-menu" popover>
  <!-- Navigation links -->
</nav>
```

---

## 📂 Project Structure

```
project-2-responsive-layout/
│
├── index.html          # Main HTML file
├── style.css           # All styles with media queries
├── assets/
│   └── images/         # Optimized images
└── README.md           # You are here
```

---

## 📱 Breakpoints Used

| Breakpoint | Range       | Target              |
|------------|-------------|---------------------|
| Mobile     | `0 – 479px` | Base CSS (default)  |
| Small      | `480px+`    | Adjusted spacing    |
| Tablet     | `768px+`    | Layout enhancements |
| Desktop    | `1024px+`   | High-res assets     |

> 💡 **Pro Tip:** Breakpoints are set where the **content breaks**, not where specific devices exist.

---

## ♿ Accessibility

- No `user-scalable=no` in the viewport meta tag
- Zoom up to **500%** supported (WCAG 2.1 compliant)
- All interactive elements meet the **44px × 44px** minimum touch target size
- Semantic HTML5 elements used throughout (`<header>`, `<nav>`, `<main>`, `<footer>`)

---

## 🚀 How to Run

No build tools or dependencies required.

```bash
# Clone the repository
git clone https://github.com/<your-username>/project-2-responsive-layout.git

# Navigate into the project
cd project-2-responsive-layout

# Open in browser
open index.html
# OR use Live Server in VS Code
```

---

## 📚 Resources

| Type          | Resource                     | Link                                      |
|---------------|------------------------------|-------------------------------------------|
| Documentation | MDN Web Docs                 | https://developer.mozilla.org             |
| Documentation | CSS-Tricks                   | https://css-tricks.com                    |
| Tool          | Fluid Type Scale Calculator  | https://utopia.fyi                        |
| Tool          | CanIUse                      | https://caniuse.com                       |

---

## 🏆 Qualification Criteria

| Requirement  | Details                                                       |
|--------------|---------------------------------------------------------------|
| Requirement  | Complete Project 2 to unlock projects for the following week  |
| Standard     | All projects must be verified for quality                     |
| Mandatory    | Project 2 is the vital bridge to professional development     |

---

## 🌱 Key Learnings

- Responsive design is about **fluidity**, not fixed dimensions
- Always include the **viewport meta tag** — without it, mobile browsers render at a fake 980px width
- Think **Mobile-First**: start simple, scale up with `min-width` queries
- Use **Grid for the layout**, **Flexbox for the components**
- Breakpoints should serve your **content**, not specific device models
- The modern **Popover API** enables interactive mobile navigation with zero JavaScript

---

## 👨‍💻 Author

**[Lalit Yadav]**
Frontend Developer Intern — DecodeLabs Batch 2026

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)]([https://linkedin.com/in/lalit-yadav-019950319](https://www.linkedin.com/in/lalit-yadav-019950319?))
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github)](https://github.com/Lalit-Alt)

---

## 🏢 Organization

**DecodeLabs**
📞 +91 89330 06408 &nbsp;|&nbsp; ✉️ decodelabs.tech@gmail.com &nbsp;|&nbsp; 🌐 [www.decodelabs.tech](https://www.decodelabs.tech) &nbsp;|&nbsp; 📍 Greater Lucknow, India

---

<div align="center">

*"Your journey to becoming a professional developer begins right here, right now, with the very first breakpoint you set today."*

**— DecodeLabs**

</div>
