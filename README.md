# EcoSmart

A full-stack web application for **EcoSmart** — a Saudi company delivering construction systems, decoration, and finishing products. Aligned to Vision 2030 and the Saudi Building Code.

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | [TanStack Start](https://tanstack.com/start) (React 19, SSR) |
| Routing | [TanStack Router](https://tanstack.com/router) |
| Styling | [Tailwind CSS v4](https://tailwindcss.com) |
| UI Components | [shadcn/ui](https://ui.shadcn.com) + [Radix UI](https://www.radix-ui.com) |
| Animations | [Framer Motion](https://www.framer.com/motion) + [GSAP](https://gsap.com) |
| Data Fetching | [TanStack Query](https://tanstack.com/query) |
| Build Tool | [Vite](https://vite.dev) |
| Language | TypeScript |

## Getting Started

### Prerequisites

- [Node.js 20+](https://nodejs.org) — install via [nvm](https://github.com/nvm-sh/nvm#installing-and-updating)
- npm or bun

### Install & Run

```sh
git clone <repository-url>
cd section-shine-flow

npm install
npm run dev
```

The dev server starts at `http://localhost:3000`.

### Available Scripts

| Script | Description |
|---|---|
| `npm run dev` | Start development server with HMR |
| `npm run build` | Production build (outputs to `.output/`) |
| `npm run preview` | Preview the production build locally |
| `npm start` | Run the production server (`node .output/server/index.mjs`) |
| `npm run lint` | Run ESLint |
| `npm run format` | Format code with Prettier |

## Project Structure

```
src/
├── components/     # Reusable UI components
├── data/           # Static data and content
├── hooks/          # Custom React hooks
├── lib/            # Utilities and helpers
├── routes/         # File-based routes (TanStack Router)
├── styles.css      # Global styles + Tailwind base
├── router.tsx      # Router configuration
└── server.ts       # SSR server entry point
```

## Deployment

Build the project then serve the output:

```sh
npm run build
npm start          # node .output/server/index.mjs
```

The `.output/` directory is self-contained and can be deployed to any Node.js host (VPS, Railway, Fly.io, etc.).
