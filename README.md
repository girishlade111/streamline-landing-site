# Streamline Landing Site

A modern, high-performance Next.js 15 landing page for enterprise software solutions — featuring AI analytics, cloud-native architecture, and cybersecurity offerings with fluid animations, responsive design, and SEO optimization.

## Features

- **Hero section** with animated headline, CTA, and product visuals
- **Feature showcase** — AI analytics, cloud-native architecture, cybersecurity cards
- **Pricing, testimonials, FAQ, and CTA sections**
- **Fluid animations** powered by Framer Motion (scroll reveals, parallax, micro-interactions)
- **Dark/light theming** via next-themes
- **SEO optimized** — metadata, OpenGraph tags, sitemap-friendly structure
- **Fully responsive** mobile-first design
- **shadcn/ui component library** — accordion, dialog, dropdowns, carousel, forms, charts

## Tech Stack

- **Framework:** Next.js 15 (App Router, static export)
- **Language:** TypeScript
- **UI:** React 19, Tailwind CSS, shadcn/ui (Radix primitives)
- **Animation:** Framer Motion
- **Charts:** Recharts
- **Forms:** React Hook Form + Zod
- **Analytics:** Vercel Analytics

## Quick Start

```bash
npm install --legacy-peer-deps
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

## Project Structure

```
app/            # Next.js App Router pages, layout, metadata
components/     # Landing sections + shadcn/ui components
lib/            # Utilities (cn helper)
styles/         # Global styles
public/         # Static assets
```

## Build & Deploy

The site is a fully static export:

```bash
npm run build     # outputs to dist/
```

Deploy the `dist/` folder to any static host (Cloudflare Pages, GitHub Pages, Netlify, Vercel).

## Notes

- `output: "export"` with `images.unoptimized` in `next.config.mjs` enables pure static hosting.
- TypeScript and ESLint errors are ignored during builds (`ignoreBuildErrors: true`).

## Author

Built by Girish Lade — [ladestack.in](https://ladestack.in)
