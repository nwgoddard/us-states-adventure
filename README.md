# 🗺️ US States Adventure!

A fun, interactive HTML game for kids (and adults!) to learn all 50 US states and their capitals.

## How to Play

### Option 1 — Open directly (easiest)
1. Download **`index.html`**
2. Double-click it to open in any web browser
3. That's it — no installation needed!

> **Note:** An internet connection is required. The game loads its map data and charting libraries from the web the first time it opens.

### Option 2 — Clone the repo
```bash
git clone https://github.com/nwgoddard/us-states-adventure.git
cd us-states-adventure
open index.html
```

---

## Game Modes

| Mode | Description |
|------|-------------|
| 🔍 **Find the State** | A state name is shown — click the correct state on the map. Use the 💡 Hint button if you're stuck (small score penalty). |
| 🏛️ **Capital Quiz** | Pick the correct capital city from 4 multiple-choice options. |
| 🌍 **Explore & Learn** | Hover over any state to see a tooltip. Click to reveal a full fun fact and the capital. No pressure! |

---

## Features

- ✅ Accurate US map using real geographic boundary data (US Census / TopoJSON)
- ⭐ Gold star on every state marking the exact location of its capital city
- 🏆 Score, streak, and lives tracking
- 🎉 Confetti + sound effects for correct answers
- 📊 Progress bar showing how many states you've completed
- 🔥 Streak bonuses for consecutive correct answers
- 📖 Fun facts for all 50 states

---

## Tech Stack

- [D3.js v7](https://d3js.org/) — map projection and rendering
- [TopoJSON Client](https://github.com/topojson/topojson-client) — decoding geographic data
- [us-atlas](https://github.com/topojson/us-atlas) — US Census state boundary data
- Vanilla JS / HTML / CSS — no build tools, no frameworks

---

## Editing

Everything is in a single file: **`index.html`**

- **State facts & capitals** → `STATE_DATA` object near the top of the `<script>` tag
- **State colors** → `STATE_COLORS` object
- **Scoring rules** → `correct_answer()` and `wrong_answer()` functions
- **Styles** → the `<style>` block in `<head>`
