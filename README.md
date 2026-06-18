# 3-Point Contest Scorekeeper

A lightweight, browser-based scoring app for running basketball 3-point shooting contests. No installation, no internet required, no backend — just open the file and start scoring.

---

## Features

- **Half-court diagram** — the 5 racks are laid out on a visual half-court (corners, wings, top of key) so judges can score by position at a glance
- **Live scoring** across 5 racks with individual ball tracking (5 balls per rack, 1 point each)
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

## Sharing This App

**To share the code** (so someone can view, copy, or edit it): send the repo link —
`https://github.com/Jaidon2082/3point-contest`

**To share a live, working webpage** (so someone can just open a link and use it, no download needed): enable GitHub Pages once, then share that URL.

1. On GitHub, go to the repo's **Settings → Pages**
2. Under **Build and deployment → Source**, choose **Deploy from a branch**
3. Set branch to `main`, folder to `/ (root)`, click **Save**
4. After a minute, the live page is at:
   `https://jaidon2082.github.io/3point-contest/`
5. Text or email that link — it works on any phone, tablet, or laptop browser

> **Important:** everyone who opens that link gets their own independent copy of the app in their own browser (see [Data & Storage](#data--storage) below). It's great for letting someone preview or use the scorekeeper on their own device, but it is **not** a shared live scoreboard — two people scoring at the same time won't see each other's entries. For one event, pick one device as "the" scorekeeper.

---

### Scoring a Contestant

1. Go to the **Score Entry** tab
2. Type the contestant's name and click **Start Scoring**
3. A half-court diagram appears with 5 racks positioned where they're actually shot from — each rack has 5 balls worth 1 point each
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

Each rack: 5 balls (1 pt each) = **5 pts max per rack**
Total possible score: **25 points**

---

### Exporting Results

Go to the **Export** tab and choose:

- **Generate Report** — produces a formatted text summary with full rack-by-rack breakdowns
- **Download .txt** — saves the report as a plain text file
- **Download .csv** — saves results in spreadsheet format (Rank, Name, Total, Rack 1–5)
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
| Any ball (made) | 1 pt |
| Any ball (missed) | 0 pts |
| **Max per rack** | **5 pts** |
| **Max total (5 racks)** | **25 pts** |

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
