# Deploying iPlan — free, ~5 minutes

You need a free GitHub account. That's the only account required — no paid tier, no credit card.

## Steps

1. Go to github.com, sign in (or create a free account).
2. Click **New repository**. Name it `iPlan` (or anything). Keep it Public. Don't add a README.
3. On the new repo page, click **uploading an existing file** (or use "Add file → Upload files").
4. Drag in all 5 files from this folder: `index.html`, `manifest.json`, `service-worker.js`, `icon-192.png`, `icon-512.png`.
5. Commit the upload.
6. Go to the repo's **Settings → Pages**.
7. Under "Build and deployment", set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
8. Wait about a minute. GitHub will show you a URL like `https://yourusername.github.io/iplan/`.

## On your phone

1. Open that URL in **Safari** (must be Safari on iOS for install to work).
2. Tap **Share → Add to Home Screen**.
3. It now installs as a real standalone app — own icon, opens full-screen, works offline, and its data lives in the phone's browser storage independent of Claude.ai.

## Updating it later

Whenever you want changes: come back here, I'll give you an updated `index.html`, and you re-upload just that one file to the same GitHub repo (drag and drop, commit). No redeploy step needed — GitHub Pages picks it up automatically within a minute or two.

## What this does NOT give you yet

- Real prayer-time calculation (still placeholder times — that's the next piece to add)
- Push notifications (iOS PWA push support is limited; would need testing)
- A true home-screen widget (hard iOS platform limit — this gets you the app icon and full-screen install, not a WidgetKit-style live widget)
