# WAMEEDH — Keep the Spark Alive

A responsive, single-file website for **WAMEEDH Scientific Club**, associated with IGEE / ex INELEC in Boumerdes, Algeria. The design pairs a dark, atmospheric visual style with club stories, event photography, member profiles, and an interactive exhibition.

## Features

- Home, About, Departments, Projects, Join, Events, Archive, and Board views.
- Event highlights and photo albums for Arduino Bootcamp, ART, HolyTech 2.0, and C Hackathon.
- Member and event carousels with manual navigation and optional autoplay.
- Living Exhibition with Members, Events, or combined playlists; pause, previous/next, and fullscreen controls.
- Subtle scroll-driven particle effects that do not replace or cover photographs.
- Light/dark theme and motion controls, plus support for reduced-motion preferences.
- Responsive navigation, search, and contact/social links.
- Embedded images, fonts, styles, and scripts: no package installation or build step.

## Repository structure

```text
.
├── index.html    # Complete website, including embedded assets
└── README.md     # Project documentation
```

## Run locally

Open `index.html` in a modern browser, or serve the repository with Python:

```bash
python3 -m http.server 8000
```

Then visit **http://localhost:8000**. No Node.js or npm dependencies are required.

## Publish with GitHub Pages

1. Create a GitHub repository and upload `index.html` and `README.md` to its root.
2. Open the repository’s **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Choose your default branch (usually `main`) and **/ (root)**, then save.
5. When deployment finishes, open the site URL shown in the Pages settings.

Keep the website filename as `index.html` so Pages serves it as the homepage. Navigation uses hash routes such as `#/events`, so it does not require server-side routing or a custom 404 page.

## Customize

The project is intentionally bundled in one HTML file. Back it up before editing.

| Change | Where to look in `index.html` |
| --- | --- |
| Page content and navigation | HTML sections and `data-view` attributes |
| Layout, colors, typography | Inline `<style>` blocks |
| Club members and photo archive | The embedded `DATA` object and `window.wameedhFinal` |
| Particle appearance and motion | `window.WAMEEDH_FX_CONFIG` |
| Exhibition timing and playback | `WAMEEDH_FX_CONFIG.exhibition` |
| Contact and social destinations | `mailto:` links and social anchors |

### Particle settings

The current version keeps original photographs fully visible, excludes photo regions from the particle overlay, disables particle rendering during photo-shaped timeline segments, and removes carousel blur. Particle paths are deterministic rather than continuously shifting with wall-clock time.

To disable particles by default, set `enabled: false` in `window.WAMEEDH_FX_CONFIG`. Visitors can also use the on-page particle and motion controls.

### Exhibition controls

- Use the on-screen previous, next, and pause/resume buttons.
- **Left / Right arrows:** switch slides.
- **Space:** pause/resume when focus is not on an interactive control.
- **Esc:** close the exhibition.
- **Fullscreen:** request fullscreen when supported by the browser.

## Technology

- HTML, CSS, and vanilla JavaScript.
- Embedded Three.js for WebGL particles.
- Embedded GSAP and ScrollTrigger for scroll animation.
- Browser Web Animations API for exhibition transitions.

## Browser and performance notes

Use a recent Chrome, Edge, Firefox, or Safari release. WebGL is needed for particle effects; when it is unavailable, the normal site content remains accessible. Fullscreen availability depends on the browser and embedding context.

The HTML file is approximately **14 MB** because media and libraries are embedded. This makes the site easy to move and host, but can increase initial load time. For a future production optimization, consider extracting media into an `assets/` directory and serving appropriately sized images separately.

## Pre-publication checklist

- Verify club member details, contact information, social links, and event dates.
- Confirm permission to publish the photographs, names, club branding, and other supplied assets.
- Test navigation, search, carousels, exhibition playback, and contact links.
- Check mobile layouts and reduced-motion mode.
- Review the licenses and notices for bundled third-party libraries before redistribution.

## License and credits

No project-wide license is specified in this repository. Add a `LICENSE` file only after deciding which rights you can grant. Club media, branding, and bundled third-party code may have separate rights and license terms; preserve the third-party notices in the HTML.
