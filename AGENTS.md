# Dashboard 1: project identity

- Only edit `/Users/hakam/Documents/ChatGPT/dashboard-1` for Dashboard 1. This is an independent repository; never copy another dashboard's app, styles, assets, dependencies, or Vercel configuration into it.
- Design: Original six-card dashboard. Preserve this dashboard's own visual authority and user-approved changes.
- GitHub: `Hakam02-doom/dashboard-one`. Vercel project: `dashboard-one`. Identity is recorded in `dashboard.config.json`.
- Development: `npm run dev` → `http://127.0.0.1:5173/`. Production preview: `npm run preview` → port 4173. Ports are fixed and do not fall back.
- Before work, run `npm run check:project`. Before publishing, run `npm run build` and `npm run test:isolation`. Use `npm run deploy` for an authorized production deployment. Never override the port, working directory, or Vercel target.
- New clones: run `npm install` to install the repository's own dependencies and pre-push guard. Do not share node_modules or use a parent dashboard's installation.
- The old `/Users/hakam/Documents/ChatGPT/dashboard` folder is a routing index, not an application. Do not implement anything there.
