# 🏀 3-Point Contest Scorekeeper

A lightweight, browser-based scoring app for running basketball 3-point shooting contests. No installation, no internet required, no backend — just open the file and start scoring.

---

## Features

- **Live scoring** across 5 racks with individual ball tracking (4 regular balls + 1 money ball per rack)
- **Real-time score display** updates as you tap each ball made or missed
- **Auto-save** — scores are written to local storage instantly so nothing is lost if the browser closes, the tab refreshes, or the device restarts
- **Session restore** — reopening the app on the same device automatically reloads all previous scores with a confirmation banner
- **Automatic standings** — contestants are ranked by total score at all times
- **Winner display** — dedicated standings view crowns the leader with a full leaderboard breakdown
- **Export results** as a formatted `.txt` report or `.csv` file for printing or record keeping
- **Mobile and tablet friendly** — works great on iPad or Android tablet for sideline use
- **Zero dependencies** — single HTML file, no frameworks, no installs, no Wi-Fi needed after opening

---

## How to Use

### Running the App

**Option A — Open locally**
1. Download `index.html`
2. Open it in any modern browser (Chrome, Safari, Firefox, Edge)
3. That's it — no server needed

**Option B — Host on GitHub Pages**
1. Fork or upload this repo to your GitHub account
2. Go to **Settings → Pages**
3. Set the branch to `main` and folder to `/ (root)`
4. Your app will be live at `https://yourusername.github.io/your-repo-name`

**Option C — Netlify Drop**
1. Go to [netlify.com/drop](https://netlify.com/drop)
2. Drag and drop `index.html` onto the page
3. A live URL is generated instantly — no account needed

---

### Scoring a Contestant

1. Go to the **Score Entry** tab
2. Type the contestant's name and click **Start Scoring**
3. Five racks appear — each has 4 regular balls (1 pt each) and 1 money ball (2 pts, labeled **MB**)
4. Tap each ball to toggle it between made (green) and missed (gray)
5. The live score updates with every tap
6. Click **Save Score** when done — the contestant is added to the leaderboard

---

### Rack Layout

| Rack | Position |
|------|----------|
| Rack 1 | Corner Left |
| Rack 2 | Wing Left |
| Rack 3 | Top of Key |
| Rack 4 | Wing Right |
| Rack 5 | Corner Right |

Each rack: 4 regular balls (1 pt) + 1 money ball (2 pts) = **6 pts max per rack**
Total possible score: **30 points**

---

### Exporting Results

Go to the **Export** tab and choose:

- **Generate Report** — produces a formatted text summary with full rack-by-rack breakdowns
- **Download .txt** — saves the report as a plain text file
- **Download .csv** — saves results in spreadsheet format (Name, Total, Made, Money Balls, Rack 1–5)
- **Copy** — copies the report to your clipboard

---

## Data & Storage

Scores are saved automatically to the browser's **local storage** every time a contestant is added or removed. This means:

- Data persists through browser closes, tab refreshes, and device restarts
- A green **✓ Saved** indicator flashes in the header after every save
- On reopen, a banner confirms data was restored
- The **Clear & Start Fresh** button on that banner wipes all scores for a new contest

> **Note:** Local storage is tied to the browser and device. Scores saved on an iPad in Safari will not appear on a laptop in Chrome. For multi-device use, designate one device as the scorer for the whole event, and export results at the end.

---

## Tips for Event Use

- On iPad, open the app in Safari and tap **Share → Add to Home Screen** for a fullscreen app-like experience with no browser chrome
- Keep the browser tab open throughout the event — local storage is a backup, not a replacement for leaving it open
- Export to `.csv` at the end for a permanent record before clearing data for the next event
- If you need to re-score a contestant, remove them with the ✕ button and re-enter them

---

## Modifying the App

The entire app is a single HTML file with vanilla HTML, CSS, and JavaScript — no build tools or dependencies required. Open it in any code editor to make changes.

Recommended setup for live editing:

1. Install [VS Code](https://code.visualstudio.com)
2. Install the **Live Server** extension by Ritwick Dey
3. Open `index.html` and click **Open with Live Server**
4. The browser auto-refreshes on every save (`Ctrl+S`)

---

## Scoring Reference

| Ball Type | Points |
|-----------|--------|
| Regular ball (made) | 1 pt |
| Money ball — MB (made) | 2 pts |
| Any ball (missed) | 0 pts |
| **Max per rack** | **6 pts** |
| **Max total (5 racks)** | **30 pts** |

---

## Browser Compatibility

Works in all modern browsers. Tested in:
- Chrome 120+
- Safari 16+
- Firefox 120+
- Edge 120+

---

## License

MIT — free to use, modify, and distribute.
