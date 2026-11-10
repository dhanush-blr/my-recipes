# 🍳 My Recipe Organizer

A modern, responsive, zero-dependency recipe manager web app built with vanilla JavaScript, HTML5, and Tailwind CSS.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Visit_App-amber?style=for-the-badge)](https://dhanush-blr.github.io/my-recipes/)
[![GitHub](https://img.shields.io/badge/GitHub-dhanush--blr%2Fmy--recipes-181717?style=for-the-badge&logo=github)](https://github.com/dhanush-blr/my-recipes)

**🔗 Live app:** https://dhanush-blr.github.io/my-recipes/

## 📸 Screenshots

| Light Mode | Dark Mode |
| :---: | :---: |
| ![My Recipe Organizer in light mode](screenshots/app-light.png) | ![My Recipe Organizer in dark mode](screenshots/app-dark.png) |

## ✨ Features

- **📱 Fully Responsive**: Fluid, mobile-first layout that adapts seamlessly to phones, tablets, and wide monitors.
- **⚖️ Dynamic Servings Scaler**: Interactive portion stepper (`[ − | 1 | + ]`) with automatic regular expression scaling of ingredient quantities.
- **⏳ Kitchen Countdown Timer**: Built-in per-recipe timer with start/pause/reset controls, visual notifications, and a synthesized audio chime via the Web Audio API.
- **🔍 Instant Search & Filter**: Real-time keystroke filtering by recipe name, individual ingredients, and category pills.
- **⭐ Favorites & Bookmarks**: Star go-to meals and filter by your favorites list with one click.
- **💾 Offline Persistence**: All custom recipes and preferences are safely stored locally in your browser via `localStorage`.
- **🖨️ Kitchen-Ready Print Styles**: Dedicated `@media print` rules hide web chrome and format cards cleanly for kitchen use.
- **📥 Backup & Export**: Download and backup your complete recipe library as a portable JSON file.
- **📤 Import & Restore**: Restore recipes from a previously exported JSON backup in one click — safely merged into your existing collection without duplicates or data loss.
- **🌙 Glare-Free Dark Mode**: Clean icon toggle with automatic preference memory for cooking in dim evening light.

---

## 🔄 Backup & Restore

### Export

Click **📥 Export Backup** in the toolbar to download your entire recipe library as a JSON file. The filename includes the export date, e.g. `my_recipes_backup_2026-11-10.json`.

### Import

Click **📤 Import Backup** and choose a JSON file exported from this app. The importer:

- **Validates the file** before touching your data — invalid JSON or files that aren't a recipe backup are rejected with a friendly message.
- **Normalizes each recipe**, filling in sensible defaults for any missing category, time, icon, servings, or favorite fields.
- **Preserves your existing recipes** — imports are additive, so nothing is overwritten or deleted.
- **Avoids ID collisions** by assigning fresh IDs to imported recipes that clash with existing ones.
- **Shows a confirmation toast** with the number of recipes imported.

Imported backups follow the same shape as the export:

```json
[
  {
    "id": 1,
    "title": "Creamy Garlic Pasta",
    "category": "Dinner",
    "time": "20 mins",
    "icon": "🍝",
    "baseServings": 2,
    "currentServings": 2,
    "favorite": true,
    "ingredients": ["200g pasta", "3 cloves garlic", "1 cup cream"],
    "steps": ["Boil the pasta.", "Sauté the garlic.", "Combine and serve."]
  }
]
```

---

## 🚀 Getting Started

### Live Demo

No installation needed — use the hosted app here:

**https://dhanush-blr.github.io/my-recipes/**

### Run Locally

This app runs completely client-side in any modern web browser. No `npm`, Node.js, Python, or local servers required!

Simply open `index.html` in your web browser:

```bash
# Clone the repository
git clone https://github.com/dhanush-blr/my-recipes.git

# Navigate to the folder
cd my-recipes

# Open in browser (macOS)
open index.html

# Open in browser (Windows)
start index.html
```

## 🛠️ Tech Stack

- **HTML5** — semantic, accessible markup
- **Tailwind CSS** (CDN) — responsive styling with class-based dark mode
- **Vanilla JavaScript** — no frameworks, no build step
- **Web Audio API** — synthesized timer chime
- **localStorage** — client-side persistence for recipes and theme

## 🌐 Hosting

The app is deployed with **GitHub Pages** from the `main` branch:

- Live URL: https://dhanush-blr.github.io/my-recipes/
- Repository: https://github.com/dhanush-blr/my-recipes

## 📄 License

This project is open source and available for personal use.
