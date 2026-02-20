# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Static marketing website for Flatiron Kids mobile apps. Built with Astro, Tailwind CSS 4, and deployed as a static site.

## Commands

- `pnpm dev` — start dev server
- `pnpm build` — production build (outputs to `dist/`)
- `pnpm preview` — preview production build locally

## Architecture

- **Astro** static site (no SSR, no client-side JS)
- **Tailwind CSS 4** via `@tailwindcss/vite` plugin, with `@tailwindcss/typography` for prose content
- Custom brand colors defined as `--color-brand-*` and `--color-accent-*` in `src/styles/global.css`

### File Structure

- `src/layouts/Base.astro` — shared layout with nav, footer, meta tags, font loading
- `src/pages/index.astro` — landing page
- `src/pages/privacy.astro` — privacy policy (COPPA-compliant template)
- `src/styles/global.css` — Tailwind imports, typography plugin, brand color theme
- `public/FlatironKids/` — logo assets (A1=white, A2=red, A3=green full-color)

### Brand

- Logo: mountain silhouette with sun circle, "FLATIRONKIDS" text
- Primary color: crimson red (`--color-brand-500: #b91c1c`)
- Accent color: olive green (`--color-accent-500: #7ba32a`)
- A2 variant is the default logo used on the site
