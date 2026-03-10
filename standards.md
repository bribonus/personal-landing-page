# STANDARDS.md

## 1. Project Overview

[cite_start]This site is a professional landing page for **Brianne E. Bonus**, a **Business Analytics and Information Systems** student at **The University of Iowa**[cite: 1]. It serves as a digital "proof of concept" to demonstrate technical literacy in **GitHub** and **LinkedIn** integration for recruiters at mid-sized companies. Success is defined by achieving at least 5 unique interactions on professional profile links within 60 days of launch.

## 2. Technical Standards

**Languages and versions:**

- **HTML5** — use semantic elements: `<header>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<nav>`.
- **CSS3** — all styles in `css/stylesheet.css`; no inline styles or `<style>` tags.

**Folder structure:**
/your-website-project (Root Folder)  
├── index.html  
├── /css  
│ └── stylesheet.css  
├── /js  
│ └── scripts.js  
├── /images  
│ └── headshot.jpg

**Framework:**

- **No framework** — vanilla CSS only.

**Architecture:**

- Static site with a single `index.html` file in the root.
- All images stored in `images/` subfolder; no external image URLs.
- **Do not link to or embed a resume** on the site.

**Accessibility & Compatibility:**

- **WCAG 2.2 Level AA:** Descriptive `alt` attributes, 4.5:1 contrast ratio, logical heading hierarchy.
- **Responsiveness:** Fully responsive from 320px and wider; no horizontal scrolling.

## 3. Design Standards

**Color palette:**
| Role | Hex Code | Usage |
| :--- | :--- | :--- |
| **Background** | #FFFFFF | Page background |
| **Primary text** | #1B263B | Navy - Body copy, paragraphs |
| **Accent** | #0D6E6E | Teal - Section headings, links |
| **Secondary background** | #F8F9FA | Light Gray - Section/Skill backgrounds |

**Typography:**

- **Fonts:** **Inter** (Bold for headings, Regular for body) imported from Google Fonts.
- **Hierarchy:** H1 (1.75rem, bold), H2 (1.25rem, bold, Teal), Body (16px, 1.6 line height).

**Component styles:**

- **Profile photo:** Circular crop, 160px diameter, centered in hero.
- **Skill tags:** Rounded pill badges; Teal background with white text.
- **Tone:** Professional, Approachable, Data-driven.
