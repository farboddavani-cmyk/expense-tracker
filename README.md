# 💰 Expense Tracker PWA

A lightweight Progressive Web App for tracking business expenses on your phone. Snap receipts, log descriptions, and export to Excel when it's time to file your taxes — no subscription, no login required.

---

## Features

- 📷 **Receipt photos** — take a photo or upload an image/PDF directly from your phone
- 🗂️ **Smart categorization** — Office Supplies, Travel, Meals, Software, and more
- 💵 **Tax tracking** — mark each expense as fully deductible, 50%, partial, or non-deductible
- 📊 **Live dashboard** — see your total spend and breakdown by category at a glance
- 📤 **One-tap export** — download as CSV or copy to paste directly into Excel
- 💾 **Works offline** — all data saved locally on your device, no internet needed after install
- 📱 **Installs like an app** — add to your Android or iOS home screen from Chrome/Safari

---

## How to install on your phone

### Android (Chrome)
1. Open your GitHub Pages URL in **Chrome**
2. Tap the **three-dot menu** (top right)
3. Tap **"Add to Home Screen"**
4. Tap **Add** — the app icon appears on your home screen

### iPhone (Safari)
1. Open your GitHub Pages URL in **Safari**
2. Tap the **Share button** (box with arrow at the bottom)
3. Tap **"Add to Home Screen"**
4. Tap **Add**

---

## How to link to the Excel spreadsheet

This app works alongside the companion **expense_tracker.xlsx** file.

| In the app | What to do in Excel |
|---|---|
| Export → **Download CSV** | Open Excel → Expense Log sheet → click cell **A5** → Data → From Text/CSV → select the file |
| Export → **Copy for spreadsheet** | Open Excel → click cell **A5** → Paste (Ctrl+V / Cmd+V) |
| Export → **Download JSON backup** | Save somewhere safe — use "Restore from backup" to reload your data |

The Excel file has four sheets that update automatically:

- **Expense Log** — your main data entry sheet
- **Dashboard** — live totals and spend by category
- **Tax Summary** — expenses grouped by deductibility, ready for your accountant
- **Instructions** — quick reference guide

---

## How to host on GitHub Pages

1. Fork or upload this repository to your GitHub account
2. Go to **Settings → Pages**
3. Under Branch, select **main** → click **Save**
4. Wait 1–2 minutes — your app will be live at:

```
https://yourusername.github.io/expense-tracker
```

---

## File structure

```
expense-pwa/
├── index.html       ← The full app (single file)
├── manifest.json    ← PWA install configuration
├── sw.js            ← Service worker (offline support)
└── icons/
    ├── icon-192.png ← App icon (Android home screen)
    └── icon-512.png ← App icon (splash screen)
```

---

## Data & privacy

All expense data is stored **locally on your device** using the browser's local storage. Nothing is sent to any server. Your data stays on your phone unless you choose to export it.

To back up your data, use **Export → Download JSON backup**. To move to a new device, restore from that backup file.

---

## Tax time checklist

- [ ] All expenses logged with descriptions
- [ ] Receipts attached or marked as pending
- [ ] Tax deductible field filled in for each entry
- [ ] CSV exported and imported into Excel
- [ ] Tax Summary sheet reviewed and printed or shared with accountant

---

## Built with

- Vanilla HTML, CSS, and JavaScript — no frameworks
- Web App Manifest for installability
- Service Worker for offline support
- localStorage for on-device data persistence

---

## License

Free to use for personal and business use.
