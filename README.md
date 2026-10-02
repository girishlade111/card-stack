# Card Stack

An interactive card-stack UI built with Next.js — cards fan out in a stack and cycle on click, with smooth spring animations and dark/light theming.

## Features

- **Interactive card stack** — click the top card to send it to the back with a spring animation
- **Framer-motion physics** — spring-based drag and stack transitions
- **Dark/light theme toggle** — theme provider with class-based theming
- **Responsive layout** — centered card stage that scales from mobile to desktop
- **Client-side only** — no backend, no env vars, no API routes

## Tech Stack

- Next.js 15 + TypeScript
- Tailwind CSS + shadcn-style components
- Framer Motion for animations
- Lucide icons

## Quick Start

```bash
npm install
npm run dev      # http://localhost:3000
npm run build    # static export to out/
```

The app is a static export (`output: "export"` in `next.config.mjs`), so it can be hosted on any static host: Cloudflare Pages, GitHub Pages, Netlify, Vercel.

## Project Structure

```
card-stack/
├── app/
│   ├── page.tsx          # Home page — renders <CardStack />
│   ├── layout.tsx        # Root layout + theme provider
│   └── globals.css       # Tailwind + theme tokens
├── components/
│   ├── card-stack.tsx    # The interactive stack component
│   └── theme-provider.tsx
└── public/               # Placeholder images/logos
```

## Deploy

```bash
npm run build
# serve out/ on any static host
```

---

**Built by Girish Lade** — [ladestack.in](https://ladestack.in)
