# 🍳 My Recipe Organizer

A modern, responsive, zero-dependency recipe manager web app built with vanilla JavaScript, HTML5, and Tailwind CSS.

## ✨ Features

- **📱 Fully Responsive**: Fluid, mobile-first layout that adapts seamlessly to phones, tablets, and wide monitors.
- **⚖️ Dynamic Servings Scaler**: Interactive portion stepper (`[ − | 1 | + ]`) with automatic regular expression scaling of ingredient quantities.
- **⏳ Kitchen Countdown Timer**: Built-in per-recipe timer with start/pause/reset controls, visual notifications, and a synthesized audio chime via the Web Audio API.
- **🔍 Instant Search & Filter**: Real-time keystroke filtering by recipe name, individual ingredients, and category pills.
- **⭐ Favorites & Bookmarks**: Star go-to meals and filter by your favorites list with one click.
- **💾 Offline Persistence**: All custom recipes and preferences are safely stored locally in your browser via `localStorage`.
- **🖨️ Kitchen-Ready Print Styles**: Dedicated `@media print` rules hide web chrome and format cards cleanly for kitchen use.
- **📥 Backup & Export**: Download and backup your complete recipe library as a portable JSON file.
- **🌙 Glare-Free Dark Mode**: Clean icon toggle with automatic preference memory for cooking in dim evening light.

---

## 🚀 Getting Started

This app runs completely client-side in any modern web browser. No `npm`, Node.js, Python, or local servers required!

### Run Locally
Simply open `index.html` in your web browser:
```bash
# Clone the repository
git clone [https://github.com/dhanush-blr/my-recipes.git](https://github.com/dhanush-blr/my-recipes.git)

# Navigate to the folder
cd my-recipes

# Open in browser (macOS)
open index.html

# Open in browser (Windows)
start index.html