## Independent workspace

- Only edit `/Users/hakam/Documents/ChatGPT/dashboard-1` for Dashboard 1. This is an independent repository; never copy another dashboard's app, styles, assets, dependencies, or Vercel configuration into it.
- Design: Original six-card dashboard. Preserve this dashboard's own visual authority and user-approved changes.
- GitHub: `Hakam02-doom/dashboard-one`. Vercel project: `dashboard-one`. Identity is recorded in `dashboard.config.json`.
- Development: `npm run dev` → `http://127.0.0.1:5173/`. Production preview: `npm run preview` → port 4173. Ports are fixed and do not fall back.
- Before work, run `npm run check:project`. Before publishing, run `npm run build` and `npm run test:isolation`. Use `npm run deploy` for an authorized production deployment. Never override the port, working directory, or Vercel target.
- New clones: run `npm install` to install the repository's own dependencies and pre-push guard. Do not share node_modules or use a parent dashboard's installation.
- The old `/Users/hakam/Documents/ChatGPT/dashboard` folder is a routing index, not an application. Do not implement anything there.

# Dashboard One

A static, responsive Uplift AI workspace adapted from the supplied screenshot. The six-card home overview, white canvas, navy rail, Inter typography, pastel charts, and restrained entrance motion are preserved. The screenshot's outer cyan frame has been removed.

The homepage contains only the original six-card overview. The sidebar stays anchored to the viewport while page content scrolls; the shell uses overflow clipping without creating a separate scroll container. The expanded feature views remain accessible through navigation. It includes 30 routes across Home, SEO, AI Visibility, Google Business, Social Media, Setup, and Settings. Article review, filtering, local editing, calendar navigation, keyword planning, social captions, profile forms, appearance preferences, search, sharing, and CSV export work in the preview. Light and dark modes share semantic foreground tokens; dark mode also themes native controls, chart labels, and the publishing-readiness panel.

## Preview data

The original application exposed LunchLink as the active workspace and Uplift AI as unfinished setup. The user chose Uplift AI. Therefore this draft uses Uplift AI content themes and clearly labeled illustrative metrics, rather than importing LunchLink's catering articles or reporting. No live analytics, AI scans, publishing connections, account data, or backend integrations are connected. Connection-dependent screens use explicit setup/empty states.

Article edits, keyword plans, social topics, business/author profiles, and preferences are saved in this browser's local storage. They do not modify the original application or publish content. Google Fonts is the only external presentation dependency, with an Arial fallback.

## Hosting

Dashboard One is configured as a static Vercel project. The deployed output is `dist`; no build command or framework is required.

## Running

Serve `dist` with any static web server. No build or package installation is required. Entry: `dist/index.html`.

## Validation

- JavaScript syntax checked.
- All 30 route renderers and internal route links checked.
- Browser checks of navigation, article filtering/review/save, and keyword planning/calendar behavior.
- Desktop, mobile, and the app's 934px viewport reviewed.

Sources: user-supplied screenshot; https://www.upliftai.co/; authenticated read-only inspection of https://dashboard.upliftai.co/dashboard/home and its navigation.
