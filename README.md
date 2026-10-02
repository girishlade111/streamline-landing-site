<div align="center">

# 🚀 Streamline — Enterprise Landing Page

**A modern, high-performance marketing landing page for enterprise software solutions.**
Built with Next.js 15, React 19, TypeScript, Tailwind CSS & shadcn/ui — featuring fluid
animations, a responsive design, SEO optimization, and fully static export so it deploys
anywhere (Cloudflare Pages, GitHub Pages, Netlify).

[![Next.js](https://img.shields.io/badge/Next.js-15.2.8-000000?style=flat-square&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-06B6D4?style=flat-square&logo=tailwindcss)](https://tailwindcss.com/)
[![shadcn/ui](https://img.shields.io/badge/shadcn/ui-latest-000000?style=flat-square)](https://ui.shadcn.com/)

</div>

---

## 📖 Table of Contents

- [📋 Project Overview](#-project-overview)
- [✨ Features](#-features)
- [🛠️ Tech Stack](#-tech-stack)
- [🚀 Quick Start](#-quick-start)
- [📁 Project Structure](#-project-structure)
- [⚙️ Environment Variables](#️-environment-variables)
- [📦 Deploy](#-deploy)
- [👤 Author](#-author)
- [📄 License](#-license)

## 📋 Project Overview

Streamline is a conversion-focused landing page for an enterprise software company.
It showcases AI analytics, cloud-native architecture, and cybersecurity offerings
across dedicated pages (company, services, solutions, pricing, resources) with
polished animations and an SEO-first setup. A documented `SEO_STRATEGY.md` describes
the organic-search plan for this site.

## ✨ Features

- Multi-page marketing site — home, company, services, solutions, pricing, resources
- Fluid scroll-based and entrance animations (Framer Motion)
- Fully responsive, mobile-first layouts
- SEO-optimized metadata, Open Graph tags, and a documented SEO strategy
- shadcn/ui component library (Radix primitives) for accessible UI
- Fully static export (`output: 'export'`) — zero server cost to host

## 🛠️ Tech Stack

- **Framework:** Next.js 15.2.8 (static export), React 19, TypeScript
- **Styling:** Tailwind CSS 3.4, shadcn/ui, Radix UI primitives
- **Animation:** Framer Motion
- **Fonts:** Geist (next/font)
- **Analytics:** @vercel/analytics

## 🚀 Quick Start

Prerequisites: Node.js 18+ and npm.

```bash
# 1. Install dependencies
npm install --legacy-peer-deps

# 2. Start the dev server
npm run dev
# open http://localhost:3000

# 3. Production static build (outputs to dist/)
npm run build
```

The production site is fully static — serve the `dist/` folder from any static host.

## 📁 Project Structure

```
.
├── app/                 # Next.js App Router pages
│   ├── company/         # Company page
│   ├── pricing/         # Pricing page
│   ├── resources/       # Resources page
│   ├── services/        # Services page
│   ├── solutions/       # Solutions page
│   ├── layout.tsx       # Root layout + metadata
│   └── page.tsx         # Home page
├── components/          # Reusable UI components (shadcn/ui + custom)
├── lib/                 # Utilities
├── public/              # Static assets
├── styles/              # Global styles
├── next.config.mjs      # Static-export config (output: 'export', distDir: 'dist')
├── SEO_STRATEGY.md      # SEO plan for this site
└── tailwind.config.js   # Tailwind theme
```

## ⚙️ Environment Variables

No environment variables are required. The site is fully static and client-side.
Vercel Analytics (`@vercel/analytics`) is included but works without configuration.

## 📦 Deploy

Because the site uses `output: 'export'`, the build (`npm run build`) produces a
`dist/` directory you can deploy to any static host:

- **Cloudflare Pages:** `cloudflare pages_deploy streamline-landing-site dist/`
- **Netlify:** drop `dist/` into a new site
- **GitHub Pages:** publish `dist/` contents

No server, no functions, no database.

## 👤 Author

Built by [Girish Lade](https://ladestack.in) — founder of
[LadeStack](https://ladestack.in), building free, open, and local-first software.

## 📄 License

MIT — free to use, modify, and share.
