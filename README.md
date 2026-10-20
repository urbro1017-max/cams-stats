# CAM'S STATS V2.0

React/Vite NFL + NBA sports desk, with ESPN-style editorial layout, NFL/NBA scores and news fetched client-side from ESPN's publicly accessible endpoints, and an illustrative CAM Fantasy Index.

## Deployment on existing Render Web Service
Build command: `yarn install && yarn build`
Start command: `npx vite preview --host 0.0.0.0 --port $PORT`
The `vite.config.js` file permits `cams-stats.onrender.com` as a preview host.

## Recommended production deployment
Render Static Site: build `npm install && npm run build`, publish directory `dist`, root directory blank. Static sites do not need a start command.

## Data disclaimer
Game scores and headlines are requested from ESPN public endpoints in the visitor's browser and refreshed every 60 seconds; endpoint accessibility and browser CORS policies are outside this project's control. A clear unavailable state appears if the feed cannot be reached. Fantasy rankings, stat leaders, projections and comparisons are demo data, NOT actual or current recommendations. For reliable production live data and fantasy projections, use a licensed provider and backend ingestion.

## Local development
`npm install`
`npm run dev`

## Version 2 changes
- NFL and NBA current scoreboard feeds with loading/failure states
- NFL and NBA latest news with external story links
- 60-second scoreboard refresh
- No fictional scores displayed as current data
- New editorial story cards and league headlines
- Render Vite preview allowlist config included
