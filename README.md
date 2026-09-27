# Don Pablo’s Fantasy Football Dashboard

A serverless weekly lineup decision dashboard built with plain HTML, CSS, and JavaScript.

## Open

Open `index.html` directly in a modern browser. No build step or server is required.

## Weekly update workflow

1. Add the next `data/week-N.js` file without deleting earlier weeks.
2. Preserve the player field names; use `null` for anything not reliably published.
3. Load the new weekly data file in `index.html`; the week selector preserves access to earlier weeks.
4. Store previous and current Vegas lines independently; implied totals are calculated in `app.js`.

Use `?week=1` or `?week=2` in the URL to open a specific week. Lineup changes are stored separately for each week in browser LocalStorage. Use **Reset recommended** to return to the report’s provisional lineup.

## Data policy

The supplied report is the only source for player evidence. Missing forecasts, usage, props, weather, practice and inactive data remain visibly pending rather than being converted to zero. Recommendations and confidence labels are explicitly presented as analyst assessments.
