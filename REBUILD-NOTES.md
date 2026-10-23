# CAM’S STATS — consolidated rebuild notes

This release is based on the latest CAM’S STATS source package. **ATLAS source code was not supplied**, so it is not a verified transplant of the ATLAS backend.

## Fixes
- Correct local ISO dates for NFL/NBA scoreboards and NBA fantasy. Previous en-CA locale formatting could generate invalid YYYYMMDD queries in some browsers.
- Route all /api requests (including NBA fantasy) to the Node backend during Vite development.
- Add a 25-second NBA fantasy request timeout, plus clearer scoreboard failure recovery.
- Add backend /api/status operational diagnostics, request counters and stale-on-upstream-error ESPN responses.
- Consolidate a high-contrast visual layer with responsive cards, keyboard focus, readable tables and restrained effects.
- Keep original NFL/NBA game review, fantasy collector, team logos and scoreboards.

## Deploy
Render: Node runtime; build `npm install && npm run build:with-data`; start `npm start`.
If the upstream ESPN build-time collector fails, diagnose that separately rather than silently publishing fabricated stats.

## Verification limitations
No live provider responses or production Render deployment verified in this environment. ATLAS backend cannot be copied without its source.
