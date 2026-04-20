<h1 align="center">Nikita Drozdov — Personal Portfolio & CV Website</h1>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap"/>
  <img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white" alt="jQuery"/>
</p>

<p align="center">
  <a href="https://readytow0rk.github.io/personal-cv-website/" target="_blank">
    <img src="https://img.shields.io/badge/🌐 Live Website-Visit Now-brightgreen?style=for-the-badge" alt="Live Website"/>
  </a>
</p>

<p align="center">
  A clean, responsive personal portfolio and CV website built with vanilla HTML, CSS, and JavaScript. Features live GitHub project integration, a contact form powered by EmailJS, downloadable CV, and a custom 404 page.
</p>

---

## 🌐 Live Demo

> **[https://readytow0rk.github.io/personal-cv-website/](https://readytow0rk.github.io/personal-cv-website/)**

The site is hosted on **GitHub Pages** and is publicly accessible. All pages are fully functional including the live GitHub projects explorer.

---

## Table of Contents

- [Features](#features)
- [Pages](#pages)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [External Integrations](#external-integrations)
- [Getting Started](#getting-started)
- [Author](#author)

---

## Features

- **Responsive Design** — adapts seamlessly across mobile, tablet, and desktop viewports
- **Live GitHub Integration** — search any GitHub username and view profile info and repositories in real time
- **Dynamic Skill Bars** — visual representation of technical skills with color-coded progress indicators
- **Downloadable CV** — one-click PDF download directly from the site and footer
- **Contact Form** — email delivery via EmailJS without a dedicated backend
- **Work History Timeline** — chronological career timeline with visual markers
- **Custom 404 Page** — friendly error page that guides users back home
- **Consistent Color Theme** — cohesive palette across all pages with per-section accent colors

---

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | [index.html](index.html) | Landing page with personal info and "About Me" section |
| Resume | [resume.html](resume.html) | Work history timeline and technical skills with progress bars |
| GitHub | [github.html](github.html) | Live GitHub profile and repository search via GitHub API |
| Contact | [contact.html](contact.html) | Project inquiry form powered by EmailJS |
| 404 | [404.html](404.html) | Custom not-found error page |

---

## Tech Stack

### Core
- **HTML5** — semantic markup with proper meta tags and PWA manifest
- **CSS3** — custom stylesheets, transitions, transforms, and Flexbox layout
- **JavaScript (ES5/ES6)** — DOM manipulation, API calls, and event handling

### Libraries & Frameworks
| Library | Version | Purpose |
|---------|---------|---------|
| Bootstrap | 4.2.1 | Responsive grid and components |
| jQuery | 3.2.1 | DOM manipulation and AJAX requests |
| Font Awesome | 4.7.0 | Icons for navigation and social links |
| Hover.css | 2.3.1 | CSS hover animation effects |
| EmailJS | 3.x | Email delivery without a server |

---

## Project Structure

```
personal-cv-website/
├── index.html              # Home / landing page
├── resume.html             # Resume & skills page
├── github.html             # GitHub projects explorer
├── contact.html            # Contact form
├── 404.html                # Custom error page
├── .gitignore
├── .gitpod.yml             # Gitpod cloud IDE config
├── .gitpod.dockerfile      # Gitpod Docker image
└── assets/
    ├── css/
    │   ├── style.css           # Main stylesheet
    │   └── github-styles.css   # GitHub page styles
    ├── js/
    │   ├── send-email.js       # EmailJS contact form handler
    │   ├── github-information.js # GitHub API integration
    │   └── maps.js             # Google Maps initialisation
    ├── images/
    │   ├── Nikita.jpg          # Profile photo
    │   ├── favicon.ico
    │   ├── apple-touch-icon.png
    │   ├── android-chrome-*.png
    │   └── site.webmanifest    # PWA manifest
    └── cv/
        └── sample-cv.pdf       # Downloadable CV
```

---

## External Integrations

### GitHub API
The GitHub page fetches live data using the public GitHub REST API — no authentication required.

- **User endpoint:** `GET /users/{username}`
- **Repos endpoint:** `GET /users/{username}/repos`
- Handles 404 (user not found), 403 (rate limit exceeded), and generic API errors gracefully
- Rate limit: 60 unauthenticated requests per hour

### EmailJS
Contact form submissions are delivered via [EmailJS](https://www.emailjs.com/) — no backend required.

- Collects: project request details, sender name, and sender email
- Prevents default form submission to avoid page reload

### Google Maps API
A `maps.js` file initialises a Google Map with marker clustering — available for future integration.

---

## Getting Started

This is a fully static website — no build step or package manager required.

**Option 1 — Open directly in browser:**
```bash
open index.html
```

**Option 2 — Serve locally with Python:**
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

**Option 3 — Use the VS Code Live Server extension:**

Right-click `index.html` → *Open with Live Server*

**Option 4 — Cloud IDE via Gitpod:**

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/readytow0rk/personal-cv-website)

> No dependencies to install. All libraries are loaded from CDN.

---

## Author

**Nikita Drozdov** — Full Stack Developer

- GitHub: [@readytow0rk](https://github.com/readytow0rk)
- LinkedIn: [nikita-drozdov-043776258](https://www.linkedin.com/in/nikita-drozdov-043776258/)
- Email: caspi.ready@gmail.com
