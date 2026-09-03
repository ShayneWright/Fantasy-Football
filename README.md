# Don Pablo’s Fantasy Football Dashboard

A serverless Week 1 lineup decision dashboard built with plain HTML, CSS, and JavaScript.

## Open

Open `index.html` directly in a modern browser. No build step or server is required.

## Weekly update workflow

1. Copy `data/week-1.js` to a new weekly file.
2. Preserve the player field names; use `null` for anything not reliably published.
3. Update `index.html` to load the new data file and update `data/league-settings.js`.
4. Store previous and current Vegas lines independently; implied totals are calculated in `app.js`.

Lineup changes are stored in browser LocalStorage. Use **Reset recommended** to return to the report’s provisional lineup.

## Data policy

The supplied report is the only source for player evidence. Missing forecasts, usage, props, weather, practice and inactive data remain visibly pending rather than being converted to zero. Recommendations and confidence labels are explicitly presented as analyst assessments.
