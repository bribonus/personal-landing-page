# Brianne E. Bonus — Personal Landing Page

![MIT License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/built%20with-HTML5-orange)
![CSS3](https://img.shields.io/badge/styled%20with-CSS3-blue)
![Status](https://img.shields.io/badge/status-live-brightgreen)

---

## Description 

This project is a professional personal landing page built for Brianne E. Bonus, a senior at The University of Iowa pursuing a Bachelor of Business Administration in Business Analytics and Information Systems. It exists to serve as a functional "proof of concept" demonstrating technical literacy in GitHub, version control, and web presence management — skills that go beyond a traditional static resume. The site showcases Brianne's academic background, technical skill set, and professional links in a clean, accessible, and fully responsive design. It is intended for hiring managers and technical recruiters at mid-sized companies who are evaluating candidates with a strong foundation in data analytics and business intelligence.

---

## Live Site

[View the live site](https://bribonus.github.io/personal-landing-page)

---

## Table of Contents

- [Description](#description)
- [Live Site](#live-site)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Accessibility](#accessibility)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

---

## Screenshots

![Landing page screenshot showing hero section with headshot, name, and navigation](images/headshot.jpg)

---

## Technologies Used

- **HTML5** — Semantic structure using `<header>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<nav>`
- **CSS3** — Custom properties, Flexbox, responsive media queries; all styles in `css/stylesheet.css`
- **JavaScript (Vanilla)** — Smooth scroll behavior in `js/scripts.js`
- **Google Fonts** — Inter typeface (Bold for headings, Regular for body)
- **serve** (npm) — Lightweight static file server for local development

---

## Features

The following features represent a roadmap of improvements and additions planned for a future version of this project:

- [ ] Add a dark mode toggle with CSS custom property theming and localStorage persistence
- [ ] Build a dedicated Projects section showcasing data analytics case studies with descriptions and links
- [ ] Embed interactive Power BI or Tableau dashboards directly on the page
- [ ] Add a downloadable resume button linking to the PDF in the repository
- [ ] Implement a contact form using a serverless function (e.g., Formspree or Netlify Forms)
- [ ] Add animated entrance transitions using CSS keyframes or the Intersection Observer API
- [ ] Create a Skills progress-bar visualization showing proficiency levels per tool
- [ ] Add a testimonials or endorsements section for peer and supervisor quotes
- [ ] Introduce a sticky "back to top" button for improved navigation on mobile
- [ ] Build a filterable project gallery using vanilla JavaScript category toggles
- [ ] Add Open Graph and Twitter Card meta tags for improved social sharing previews
- [ ] Integrate a favicon and web app manifest for PWA compatibility
- [ ] Implement a blog or "Insights" section for writing about data analytics topics
- [ ] Add micro-interactions (hover animations, button ripple effects) to skill tags and links
- [ ] Create a timeline component visually representing academic and work history
- [ ] Add a language switcher for Spanish or Italian internationalization
- [ ] Integrate Google Analytics or Plausible for privacy-friendly visitor tracking
- [ ] Optimize all images with WebP format conversion and lazy loading
- [ ] Add a loading skeleton screen for perceived performance improvement
- [ ] Improve color contrast for WCAG 2.2 AAA compliance across all text elements
- [ ] Add a print stylesheet for clean single-page resume printing
- [ ] Create an RSS feed for any future blog or project updates
- [ ] Add smooth page transitions using the View Transitions API
- [ ] Build a "Now" page describing current courses, projects, and reading
- [ ] Add a GitHub activity feed widget showing recent commits and contributions
- [ ] Integrate LinkedIn badge for live connection count display
- [ ] Add a certifications section for future Microsoft, Salesforce, or Snowflake credentials
- [ ] Create a dedicated page for the AArete Capstone project with methodology detail
- [ ] Add structured data (JSON-LD schema) for Person, ContactPoint, and WebPage types
- [ ] Implement a cookie consent banner for GDPR compliance
- [ ] Build an awards and honors section highlighting Dean's List recognition
- [ ] Add a study abroad highlight card for the Verona, Italy experience
- [ ] Create a "Tech Stack" visual icon grid using SVG logos
- [ ] Add a Spotify or book recommendation widget as a personal touch
- [ ] Integrate GitHub Pages deploy automation via a GitHub Actions CI/CD workflow
- [ ] Add a page speed and Lighthouse score badge in the README
- [ ] Create a custom 404 error page matching the site's design system
- [ ] Improve mobile navigation with a hamburger menu and slide-in drawer
- [ ] Add keyboard navigation focus styles beyond browser defaults for accessibility
- [ ] Implement skip-to-content link for screen reader and keyboard user accessibility
- [ ] Add a "References available upon request" section with a mailto call to action
- [ ] Create a visual data storytelling section using Chart.js or D3.js
- [ ] Integrate a headless CMS (e.g., Contentlayer or Sanity) for content management
- [ ] Add automated accessibility testing with axe-core in a GitHub Actions pipeline
- [ ] Generate an automated sitemap.xml and robots.txt for search engine optimization

---

## Getting Started

To run this project locally:

1. **Clone the repository**
   ```bash
   git clone https://github.com/bribonus/personal-landing-page.git
   cd personal-landing-page
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the local server**
   ```bash
   npm start
   ```

4. Open your browser and navigate to `http://localhost:5000`

No build step is required — this is a fully static site.

---

## Project Structure

```
personal-landing-page/
├── index.html                  # Main HTML file
├── css/
│   └── stylesheet.css          # All styles (no inline styles)
├── js/
│   └── scripts.js              # Smooth scroll behavior
├── images/
│   └── headshot.jpg            # Professional headshot
├── Brianne_Bonus_Resume.pdf    # Resume (repository reference only)
├── PRD.md                      # Product Requirements Document
├── STANDARDS.md                # Design and technical standards
├── package.json
└── README.md
```

---

## Accessibility

This site targets **WCAG 2.2 Level AA** compliance:

- Descriptive `alt` attributes on all images
- Logical heading hierarchy (H1 → H2 → H3)
- 4.5:1 minimum color contrast ratio
- Fully responsive from 320px viewport width and wider
- `aria-label` attributes on all external links
- Semantic landmark elements throughout

---

## Contributing

Contributions, suggestions, and improvements are welcome. To contribute to this project:

1. **Fork** this repository by clicking the Fork button at the top right of the GitHub page.
2. **Clone** your fork locally: `git clone https://github.com/your-username/personal-landing-page.git`
3. **Create a branch** for your changes: `git checkout -b feature/your-feature-name`
4. **Make your changes** following the standards outlined in `STANDARDS.md`.
5. **Commit** your changes with a clear message: `git commit -m "Add: description of your change"`
6. **Push** your branch to GitHub: `git push origin feature/your-feature-name`
7. **Open a Pull Request** on the original repository and describe what you changed and why.

Please ensure any changes maintain WCAG 2.2 Level AA accessibility compliance and follow the color palette and typography rules defined in `STANDARDS.md`.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

**Brianne E. Bonus**
The University of Iowa
BAIS 3300 — Business Applications and Information Systems

---

## Contact

- GitHub: [github.com/bribonus](https://github.com/bribonus)

---

## Acknowledgements

- [Google Fonts](https://fonts.google.com/) — Inter typeface used throughout the site
- [serve](https://www.npmjs.com/package/serve) — Static file server used for local development
- [Shields.io](https://shields.io/) — README badge generation
- [MDN Web Docs](https://developer.mozilla.org/) — HTML5 semantic elements and CSS3 reference documentation
- [W3C WCAG 2.2 Guidelines](https://www.w3.org/TR/WCAG22/) — Accessibility compliance reference
- [CSS-Tricks](https://css-tricks.com/) — Flexbox and responsive design patterns reference
- [The Noun Project](https://thenounproject.com) — Icon resources
- **Replit AI (Claude)** — Initial code structure, README generation, and site scaffolding generated with AI assistance and reviewed, customized, and approved by the author
- Icon: [vibe coding](https://thenounproject.com) by iqonica from [Noun Project](https://thenounproject.com) (CC BY 3.0)
