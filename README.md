# 💸 Neo Spend — Personal Finance Tracker PWA

A fully interactive personal finance tracker built as a **Progressive Web App (PWA)** — installable on iOS and Android, works offline, no backend required.

---

## ✨ Features

| Feature | Details |
|---|---|
| 📊 Dashboard | Summary cards with animated counters, donut chart, trend chart, caution zones, budget vs actual bar |
| 💳 Transactions | 30 realistic Indian transactions, live search + category filter, High Spend badges |
| 💰 Budget | Per-category editable budgets, live recalculation, stacked progress bar |
| ➕ Add Transaction | FAB button opens a bottom sheet form — adds to transaction list instantly |
| 📱 PWA | Installs on iOS (Safari) and Android (Chrome) — works offline |
| 🌙 Dark Mode | Full dark theme, `#0a0d14` base — designed for AMOLED screens |
| 🇮🇳 INR Formatting | All currency in ₹ with Indian lakh/crore formatting |

---

## 🚀 Deploy to Netlify (Recommended)

### Option A — Drag & Drop (Fastest)
1. Go to [netlify.com](https://netlify.com) → Log in → **Sites**
2. Drag the entire `neo-spend/` folder onto the Netlify dashboard
3. Done — you'll get a live URL like `https://neo-spend-xxxx.netlify.app`

### Option B — GitHub + Netlify CI/CD
1. **Push to GitHub:**
   ```bash
   cd neo-spend
   git init
   git add .
   git commit -m "feat: Neo Spend PWA"
   git remote add origin https://github.com/YOUR_USERNAME/neo-spend.git
   git push -u origin main
   ```
2. Go to [app.netlify.com](https://app.netlify.com) → **Add new site** → **Import from Git**
3. Select your repo → Build settings are auto-detected via `netlify.toml`
4. Click **Deploy site**

---

## 📱 Install on iOS

1. Open the Netlify URL in **Safari** on iPhone/iPad
2. Tap the **Share button** (box with arrow pointing up)
3. Scroll down and tap **"Add to Home Screen"**
4. Tap **Add** — Neo Spend appears on your home screen like a native app

> Note: iOS PWAs require Safari. Chrome on iOS does not support "Add to Home Screen" for PWAs.

---

## 📱 Install on Android

1. Open the Netlify URL in **Chrome** on Android
2. Chrome will show an **"Add Neo Spend to Home screen"** banner automatically
3. Tap **Install** — the app installs like a native APK
4. Alternatively: tap the 3-dot menu → **"Add to Home screen"**

---

## 🗂 Project Structure

```
neo-spend/
├── index.html       ← Complete single-page app (HTML + CSS + JS)
├── manifest.json    ← PWA manifest (icons, name, theme)
├── sw.js            ← Service worker (offline caching)
├── netlify.toml     ← Netlify headers & redirect config
└── README.md        ← This file
```

---

## 🛠 Local Development

```bash
# Install a simple local server (one-time)
npm install -g serve

# Run locally
cd neo-spend
serve .
# Open http://localhost:3000
```

Or use VS Code Live Server extension — right-click `index.html` → **Open with Live Server**.

---

## 📦 Tech Stack

- **Vanilla HTML / CSS / JavaScript** — zero frameworks
- **Chart.js** (CDN) — donut, area, bar charts
- **Google Fonts** — Space Grotesk + Space Mono
- **Material Symbols** — icons
- **PWA APIs** — Service Worker, Web App Manifest, `beforeinstallprompt`

---

## 🧑‍💻 Built by

Ashwanth Raja S P — VIT Vellore, CSBS 2029  
[github.com/ashwanthraja07](https://github.com/ashwanthraja07)
