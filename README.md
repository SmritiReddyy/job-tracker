# eat-pray-apply

> Touch grass occasionally. Apply relentlessly. Somewhere between refreshing your inbox and questioning your life choices, this app keeps count so you don't have to.
 
> Track your job applications the way GitHub tracks your commits.

**Live demo:** [smritireddyy.github.io/job-tracker](https://smritireddyy.github.io/job-tracker/)

---

## Why

Most job seekers lose track of their momentum. A spreadsheet is tedious. ATS tools are overkill. job-tracker gives you one thing: a visual record of how consistently you're showing up — the same satisfaction loop as a GitHub contribution graph, applied to your job search.

No account. No backend. No ads. Just open the URL and log your applications.

---

## Features

**Contribution heatmap** — a day-by-day grid from March 2026 onward, color-coded by volume. The grid automatically adds a new month on the first of each month — no code changes needed. One glance tells you where you went dark and where you were on a roll.

**Three independent goal trackers** — set separate daily, weekly, and monthly targets. Each has its own progress bar and live count so you always know how far you are from each goal.

**Streak counter** — tracks your current active streak and your longest streak to date. Missing a day hurts more when the number is staring back at you.

**Monthly totals chart** — a bar chart showing total applications per month, so you can see the big-picture arc of your search over time.

**Weekly totals chart** — last 12 weeks of activity at a glance, useful for spotting effort patterns week over week.

**Next month preview** — the upcoming month is always visible (view-only) so you can plan ahead without being able to accidentally log future dates.

**CSV export** — download all your application data as a CSV with one click. Good for backups, or dropping into a spreadsheet for deeper analysis.

**Zero infrastructure** — a single HTML file. No Node, no build step, no server. Data lives in your browser's localStorage and persists between sessions.

---

## How to Use

**Logging applications**

| Action | How |
|---|---|
| Log for today | Set the count in the number field, click **+ add** |
| Log for a past day | Click any cell in the grid to select that date, set count, click **+ add** |
| Correct a day's count | Select the date, enter the correct total, click **set exact** |
| Keyboard shortcut | Type count in the number field, press **Enter** |
| Export your data | Click **export csv** to download all entries as a CSV file |

**Setting goals**

Type a number next to daily, weekly, or monthly and click **set**. Each goal is saved independently and persists across sessions. Defaults are 10 / 30 / 100 — adjust to your pace.

**Reading the grid**

Cells get darker as the count goes up. Hover any cell to see the exact count for that day. Today is outlined in green. Future dates are dimmed and non-interactive.

---

## Deploy to GitHub Pages

1. Create a new **public** repo at [github.com/new](https://github.com/new)
2. Upload `index.html` via **Add file → Upload files**
3. Go to **Settings → Pages → Source: Deploy from branch → main / root → Save**
4. Visit `https://<your-username>.github.io/job-tracker/` in ~60 seconds

No build step needed. The file is self-contained.

---

## Tech Stack

- **HTML / CSS / Vanilla JS** — no frameworks, no dependencies to install
- **Chart.js** — weekly and monthly bar charts (loaded via CDN)
- **Google Fonts** — DM Mono + DM Sans (loaded via CDN)
- **localStorage** — all data stored client-side, zero backend
- **GitHub Pages** — free static hosting

---

## A note on data

Your data lives in your browser's localStorage. It is never sent anywhere. If you clear your browser data or switch devices, it will be gone — use the **export csv** button periodically to back up your entries. The CSV downloads as `job-applications.csv` with one row per active day.
