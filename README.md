# Kharchila 💸

> **Apna Kharcha. Apni Marzi.**
> *(Roughly: "Your spending. Your rules." — "Kharchila" is Hindi/Urdu slang for a big spender, which is a fittingly ironic name for an expense tracker.)*

A personal expense tracker + friend bill splitter, built as a single self-contained `index.html` file. No backend, no database, no sign-up, no tracking — every rupee you log stays on your own device.

![Made with HTML CSS JS](https://img.shields.io/badge/stack-HTML%20%2B%20CSS%20%2B%20JS-7C3AED) ![No backend](https://img.shields.io/badge/backend-none-9333EA) ![License: MIT](https://img.shields.io/badge/license-MIT-blue)

## ✨ Features

### 🏠 Dashboard
- Big ₹ total-spent hero number
- Day / Week / Month / Year filter pills
- Donut chart of spend-by-category (Chart.js)
- Top 3 categories with animated progress bars
- Last 5 transactions at a glance

### ➕ Add Expense
- Large numpad-style ₹ amount entry — no fiddly native number keyboard
- 8 emoji categories: Food, Transport, Shopping, Health, Entertainment, Bills, Education, Other
- Optional note + date (defaults to today)
- Instant save with a little success animation

### 🤝 Split — Udhari Tracker
- Add friends by name
- Log a shared expense: amount, description, and who actually paid
- Auto-splits equally between you and everyone selected
- Running balance per friend ("Rahul owes you ₹300")
- One-tap **Settle up**, with a full history of every split and settlement

### 🕓 History
- Full transaction list, newest first
- Filter by category, this week, or this month
- Search by note keyword
- Delete entries (with confirmation)
- Export **everything** — expenses, friend balances, and split history — as one CSV file

## 🔒 Privacy, by construction

Kharchila has no server to talk to. Every byte of data is read from and written to your browser's `localStorage`, on your device, full stop. There's no login because there's no account to log into. The only way data leaves the app is if *you* tap "Export as CSV."

## 🛠 Tech stack

- Vanilla HTML, CSS, and JavaScript — no frameworks, no bundler, no build step
- [Chart.js](https://www.chartjs.org/) (via CDN) for the donut chart
- [Google Fonts](https://fonts.google.com/) — Sora for numbers/headings, Inter for body text
- Browser `localStorage` for all persistence

## 🚀 Getting started

### Run it locally
No installation needed — just open the file.

```bash
git clone https://github.com/<your-username>/kharchila.git
cd kharchila
open index.html   # macOS — or just double-click it on any OS
```

### Deploy to GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Pick the `main` branch and `/ (root)` folder, then **Save**.
5. Your app goes live at `https://<your-username>.github.io/kharchila/` within a minute or two.

That's it — no CI, no build pipeline, nothing to break.

## 📁 Project structure

```
kharchila/
├── index.html    # everything: markup, styles, and app logic
├── README.md
├── LICENSE
└── .gitignore
```

## ⚠️ Disclaimer

Kharchila is in early development — like a baby just learning to walk. It tries its best but may make mistakes. It is **not** a financial tool. All data lives only on your device, and the author is not liable for any data loss or financial decisions made using this app.

## 📄 License

Released under the [MIT License](LICENSE) — do whatever you like with it.

---

Made with 🍵 and one too many group dinners that needed splitting three ways.
