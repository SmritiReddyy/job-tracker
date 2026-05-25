# job-tracker

Personal job application tracker — GitHub contributions graph style.

## Features
- Heatmap grid (March 2026 onward, auto-expands each month) with color intensity by daily count
- Current + longest streak counter
- Weekly bar chart (last 12 weeks)
- Click any day cell to select it, then log or set the count
- Data stored in `localStorage` — persists across browser sessions

## Deploy to GitHub Pages (5 steps)

1. **Create a new GitHub repo**
   - Go to https://github.com/new
   - Name it `job-tracker` (or anything you want)
   - Set to **Public** (required for free GitHub Pages)
   - Don't initialize with README

2. **Push this file**
   ```bash
   cd /path/to/this/folder
   git init
   git add index.html README.md
   git commit -m "init job tracker"
   git branch -M main
   git remote add origin https://github.com/SmritiReddyy/job-tracker.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repo → Settings → Pages
   - Source: **Deploy from a branch**
   - Branch: `main` / `/ (root)`
   - Click Save

4. **Wait ~60 seconds**, then visit:
   ```
   https://SmritiReddyy.github.io/job-tracker/
   ```

5. **Bookmark it** — your data lives in your browser's localStorage so it persists between visits.

## Usage

| Action | How |
|---|---|
| Log apps for today | Set count → click **+ add** |
| Log for another day | Click a cell to select it, set count → **+ add** |
| Correct a day | Select date, enter correct total → **set exact** |
| Keyboard shortcut | Type count in the number field → press Enter |

## Extending

New months appear automatically — the grid always shows March 2026 through the current month.