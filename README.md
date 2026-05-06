# Tracker App

`tracker-app` is a standalone frontend showcase built from the extracted Uber-style UI in `/home/dev/Desktop/suru se suru/uber/frontend`.

## What It Is Now

- Frontend-only demo app
- No backend required
- Local mock authentication and profile storage
- Rider and captain showcase flows
- Testing buttons that simulate booking, matching, trip progress, demand, and earnings states

## Demo Features

- Home screen includes instant rider and captain showcase launchers
- Login and signup screens support demo autofill and one-click preview
- Rider dashboard includes scenario buttons for office, airport, and night surge flows
- Captain dashboard includes online/offline simulation and trip-state controls
- All demo data is stored in `localStorage`, so the app works fully offline after install

## Architecture

- `src/services/api.js`: mock async service layer replacing backend APIs
- `src/context/UserContext.jsx`: rider session storage
- `src/context/CaptainContext.jsx`: captain session storage
- `src/pages/UserHome.jsx`: rider demo interactions and booking showcase
- `src/pages/CapitanHome.jsx`: captain demo interactions and earnings showcase

## Run

```bash
npm install
npm run dev
```

## Netlify

- Build command: `npm run build`
- Publish directory: `dist`
- SPA routing is configured in `netlify.toml`

## Reset Demo Data

Use the `Reset Demo Data` button on the landing page to restore default demo users and clear active sessions.
