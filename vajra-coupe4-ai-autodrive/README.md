# Vajra Coupe‑4 — Configurator & Immersive Test Drive

An interactive, single-page 3D car configurator and "immersive test drive" experience for the **Vajra Coupe‑4**, built with [Three.js](https://threejs.org/) and [GSAP](https://greensock.com/gsap/).

## ✨ Features

- Real-time 3D car viewer (WebGL via Three.js r128)
- Color / trim configurator
- Cinematic camera moves and scroll-triggered animations (GSAP + ScrollTrigger)
- Post-processing effects (bloom, SSAO, bokeh depth-of-field, FXAA)
- Accessibility touches: visible keyboard focus states, `prefers-reduced-motion` support, WebGL-unavailable fallback screen
- Fully responsive, mobile-friendly layout

## 🚀 Getting started

This is a static, single-file site — no build step required.

### Option 1: Open directly
Just open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari).

> Note: some browsers restrict certain features (like fetch/module loading) when opening HTML files directly via `file://`. If you run into issues, use a local server instead (see below).

### Option 2: Run a local server
```bash
# Python 3
python -m http.server 8000

# or Node.js
npx serve .
```
Then visit `http://localhost:8000` in your browser.

## 🌐 Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to `Deploy from a branch`.
4. Choose the `main` branch and `/ (root)` folder, then save.
5. Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

## 🧰 Tech stack

- [Three.js](https://threejs.org/) `r128` (WebGL rendering, orbit controls, post-processing passes)
- [GSAP](https://greensock.com/gsap/) `3.12.2` + ScrollTrigger (animation)
- Vanilla HTML/CSS/JS — Google Fonts: Fraunces, Inter, JetBrains Mono
- All dependencies are loaded via CDN (cdnjs / jsdelivr) — no `npm install` needed

## 📁 Project structure

```
.
├── index.html      # entire app: markup, styles, and script
├── README.md
├── LICENSE
└── .gitignore
```

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
