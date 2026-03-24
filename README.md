# Motile Website

Landing page and marketing website for Motile.

## Tech Stack

- **Framework**: [Astro](https://astro.build) — fast, SEO-friendly, island architecture
- **Styling**: [Tailwind CSS](https://tailwindcss.com) — utility-first CSS
- **Language**: TypeScript (strict mode)
- **Deploy**: GitHub Pages via GitHub Actions

## Local Development

### Prerequisites

- Node.js 20+
- npm 9+

### Setup

```bash
npm install
npm run dev
```

The dev server starts at `http://localhost:4321`.

### Build

```bash
npm run build       # production build → dist/
npm run preview     # preview the production build locally
```

## Project Structure

```
src/
├── components/
│   ├── Hero.astro          # Main headline, subheadline, CTAs
│   ├── Features.astro      # Key features / benefits grid
│   ├── ThemeShowcase.astro # Product screenshots or demo
│   ├── HowItWorks.astro    # Numbered steps / onboarding flow
│   └── Footer.astro        # Nav links, social, legal
├── layouts/
│   └── Layout.astro        # Base HTML shell with SEO meta tags
├── pages/
│   └── index.astro         # Home page — composes all sections
└── styles/
    └── global.css          # Tailwind directives + global styles
```

## Deployment

The site deploys automatically to GitHub Pages on every push to `main` via `.github/workflows/deploy.yml`.

### Manual deploy

1. Go to the repo on GitHub
2. Navigate to **Actions** > **Deploy to GitHub Pages**
3. Click **Run workflow**

### First-time GitHub Pages setup

1. Go to **Settings** > **Pages**
2. Under **Source**, select **GitHub Actions**
3. Push to `main` — the workflow handles the rest

## Contributing

All section components include `// TODO` comments marking content that needs to be replaced with real Motile copy, images, and links.
