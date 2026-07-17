# Srinath Avula — Portfolio

A dark-themed, animated personal portfolio for **Srinath Avula**, QA Automation Test Engineer, built with React, TypeScript, Vite, and Tailwind CSS.

**Live site:** _https://srinathavula.github.io/Srinath-portfolio-website/_

![Tech](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)
![Tech](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Tech](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white)
![Tech](https://img.shields.io/badge/TailwindCSS-4-06B6D4?logo=tailwindcss&logoColor=white)
![Tech](https://img.shields.io/badge/Framer%20Motion-11-0055FF?logo=framer&logoColor=white)

---

## ✨ Features

- **Always-dark UI** with an electric-blue accent theme, `Inter` + `Space Mono` typography, and a custom scrollbar.
- **Interactive cursor effect** — three gravity-lagging stars that chase the mouse across a fixed canvas overlay.
- **Scroll-aware navbar** that goes from transparent to a blurred glass bar on scroll.
- **Section-based layout** — Hero, Summary, Work Experience, Projects, Skills, and Education & Certifications — each with `whileInView` fade-up animations via Framer Motion.
- **Fully responsive**, mobile-first design.
- **Zero backend** — a single static bundle, deployable anywhere that serves static files.

## 🧱 Tech Stack

| Layer            | Tooling                                  |
|-------------------|-------------------------------------------|
| Framework          | React 18 + TypeScript                    |
| Build tool         | Vite 5                                   |
| Styling            | Tailwind CSS v4 (CSS-first `@theme` config) |
| Animation          | Framer Motion                            |
| Icons              | Lucide React                             |
| Fonts              | Google Fonts — Inter (sans), Space Mono (mono) |

## 📁 Project Structure

```
src/
├── main.tsx              # App entry point
├── App.tsx                # Root layout — assembles all sections + footer
├── index.css               # Tailwind import, theme tokens, scrollbar styling
└── components/
    ├── Navbar.tsx           # Fixed, scroll-aware nav
    ├── Hero.tsx              # Landing section — intro, contact chips, photo
    ├── Summary.tsx            # Professional summary (also exports SectionHeading)
    ├── Experience.tsx          # Work experience timeline
    ├── Projects.tsx             # Project card grid
    ├── Skills.tsx                # Technical skills grid
    ├── Education.tsx              # Education & certifications
    ├── GravityStars.tsx            # Canvas-based cursor-chasing stars effect
    └── ThankYou.tsx                 # Closing / contact CTA section

public/
└── srinath.jpeg            # Profile photo
```

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) 18+
- npm (bundled with Node)

### Installation

```bash
git clone https://github.com/Srinathavula/<repo-name>.git
cd <repo-name>
npm install
```

### Development

```bash
npm run dev
```

Opens the site locally with hot-reload, typically at `http://localhost:5173`.

### Production Build

```bash
npm run build
```

Outputs a static, production-ready bundle to `dist/`.

### Preview the Production Build

```bash
npm run preview
```

## 🎨 Customization

- **Colors / theme tokens** — edit the `@theme` block in `src/index.css` (all colors are HSL-based CSS variables: `--color-background`, `--color-primary`, etc.).
- **Content** — each section's copy and data lives directly in its component file (e.g. project cards in `src/components/Projects.tsx`, skills in `src/components/Skills.tsx`).
- **Profile photo** — replace `public/srinath.jpeg` with your own image, keeping the same filename (or update the `src` path in `Hero.tsx`).

## 📦 Deployment

This is a static site and can be deployed to any static host:

- **Vercel** — import the repo, framework preset `Vite`, no extra config needed.
- **Netlify** — build command `npm run build`, publish directory `dist`.
- **GitHub Pages** — build locally and push the `dist/` output to a `gh-pages` branch (or use an action like `peaceiris/actions-gh-pages`).

## 📄 License

This project is personal portfolio code. Feel free to fork it for inspiration, but please don't republish it as your own personal site content.

## 🙋 Contact

- **Email:** avulasrinath225@gmail.com
- **Phone:** +91 6281358815
- **LinkedIn:** [linkedin.com/in/srinathavula](https://linkedin.com/in/srinathavula)
- **GitHub:** [github.com/Srinathavula](https://github.com/Srinathavula)

---

**Designed & Built by Srinath Avula.**
