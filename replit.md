# Brianne E. Bonus — Personal Landing Page

## Project Overview

A professional personal landing page for Brianne E. Bonus, a Business Analytics and Information Systems student at The University of Iowa (graduating May 2026). Serves as a digital proof-of-concept demonstrating GitHub and web presence management skills.

## Architecture

- **Type:** Static HTML/CSS/JS website
- **Stack:** Vanilla HTML5, CSS3, no frameworks
- **Server:** `serve` npm package (static file server)
- **Port:** 5000

## Folder Structure

```
/
├── index.html          # Main page
├── css/
│   └── stylesheet.css  # All styles (no inline styles)
├── js/
│   └── scripts.js      # Smooth scroll behavior
├── images/
│   └── headshot.svg    # Placeholder — replace with actual headshot.jpg
├── package.json
└── node_modules/
```

## Design Standards

- **Colors:** Background #FFFFFF, Primary text #1B263B, Accent #0D6E6E, Section bg #F8F9FA
- **Typography:** Inter font (Google Fonts), H1 1.75rem bold, H2 1.25rem bold teal
- **Profile photo:** 160px circular crop
- **Accessibility:** WCAG 2.2 Level AA

## Development

```bash
npm start   # Starts serve on port 5000
```

## Deployment

Configured as a **static** deployment. The user can click Publish to deploy.

## Notes

- The `images/headshot.svg` is a placeholder. Replace with `images/headshot.jpg` (or update the `<img src>` in index.html) once the actual headshot is provided.
- LinkedIn and GitHub URLs in `index.html` should be updated to Brianne's actual profile URLs.
