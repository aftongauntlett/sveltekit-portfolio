# SvelteKit Portfolio

[![Commit Activity](https://img.shields.io/github/commit-activity/m/aftongauntlett/sveltekit-portfolio)](https://github.com/aftongauntlett/sveltekit-portfolio/commits)
![SvelteKit](https://img.shields.io/badge/SvelteKit-%23ff3e00.svg?style=flat&logo=svelte&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)

My personal developer portfolio, built with SvelteKit, Tailwind CSS, and a custom HSL-based theming system. Scaffolded using my own [sveltekit-starter](https://github.com/aftongauntlett/sveltekit-starter), designed for fast, accessible front-end builds.

## Features

- **SvelteKit** with file-based routing and SSR support
- **Tailwind CSS v4.1** with fluid `clamp()`-based typography and spacing
- **Custom Theme System** using CSS variables and a hex-to-HSL sync script
- **Animated Dark Mode Toggle** using CSS + icon layers
- **Reusable Components** – `Section`, `ProjectCard`, `HeroCard`, and more
- **Accessible Design** using semantic HTML and keyboard-safe interaction
- **Mobile-First Layout** with smooth transitions and responsive design

## Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/aftongauntlett/sveltekit-portfolio.git
cd sveltekit-portfolio
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run the Dev Server

```bash
npm run dev
```

Visit `http://localhost:5173` in your browser to view the site locally.

## Theme Sync Scripts

This project uses a design tooling system that converts hex values in `color-preview.css` into synced HSL values in `theme.css` for consistent theming.

- `npm run watch-theme` — auto-syncs on save
- `npm run sync-theme` — manual one-time sync

## Folder Structure (Relevant Parts)

```
src/
  lib/
    components/
      HeroCard.svelte
      ProjectCard.svelte
      Section.svelte
    styles/
      color-preview.css
      theme.css
  routes/
    +layout.svelte
    +page.svelte        # Homepage
    about/+page.svelte
    contact/+page.svelte
```

## License

MIT License

Copyright (c) 2025 Afton Gauntlett

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
IN THE SOFTWARE.
