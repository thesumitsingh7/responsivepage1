# Task 01 — Responsive Landing Page
**Internship:** UpStartInterns · Full Stack Development  
**Student Intern:** Sumit Kumar  
**Project:** Lumière Artisan Boulangerie & Café  

---

## 🌟 Overview

This project is a single-page responsive website built to fulfill all requirements of **Task 01 (Warm-up · Responsive Landing Page)**. It is self-contained in a single HTML file (`index.html`), embedding semantic HTML5, mobile-first responsive CSS3, crisp inline vector SVGs, and interactive vanilla JavaScript.

---

## ✅ Acceptance Criteria Met

| Requirement | Implementation Detail | Status |
| :--- | :--- | :---: |
| **Mobile & Desktop Layout** | Implemented mobile-first. At `< 768px`, displays a single-column layout with an accessible collapsible drawer menu. At `≥ 768px` and `≥ 1024px`, expands into multi-column desktop grids, inline navigation, and side-by-side hero split. | **PASSED** |
| **Real Content (No Lorem Ipsum)** | Handcrafted, authentic copy for an artisanal sourdough bakery & specialty espresso bar (fermentation times, heritage grain origins, daily hot-pull bake timetable, pricing, and operating hours). | **PASSED** |
| **Images Do Not Overflow** | All visual illustrations are inline vector SVGs with dynamic `viewBox` coordinates, governed by universal CSS rules (`max-width: 100%; height: auto; display: block;`). Parent containers enforce strict width boundaries. | **PASSED** |
| **Zero Horizontal Scroll at 375px** | Tested and verified: page maintains exact viewport containment with `overflow-x: hidden`, flexible padding, and `box-sizing: border-box`. | **PASSED** |
| **All-in-One Single File** | Everything (HTML, CSS styling, SVG illustrations, and JS behavior) is packaged cleanly into `index.html` with zero external dependencies. | **PASSED** |

---

## 🛠️ Key Design & Architectural Decisions

1. **Mobile-First CSS Strategy**:
   - The default stylesheet targets mobile devices (using the standard 375px iPhone screen as the minimum reference).
   - Progressive enhancement via `@media (min-width: 768px)` and `@media (min-width: 1024px)` expands the layout for tablets and desktops.

2. **Zero-Dependency Vector Graphics (SVGs)**:
   - Hand-crafted inline SVG graphics for the hero bread boule, batard loaf, French butter croissant, and flat white espresso cup.
   - Using inline SVGs eliminates broken image links, reduces HTTP requests to zero, ensures lightning-fast loading, and prevents image overflow on narrow viewports.

3. **Accessibility & Semantics**:
   - Clean HTML5 landmark elements: `<header>`, `<main>`, `<section>`, `<article>`, `<footer>`.
   - ARIA attributes (`aria-expanded`, `aria-controls`, `aria-label`, `role="status"`) for full keyboard and screen-reader accessibility.

---

## 🚀 How to Run

Because the project is completely self-contained in `index.html`, you do not need any build tools, package managers, or server installations.

### Option 1: Direct File Opening (Easiest)
Simply double-click `index.html` in your file manager, or open it in any web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari).

### Option 2: Using Local HTTP Server
If you prefer running a local server:

**Using Python:**
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` in your browser.

**Using Node.js:**
```bash
npx serve .
```

---

## 📐 Responsive Testing Checklist

- [x] **375px (iPhone SE / Mobile):** Single column, collapsible nav drawer, zero horizontal overflow.
- [x] **414px / 430px (iPhone Pro / Plus):** Proportional layout, clear typography.
- [x] **768px (Tablet / iPad):** 3-column craft cards, 2-column menu grid, inline navigation bar.
- [x] **1024px+ (Desktop / Laptop):** Split 2-column hero, 3-column menu showcase, comfortable reading widths.
