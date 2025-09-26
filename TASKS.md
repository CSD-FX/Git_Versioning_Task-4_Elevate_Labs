# DevOps Task 4 — Version-Controlled DevOps Project

## Project Overview
- Theme: Harry Potter — Fantastic Beasts prequel series
- Objective: Manage a small multi-page website using Git best practices
- Pages: `index.html`, `about.html`, `contact.html`
- Deployment: GitHub Pages (static hosting)

---

## Branch Strategy

| Branch              | Purpose                               | Version |
|--------------------|---------------------------------------|--------|
| main                | Production / landing page              | v1.0   |
| dev                 | Integration branch                     | v1.0+  |
| feature1-about      | Add About page                         | v1.0   |
| feature2-contact    | Add Contact page                       | v2.0   |

---

## Version History

### Version 1.0
- **Files Added:** `index.html`, `about.html`, `assets/css/style.css`
- **Branch:** `feature1-about` merged into `dev` → `main`
- **Tag:** `v1.0`
- **Description:** Landing page with poster, About page with movie details

### Version 2.0
- **Files Added:** `contact.html`
- **Branch:** `feature2-contact` merged into `dev` → `main`
- **Tag:** `v2.0`
- **Description:** Added Contact page with project owner details

---

## Deployment Instructions
1. GitHub Pages enabled from `main` branch (root folder)
2. URL: `https://<your-username>.github.io/<repo-name>/`
3. Navigate using the navbar to `Home`, `About`, `Contact`

---

## Local Testing
```bash
# Serve site locally
python3 -m http.server 8000
# Open in browser
http://localhost:8000/index.html
# Click About and Contact links to test navigation

