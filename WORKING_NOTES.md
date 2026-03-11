# Working Notes — Brianne E. Bonus Personal Landing Page

> **INTERNAL DOCUMENT — NOT FOR PUBLIC AUDIENCES**
> This file is intended for developer and AI assistant reference only. It is not part of the public-facing project. Update this file at the end of every working session before committing.

---

## 1. How to Use This File (For AI Assistants)

1. Read this entire file before suggesting changes or writing any code.
2. Read `README.md` for the public-facing project description and feature roadmap.
3. Do not change the folder structure or file naming conventions without explicit discussion with the author.
4. Follow all conventions listed in Section 8 exactly — do not introduce new patterns without flagging them.
5. Do not suggest any approach listed in Section 10 (What Was Tried and Rejected).
6. Ask clarifying questions before making large structural changes (e.g., adding a framework, restructuring HTML, changing the color palette).
7. This project was **AI-assisted** (scaffolded and generated with Replit AI / Claude). Refactor conservatively — prefer small, targeted edits over wholesale rewrites.

---

## 2. Current State

**Last Updated:** 2026-03-11

This is a complete, live personal landing page for Brianne E. Bonus. The site is fully functional and deployed via Replit. All required content from the PRD is present. The repository root also contains supporting documents (PRD.md, STANDARDS.md, resume PDF, LICENSE, README.md). No backend or database is involved.

### What Is Working
- [x] Hero section with professional headshot, full name, and tagline
- [x] About section with accurate academic bio (University of Iowa, BBA BAIS, Certificate of International Business, May 2026)
- [x] Skills section with three categorized subsections and teal pill badges
- [x] Contact section with correct LinkedIn, GitHub, and email links
- [x] Sticky navigation header with smooth scroll to sections
- [x] Fully responsive layout (320px and wider, no horizontal scroll)
- [x] Google Fonts (Inter) loaded via CDN
- [x] CSS custom properties for color palette and typography
- [x] WCAG 2.2 Level AA accessibility (alt text, aria-labels, heading hierarchy, contrast)
- [x] Static file server running via `serve` on port 5000
- [x] `README.md` with full documentation, badges, and 45-feature roadmap
- [x] `STANDARDS.md` in repository root
- [x] `PRD.md` in repository root
- [x] `Brianne_Bonus_Resume.pdf` in repository root
- [x] `LICENSE` (MIT) added on GitHub

### What Is Partially Built
- [ ] **Profile photo crop** — headshot displays correctly but image is large (950 KB); not yet optimized or converted to WebP

### What Is Not Started
- [ ] Projects section (deferred per PRD scope)
- [ ] Contact form
- [ ] Dark mode toggle
- [ ] Interactive dashboards or data visualizations
- [ ] GitHub Actions CI/CD for automated deployment
- [ ] Custom domain setup

---

## 3. Current Task

**What I was working on when I last stopped:**
The initial site was fully built and all content from the PRD was added. The final session focused on adding repository documentation files (README.md, WORKING_NOTES.md), confirming correct LinkedIn and GitHub profile URLs, and adding the resume PDF to the root. The LICENSE file was added directly on GitHub by the author.

**The very next step is:**
Optimize `images/headshot.jpg` by compressing it and converting to WebP format to improve page load performance, then update the `<img>` tag in `index.html` accordingly.

---

## 4. Architecture and Tech Stack

| Technology | Version | Why It Was Chosen |
| :--- | :--- | :--- |
| HTML5 | N/A | Required by STANDARDS.md; semantic elements improve accessibility and SEO |
| CSS3 | N/A | Required by STANDARDS.md; vanilla CSS keeps the project dependency-free |
| JavaScript (Vanilla) | ES6+ | Minimal interactivity needed (smooth scroll only); no framework justified |
| Google Fonts — Inter | N/A | Specified in STANDARDS.md as the required typeface |
| serve (npm) | ^14.2.6 | Lightweight, zero-config static file server for local development on Replit |
| Node.js | 20.x | Required runtime for `serve`; installed via Replit module system |
| Replit | N/A | Free hosting platform used for development and live preview |
| GitHub | N/A | Version control and public repository hosting per PRD requirements |

---

## 5. Project Structure Notes

```
personal-landing-page/
├── index.html                  # Single-page site entry point
├── css/
│   └── stylesheet.css          # All styles — no inline styles or <style> tags allowed
├── js/
│   └── scripts.js              # Smooth scroll only; keep minimal
├── images/
│   └── headshot.jpg            # Local headshot — no external image URLs per STANDARDS.md
├── Brianne_Bonus_Resume.pdf    # Repository reference only — not linked on the site per STANDARDS.md
├── PRD.md                      # Product Requirements Document
├── STANDARDS.md                # Design and technical standards (renamed from standards.md)
├── README.md                   # Public-facing project documentation
├── WORKING_NOTES.md            # This file — internal only
├── package.json                # npm config for `serve` dependency
├── package-lock.json           # Lockfile — do not edit manually
└── replit.md                   # Replit environment notes (auto-managed)
```

**Non-obvious decisions:**
- `Brianne_Bonus_Resume.pdf` is in the root for repository visibility but is **intentionally not linked from the website** per STANDARDS.md ("Do not link to or embed a resume on the site").
- `node_modules/` and `package.json` exist solely to run `serve` locally on Replit — this project has no build step and no JavaScript dependencies for the site itself.
- `replit.md` is managed by Replit and should not be deleted.

**Files that must not be changed without discussion:**
- `css/stylesheet.css` — color palette, typography, and component styles are all defined in STANDARDS.md and must not drift
- `STANDARDS.md` — authoritative design and technical spec for this project
- `package-lock.json` — do not edit manually

---

## 6. Data / Database

This project has **no persistent data, database, or flat data files**. All content is hardcoded in `index.html`. There is no backend server, API, or data layer of any kind.

---

## 7. Conventions

### Naming Conventions
- **HTML file:** `index.html` only — single page, no additional HTML files
- **CSS file:** `css/stylesheet.css` — singular, lowercase, hyphenated
- **JS file:** `js/scripts.js` — singular, lowercase, hyphenated
- **Images:** lowercase, hyphenated filenames stored in `images/`
- **CSS classes:** lowercase, hyphenated (e.g., `.skill-tag`, `.profile-photo`, `.contact-list`)
- **CSS custom properties:** `--color-bg`, `--color-text`, `--color-accent`, `--color-section-bg`, `--font-family`

### Code Style Rules
- No inline styles — all CSS goes in `css/stylesheet.css`
- No `<style>` tags in HTML
- Semantic HTML5 elements required: `<header>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<nav>`
- All external links must include `target="_blank"`, `rel="noopener noreferrer"`, and a descriptive `aria-label`
- All images require descriptive `alt` attributes
- `aria-labelledby` used on every `<section>` pointing to its heading

### Color Palette (Do Not Deviate)
| Role | Hex |
| :--- | :--- |
| Background | `#FFFFFF` |
| Primary text | `#1B263B` |
| Accent | `#0D6E6E` |
| Section background | `#F8F9FA` |

### Typography (Do Not Deviate)
- Font: Inter (Google Fonts)
- H1: 1.75rem, bold
- H2: 1.25rem, bold, teal (`#0D6E6E`)
- Body: 16px, line-height 1.6

### Git Commit Message Style
- Imperative mood, present tense: "Add headshot image", "Update LinkedIn URL"
- Short and descriptive — no need for conventional commit prefixes on this project

---

## 8. Decisions and Tradeoffs

- **Decision made: No CSS framework (no Tailwind, Bootstrap, etc.)** — STANDARDS.md explicitly requires vanilla CSS only. Do not suggest adding a framework.
- **Decision made: No JavaScript framework (no React, Vue, etc.)** — The site is a single static page with no state or dynamic content. A framework would be over-engineering.
- **Decision made: `serve` used as the local dev server instead of a custom Node.js server** — Zero configuration needed; appropriate for a purely static site.
- **Decision made: Resume PDF is in the repository root but not linked on the site** — STANDARDS.md explicitly prohibits linking to or embedding the resume. The PDF is for repository reviewers only.
- **Decision made: Headshot stored locally in `images/` folder** — STANDARDS.md prohibits external image URLs. The image must always be hosted locally.
- **Decision made: Single `index.html` with all sections** — PRD specifies a static site with a single HTML file. No routing or multi-page structure is needed.
- **Decision made: `standards.md` renamed to `STANDARDS.md`** — Renamed to all-caps for consistency with conventional repository documentation naming (README, LICENSE, etc.).

---

## 9. What Was Tried and Rejected

- **SVG placeholder as headshot** — An SVG with initials "BB" was used temporarily while awaiting the real headshot. It was replaced with the actual JPG. Do not revert to the SVG.
- **`images/headshot.jpg` as an empty file** — The first upload attempt resulted in a 0-byte file. The actual image was re-uploaded successfully. Do not reference the old empty file.

---

## 10. Known Issues and Workarounds

- **Headshot file size is large (~950 KB)** — The JPG has not been compressed or converted to WebP. Page load may be slower on mobile connections. No workaround is in place. This is the next optimization task.
- **LinkedIn and GitHub URLs were initially incorrect** — Placeholder URLs (`/in/brianne-bonus`, `/brianneebonus`) were used during scaffolding and later corrected to the real profiles. The correct URLs are now in place; do not revert.
- **`LICENSE` file exists on GitHub but not in the local Replit environment** — The author added the LICENSE directly via GitHub's web interface. It is present in the remote repository. This is not a bug — the local working copy will receive it on the next `git pull`.

---

## 11. Browser / Environment Compatibility

**Tested in:** Replit web preview (Chromium-based)

**Expected to work in:**
- Chrome / Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile Safari (iOS 15+)
- Chrome for Android (latest)

**Known incompatibilities:**
- CSS custom properties (`var()`) are not supported in Internet Explorer 11. IE11 is not a target browser for this project.
- `scroll-behavior: smooth` is not supported in older Safari versions; scroll will fall back to instant jump gracefully.

**Environment:**
- Runtime: Node.js 20.x (Replit)
- OS: NixOS (Replit container)
- Static server: `serve` ^14.2.6 on port 5000

---

## 12. Open Questions

- Should the resume PDF eventually be linked from the site (e.g., as a button in the hero or contact section), or remain repository-only? STANDARDS.md currently prohibits this — would require a standards update.
- Should a Projects section be built for the AArete Capstone or data mining projects before the May 2026 graduation deadline?
- Should the site be deployed to GitHub Pages (free) in addition to Replit, since GitHub Pages was the original deployment target in the PRD?
- Is a custom domain desired for the deployed site?
- Should `Brianne_Bonus_Resume.pdf` be renamed with a version date or kept as a generic filename?

---

## 13. Session Log

### 2026-03-11
- **Accomplished:** Full site scaffolded and deployed on Replit. All PRD content added: hero with headshot, about bio, skills with pill badges, contact with correct LinkedIn/GitHub/email. Sticky nav with smooth scroll implemented. CSS custom properties, responsive layout, and WCAG 2.2 Level AA accessibility applied. Repository root populated with PRD.md, STANDARDS.md, Brianne_Bonus_Resume.pdf. README.md generated with badges, 45-feature roadmap, and all required sections. WORKING_NOTES.md generated. MIT LICENSE added by author directly on GitHub.
- **Left incomplete:** Headshot image not yet optimized (950 KB JPG, no WebP conversion).
- **Decisions made:** Resume intentionally not linked on site per STANDARDS.md. `standards.md` renamed to `STANDARDS.md`. `serve` chosen as static dev server. No framework used per STANDARDS.md.
- **Next step:** Compress and convert `images/headshot.jpg` to WebP; update `<img>` src in `index.html`.

---

## 14. Useful References

- [STANDARDS.md](./STANDARDS.md) — authoritative design and technical spec for this project
- [PRD.md](./PRD.md) — original product requirements document
- [README.md](./README.md) — public-facing documentation and feature roadmap
- [MDN HTML5 Semantic Elements](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html) — reference for correct semantic element usage
- [MDN CSS Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) — reference for `var()` usage
- [WCAG 2.2 Quick Reference](https://www.w3.org/WAI/WCAG22/quickref/) — accessibility compliance checklist
- [Google Fonts — Inter](https://fonts.google.com/specimen/Inter) — typeface used throughout the site
- [serve npm package](https://www.npmjs.com/package/serve) — static file server documentation
- [Shields.io](https://shields.io/) — README badge generator
- **AI Assistance:** Site structure, HTML/CSS, and all documentation files were generated using Replit AI (Claude) and reviewed, customized, and approved by the author. All URLs, personal details, and content decisions were provided and verified by the author.
