# WAMEEDH Scientific Club — Official Website

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-2ea44f?logo=github)](https://github.com/Wameeedh/Wameedh-website)
[![Stack](https://img.shields.io/badge/Stack-HTML5%20%7C%20Modern%20CSS%20%7C%20Vanilla%20JS-F7DF1E?logo=javascript&logoColor=black)](#tech-stack--architecture)
[![Zero Build](https://img.shields.io/badge/Build-Zero%20Dependency-brightgreen)](#zero-build-architecture)
[![Organization](https://img.shields.io/badge/Organization-WAMEEDH-080c12?logo=github)](https://github.com/Wameeedh)

### *A spark is only the beginning.*
**Learn by doing. Build together. Share what works.**

[Explore Features](#key-features) • [Local Preview](#quick-start--local-development) • [Architecture](#tech-stack--architecture) • [Handover Guide](#guide-for-future-generations-handover) • [About the Club](#about-wameedh-scientific-club) • [Maintainer](#maintainer--handover-contact)

---

</div>

## 🌐 Overview

This repository hosts the **official interactive web platform** for **WAMEEDH Scientific Club**, established at the **Institute of Electrical & Electronic Engineering (IGEE, formerly INELEC)**, **University of M’Hamed Bougara, Boumerdes, Algeria**.

Designed to embody the spirit of innovation and hands-on engineering, the website acts as both a living digital exhibition of the club’s journey and an interactive hub for students, members, and external partners.

---

## ✨ Key Features

- 🌟 **Living Interactive Exhibition:** An immersive multimedia showcase of club moments, past editions, workshops, and milestones with dynamic camera transitions, particle emitters, and modal navigation.
- 🌓 **Dual Atmospheric Theme Engine:**
  - **Ambient Night (Default):** Deep obsidian background with warm luminous accents, designed for low-light focus and high-contrast visuals.
  - **Frostlight Day:** A refined mineral-blue day theme with subtle gradients, soft glassmorphism, and daylight readability.
- ⚡ **Interactive Particle & Canvas FX:** Custom canvas animation system rendering ambient sparks that react to user interaction, echoing the *Wameedh* (*spark*) identity.
- 🔊 **Soundscape Experience:** Embedded audio ambiance and subtle sound feedback that brings life to user interactions (with user control and reduced-motion respect).
- 🧭 **Hash-Based Deep Navigation:** Fast client-side routing supporting direct links to key views:
  - `#/home` — Main hero portal and overview.
  - `#/about` — Club identity, values, and story.
  - `#/departments` — Deep dive into the 6 specialized club divisions.
  - `#/projects` — Embedded hardware, robotics, AI, and software portfolio.
  - `#/events` — Signature bootcamps, hackathons, and training series (`#/events/bootcamp`, `#/events/art`, `#/events/holytech`).
  - `#/archive` — Historic timeline and retrospective gallery.
  - `#/board` & `#/join` — Community pathways, recruitment, and contact dialogs.
- 📱 **Responsive & Mobile Optimized:** Touch-friendly drawers, safe-area inset adaptation for modern mobile displays, and accessible keyboard navigation.
- 🚀 **Zero-Build Self-Contained Architecture:** Engineered to run with zero compiler steps or complex package dependencies. Everything required to run the site is self-contained.

---

## 🗂️ Project Structure

```text
Wameedh-website/
├── .github/
│   ├── workflows/
│   │   └── deploy.yml              # Automated GitHub Pages CI/CD workflow
│   └── PULL_REQUEST_TEMPLATE.md    # PR template for club contributors
├── .gitignore                      # Standard project gitignore
├── CONTRIBUTING.md                 # Contribution and workflow guide
├── index.html                      # Core standalone web application (14 MB)
├── LICENSE                         # MIT Open Source License
├── package.json                    # Development scripts and project metadata
└── README.md                       # Complete documentation & handover guide
```

---

## 🏗️ Tech Stack & Architecture

### Zero-Build Architecture
The application is intentionally designed as a high-performance, self-contained single-page application.
- **Embedded Fonts & Graphics:** Web fonts (Wameedh Serif / Sans) and iconography are embedded directly into the document using standard Data URIs, eliminating external CDN latency and avoiding broken asset paths across different hosting environments.
- **Vanilla Modern JavaScript:** No heavy frontend frameworks (React/Vue/Angular) are required. Pure browser APIs handle DOM routing, canvas animations, and modal state management.
- **Modern CSS3:** Features responsive grid layouts, backdrop-filter glassmorphism, CSS custom properties for instant theme toggling, and media queries for dark/light mode and reduced-motion preferences.

---

## 💻 Quick Start & Local Development

No package installation or compilation is required to run the website. You can open and view it using any of the following methods:

### Option 1: Direct Browser Launch
Simply double-click `index.html` or open it with your favorite browser:
```bash
xdg-open index.html   # Linux
open index.html       # macOS
start index.html      # Windows
```

### Option 2: Using npm / Node.js
```bash
# Clone the repository
git clone git@github.com:Wameeedh/Wameedh-website.git
cd Wameedh-website

# Start local dev server (default port: 3000)
npm start
```

### Option 3: Using Python
```bash
python3 -m http.server 3000
# Visit http://localhost:3000 in your browser
```

### Option 4: VS Code Live Server
Open the project directory in VS Code, right-click `index.html`, and select **"Open with Live Server"**.

---

## 🚢 Deployment

### GitHub Pages (Automated via GitHub Actions)
The repository includes [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) configured for automatic deployment:
1. In your GitHub repository settings, navigate to **Settings** → **Pages**.
2. Under **Build and deployment** → **Source**, select **GitHub Actions**.
3. Every push to the `main` branch will automatically build and publish the live site.

### Vercel / Netlify / Static Hosts
Because the entry point is at the root (`index.html`), simply connect the repository to Vercel, Netlify, or Cloudflare Pages. Set the build command to empty and publish directory to `.`.

---

## 📖 About WAMEEDH Scientific Club

**WAMEEDH** is a student-run scientific and technical club at the **Institute of Electrical & Electronic Engineering (IGEE, formerly INELEC)**, **University of M’Hamed Bougara, Boumerdes, Algeria**.

We bring curious students together to turn academic knowledge into practical experience. Through projects, workshops, bootcamps, and shared challenges, we create a space to explore ideas, develop skills, and build things together.

### What We Explore
- **Electronics & Embedded Systems:** Circuits, microcontrollers, PCB design, and hardware prototyping.
- **Robotics & Automation:** Connecting code, sensors, kinematics, and real-time control.
- **Software Engineering & Computer Science:** Modern programming, algorithms, and practical systems development.
- **Artificial Intelligence & Computer Vision:** Exploring intelligent algorithms, computer vision pipelines, and data-driven systems.
- **Internet of Things (IoT):** Connected hardware, sensor networks, telemetry, and smart applications.
- **3D Design & Prototyping:** CAD modeling, 3D printing, and mechanical prototyping.

### Our Core Departments

| Department | Mission & Contribution |
| :--- | :--- |
| **Projects** | Turns questions, research, and ideas into practical engineering systems. |
| **Learning** | Supports skill development through workshops, peer training, and tutorials. |
| **Events** | Creates spaces for engineers to meet, compete, and exchange knowledge. |
| **Logistics** | Powers the organization, technical supplies, and practical needs of club activities. |
| **Media** | Shares the club’s journey and technical impact through visual storytelling. |
| **External Relations** | Bridges the club with sponsors, academic institutions, and industry partners. |

### Signature Club Events
- **Arduino Bootcamp:** A foundational hands-on training series introducing students to electronics, microcontroller programming, and circuit building.
- **ART (Arduino Robotic Training):** Putting theory into motion through robotics design, sensor integration, and autonomous navigation.
- **HolyTech:** An annual flagship tech convention bringing together innovators, technical exhibitions, tech talks, and project competitions.
- **C Hackathon:** An intensive low-level programming hackathon challenging participants to solve complex engineering and algorithmic problems in C.

---

## 🤝 Guide for Future Generations (Handover)

> [!TIP]
> **To incoming Web Leads, Developers, and Club Boards:**  
> This website is built for longevity. Because it does not rely on third-party npm build toolchains that degrade over time, it can be maintained and modified for years to come without dependency conflicts.

### How to Make Common Updates:
1. **Adding or Updating Text & Links:**
   - Open `index.html` in any code editor (VS Code, Neovim, etc.).
   - Search for the section heading or identifier (e.g. `id="events"`, `id="departments"`, `#/events/bootcamp`).
   - Edit the markup directly.
2. **Updating Social Links & Contact Details:**
   - Search for `mailto:` or `instagram.com` inside `index.html` to update communication channels.
3. **Updating the Gallery / Living Exhibition:**
   - The interactive exhibition logic is located within the `<div id="living-exhibition">` structure and corresponding script block near the end of `index.html`.
4. **Theme Customization:**
   - CSS variables for both Night and Day themes are defined in the `<style>` block at the beginning of `index.html` (`:root` and `body.day`).

---

## 📬 Connect With WAMEEDH

- **Email:** [wameedh.sc@gmail.com](mailto:wameedh.sc@gmail.com)
- **Instagram:** [@wameedh.sc](https://www.instagram.com/wameedh.sc/)
- **Facebook:** [WAMEEDH Scientific Club](https://www.facebook.com/wameedh.sc/)
- **LinkedIn:** [WAMEEDH Scientific Club](https://www.linkedin.com/company/wameedh-scientific-club)
- **Official Web Page (IGEE):** [igee.univ-boumerdes.dz/Wameedh_SC.html](https://igee.univ-boumerdes.dz/Wameedh_SC.html)
- **Campus Location:** IGEE (ex-INELEC) · University of M’Hamed Bougara · Boumerdes, Algeria

---

## 👤 Maintainer & Handover Contact

This website and its architecture were built and curated with passion for **WAMEEDH Scientific Club**.

- **Lead Developer & Maintainer:** **Ayoub**
  - **GitHub:** [@99S7CK1GC](https://github.com/99S7CK1GC)
  - **Email:** [ayoubbenbarkat1342@gmail.com](mailto:ayoubbenbarkat1342@gmail.com)

> [!NOTE]
> **A Message to Future Generations of Wameedh Members:**  
> If you are a future club member, webmaster, or board lead taking over the digital assets of Wameedh and you ever need help, have questions about how a particular part of the site works, or need assistance handing over or migrating projects, **please don't hesitate to reach out to me!** You can contact me via email or open an issue/discussion on GitHub. Keep the spark burning! 🔥

---

## 💐 Acknowledgments

- Special thanks to **Chaita Mouhamed Nizar** for his invaluable help, dedication, and contributions to this project.
- Heartfelt appreciation to all past and present Wameedh members, organizers, and mentors who dedicate their time to hands-on learning.

---

<div align="center">

**No spark burns alone. Keep the spark alive.**

</div>
