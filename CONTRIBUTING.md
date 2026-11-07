# Contributing to the WAMEEDH Website

Thank you for your interest in contributing to the **WAMEEDH Scientific Club** website! Whether you are a club member, a web lead, or a student developer, your contributions help keep the spark alive.

---

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone git@github.com:Wameeedh/Wameedh-website.git
   cd Wameedh-website
   ```

2. **Run locally:**
   Because the website uses a zero-build static architecture, you can run it immediately with any static server:
   ```bash
   # Using Node
   npm start
   # or using Python
   npm run serve:python
   # or simply double-click index.html in your browser!
   ```

---

## 🛠️ Architecture & Conventions

- **Self-Contained Single-File Design:** `index.html` holds the markup, styles, scripts, fonts, and inline graphical assets. This guarantees instant deployment on GitHub Pages or any static CDN with zero dependencies.
- **Routing:** Hash-based routes (`#/home`, `#/about`, `#/departments`, `#/projects`, `#/events`, `#/events/bootcamp`, `#/events/art`, `#/events/holytech`, `#/archive`, `#/board`, `#/join`).
- **Theming:** Night (default dark ambient theme) and Frostlight Day (`body.day`).

---

## 📝 Submitting Changes

1. Create a descriptive branch:
   ```bash
   git checkout -b feature/update-workshops
   ```
2. Test your changes locally on multiple screen sizes (desktop, tablet, mobile).
3. Commit your changes with clear commit messages:
   ```bash
   git commit -m "Add details for upcoming Arduino Bootcamp edition"
   ```
4. Push to your branch and open a Pull Request.

---

## 🤝 Questions & Mentorship

If you are a new member or future web lead looking for guidance, feel free to reach out to the project maintainers listed in the [README](README.md#maintainer--handover-contact).
