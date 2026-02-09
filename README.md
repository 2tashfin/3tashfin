# 3tashfin — PDF Reader PWA

A clean, fast PDF reader you can install on your iPhone as an app.

## What's in here

```
3tashfin/
├── index.html       ← Main app
├── manifest.json    ← PWA config (app name, icon, etc.)
├── sw.js            ← Service worker (offline support)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## How to get it on your phone

### Option A: GitHub Pages (free, easiest)

1. Create a GitHub account if you don't have one → github.com
2. Create a new repository (name it whatever, like `3tashfin`)
3. Upload all the files from the `3tashfin/` folder to the repo
4. Go to **Settings → Pages → Source** → select `main` branch → Save
5. Wait ~1 minute, then visit `https://yourusername.github.io/3tashfin/`
6. On your iPhone, open that URL in **Safari**
7. Tap the **Share button** (square with arrow) → **Add to Home Screen**
8. Done! It'll appear as an app icon on your home screen

### Option B: Netlify (also free, drag & drop)

1. Go to app.netlify.com and sign up
2. Drag the entire `3tashfin/` folder onto the deploy area
3. You'll get a URL like `https://random-name.netlify.app`
4. Open that URL on your iPhone in Safari → Add to Home Screen

### Option C: Run locally (for testing)

If you have Python installed on your computer:

```bash
cd 3tashfin
python3 -m http.server 8080
```

Then on your phone (same Wi-Fi), open `http://YOUR_COMPUTER_IP:8080`

## Features

- **Open & render real PDFs** using PDF.js
- **Pinch-to-zoom** + zoom controls
- **Files persist** between sessions (stored in IndexedDB)
- **Search** your document library
- **Sort** by newest, oldest, or name
- **Offline support** via service worker
- **Installable** as a home screen app (PWA)
- **Dark theme** optimized for OLED screens

## Customization

- Edit colors in the `:root` CSS variables in `index.html`
- Change the app name in `manifest.json`
- Replace icons in `icons/` folder
