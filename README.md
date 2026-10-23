# CAM'S STATS — Fresh Build v3

A **new**, dependency-free Node.js sports dashboard. This intentionally replaces the old React/Vite frontend and its overlapping styles and routes.

## Render
Create a **Node Web Service** connected to `urbro1017-max/cams-stats`.

- Build: `npm install && npm run build`
- Start: `npm start`
- Health: `/api/health`
- Node 20+

**Replace all old repository contents** with the files from this folder. Do not nest this folder inside the repository. Do not delete the repository or its history. `npm run build:with-data` is no longer used.

## Features
- NFL and NBA daily scoreboards with team logos, live/final states, date navigation, and historical game details.
- Completed game box scores, scoring plays, and play-by-play when supplied by ESPN.
- Team directories with logos.
- NBA daily fantasy scoring from completed-game box scores, with scoring formula shown.
- Honest NFL fantasy limitation: game box scores are available, but season-wide fantasy rankings are **not** implemented in this clean rebuild.
- API proxy with validation, timeout, caching and stale-data fallback.
- No fabricated scores or player stats.

## Data source
Uses ESPN's unofficial public site API, which can change, rate-limit, or be unavailable. Historical coverage depends on provider availability. No guarantee of live uptime or complete archives. No official league affiliation.

## Run
`npm start` then visit http://localhost:3000. `npm test` for API tests.
