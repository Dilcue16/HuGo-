# HuGo PWA — Installation & Deployment Guide
## Human Rights on the Go
### Bulacan Police Provincial Human Rights Affairs Office · BULPPO, PRO 3

---

## FILES IN THIS PACKAGE

```
hugo-pwa/
├── index.html          ← Main app (entire HuGo system)
├── manifest.json       ← PWA manifest (app name, icons, shortcuts)
├── sw.js               ← Service worker (offline, caching, sync)
├── offline.html        ← Offline fallback page
├── icons/
│   ├── icon-72.png
│   ├── icon-96.png
│   ├── icon-128.png
│   ├── icon-144.png
│   ├── icon-152.png
│   ├── icon-192.png    ← Main app icon
│   ├── icon-384.png
│   └── icon-512.png    ← Splash/install icon
└── README.md           ← This file
```

---

## OPTION 1 — HOST ON GITHUB PAGES (FREE, FASTEST)

1. Create a free account at https://github.com
2. Create a new repository named: `hugo-pwa`
3. Upload ALL files from this folder (keep folder structure)
4. Go to Settings → Pages → Source: main branch → /root
5. Your app will be live at:
   `https://YOUR-USERNAME.github.io/hugo-pwa/`
6. Share this URL with all station users

---

## OPTION 2 — HOST ON NETLIFY (FREE, DRAG & DROP)

1. Go to https://netlify.com and create a free account
2. Drag the entire `hugo-pwa` folder into Netlify
3. Your app gets a URL like: `https://hugo-xxxxx.netlify.app`
4. Optional: Set custom domain in Netlify settings

---

## OPTION 3 — LOCAL TESTING ON PC (NO HOSTING NEEDED)

Install a simple local server:

```bash
# If you have Python installed:
cd hugo-pwa
python3 -m http.server 8080

# Then open in Chrome:
http://localhost:8080
```

Or install VS Code + Live Server extension and open index.html.

---

## HOW TO INSTALL ON ANDROID PHONE

1. Host the app using Option 1 or 2 above
2. Open Chrome on your Android phone
3. Go to the URL (e.g. https://your-username.github.io/hugo-pwa/)
4. Wait for the page to fully load
5. Tap the 3-dot menu (⋮) in Chrome
6. Tap "Add to Home screen"
7. Tap "Add"
8. HuGo icon will appear on your home screen
9. Tap it — it launches fullscreen like a native app!

---

## HOW TO INSTALL ON iPHONE / iOS

1. Open Safari (must use Safari, not Chrome)
2. Go to the URL
3. Tap the Share button (box with arrow)
4. Scroll down and tap "Add to Home Screen"
5. Tap "Add"

Note: Camera works on iOS Safari. Some PWA features may be limited.

---

## VALID INSPECTION TOKENS (for camera module)

```
HUGO-INSPECT-01
PHRA-CAM-2025
BULPPO-SU-99
```

These tokens are hardcoded for testing. In production, generate tokens dynamically.

---

## MODULES INCLUDED

| Module | Access |
|--------|--------|
| Weekly PICE | Station user |
| Monthly Medical Check-up | Station user |
| Monthly PHROs & COs | Station user |
| Monthly IDD | Station user |
| AI Camera Inspection | Token required |
| Master Consolidated Report | Super user only |

---

## REQUIREMENTS

- Chrome 80+ on Android (recommended)
- Safari 14+ on iOS
- Internet connection for AI features
- Camera permission for inspection module

---

## SUPPORT

HuGo v4 — Human Rights on the Go
Bulacan Police Provincial Human Rights Affairs Office
BULPPO, PRO 3, PNP
