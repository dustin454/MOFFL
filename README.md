# MOFFL Website Prototype

A zero-build static website designed for free GitHub Pages hosting.

## Preview locally
You can now simply double-click `index.html`. Version 3 embeds the website data directly in the browser bundle, so History, Records, GM profiles, drafts, financials, and rules populate even when opened from a local folder. Running a local web server is still optional.

## Publish on GitHub Pages
1. Create a GitHub repository (for example `moffl`).
2. Upload everything in this folder to the repository root.
3. In repository Settings → Pages, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save. GitHub will provide the public site URL.

## Data
The `/data` folder is generated from `MOFFL_Normalized_Database_v3.xlsx`.
No database server is required; the site reads JSON in the browser.

## Included prototype pages
- Home / League HQ
- League History / Champions
- GM Hub
- Draft Archive
- Financials & ROI
- Constitution

## Next build targets
- Individual GM profile routes/pages
- Full season pages and standings
- Record Book
- Championship roster explorer
- Player Hall of Fame / championship leaderboard
- Rule proposal submission workflow
- Announcements/current-season dashboard

## Version 2 additions
- Dynamic individual GM franchise profiles (`gm.html?gm=GM006`)
- Career season timeline for every normalized GM
- Championship and runner-up history by GM
- Financial resume / ROI embedded into GM profiles
- Recent draft history per GM
- Automatically calculated MOFFL Record Book
- Hall of Fame / legacy leader pages for GMs and championship players

The Hall of Fame page is explicitly presented as a data-driven legacy gallery until the league creates an official induction process.


## Version 3 fix
- Embedded all JSON data directly into `assets/app.js`.
- Pages no longer depend on browser permission to fetch local JSON files.
- Still retains the `/data` JSON files for GitHub Pages and future development.


## Scope cleanup
Head-to-head and rivalry features were removed because only the 2023 weekly matchup dataset was available. The public site now focuses on league-wide historical data with meaningful multi-season coverage.
