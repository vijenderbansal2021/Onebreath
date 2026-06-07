# One Breath — PWA Deployment Guide

## What's in this folder

| File | Purpose |
|------|---------|
| `index.html` | The complete app (all screens + logic) |
| `manifest.json` | Makes it installable like a native app |
| `sw.js` | Service worker — enables full offline use |

You also need to add:
- `icon-192.png` — 192×192px app icon (dark background, simple mark)
- `icon-512.png` — 512×512px app icon (same design, larger)

---

## Deploy in 5 minutes (Free — Netlify)

1. Go to **netlify.com** → sign up free with GitHub or email
2. Drag and drop this entire `OneBreath-PWA` folder onto the Netlify dashboard
3. Netlify gives you a live URL instantly, e.g. `https://onebreath-abc123.netlify.app`
4. (Optional) Add a custom domain like `onebreath.app` — Netlify handles HTTPS free

That's it. Your app is live worldwide.

---

## Alternative: GitHub Pages (also free)

1. Create a free GitHub account at github.com
2. New repository → name it `onebreath` → set to Public
3. Upload all files in this folder
4. Go to Settings → Pages → Source: main branch / root
5. Your URL: `https://yourusername.github.io/onebreath`

---

## How users install it (no App Store needed)

### iPhone / Safari
1. Open the URL in Safari
2. Tap the Share button (box with arrow)
3. Tap "Add to Home Screen"
4. Tap "Add" — app icon appears on home screen
5. Opens fullscreen, works offline ✓

### Android / Chrome
1. Open the URL in Chrome
2. Chrome automatically shows "Add to Home Screen" banner
3. Tap Install
4. App icon appears, works offline ✓

### Windows / Mac (desktop)
1. Open in Chrome or Edge
2. Click the install icon in the address bar
3. Installed as a standalone desktop app

---

## App icon — create one free

Go to **canva.com** → create a 512×512 design:
- Dark background (#0d1117)
- Simple white/teal circle or leaf shape
- Export as PNG
- Resize to 192×192 for the second icon

Or use **realfavicongenerator.net** to generate all sizes at once.

---

## Privacy Policy (required for Google Play, optional for PWA)

One Breath collects zero user data. Here's a minimal privacy policy
you can paste into a free page on **notion.site** or **github pages**:

---
*One Breath does not collect, store, or transmit any personal data.
All session data (streaks, history) is stored locally on your device
and never leaves it. No accounts. No analytics. No tracking.*
---

---

## Going further — Google Play ($25 one-time fee)

Once your PWA is live, you can wrap it for the Play Store using
**PWABuilder** (pwabuilder.com):

1. Enter your live URL
2. Click "Package for Stores" → Android
3. PWABuilder generates an APK/AAB file
4. Upload to Google Play Console (one-time $25 registration)
5. Set price to Free → Submit

No native code. No Android Studio needed.
