# CAM’S STATS — ESPN-backed release

Single Node.js backend, no API key, no Python or Vite. Live and historical ESPN scoreboards, team logos, game box scores, NBA daily fantasy and NFL daily fantasy. No fake scores.

## Render
Runtime: Node; build: `npm install && npm run build`; start: `npm start`. Replace all files in the repository root with the **contents** of this folder.

## API
`/api/health`, `/api/nfl/scoreboard?date=2026-10-22`, `/api/nba/scoreboard?date=2026-10-22`, `/api/nfl/game?id=EVENT_ID`, `/api/nba/game?id=EVENT_ID`, `/api/nfl/teams`, `/api/nba/teams`, `/api/fantasy?league=nfl&date=2026-10-22&scoring=ppr`.

ESPN is an unofficial source, and may throttle or alter endpoints. Daily fantasy includes only completed games and may omit statistics unavailable in provider box scores. Historical season aggregates and live projections are not included.
