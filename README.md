# Faithful — 90-Day Stewardship Journey

A self-contained web app version of your 90-day devotional. No build step, no dependencies to install — it's a single `index.html` that runs anywhere.

## What's in this folder
- `index.html` — the entire app (all 90 days of content + UI are embedded in this one file)
- `manifest.json` — makes "Add to Home Screen" behave like a real app icon
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` — home screen icons

## Deploy to GitHub Pages (~10 minutes)

1. **Create a repo.** Go to github.com → New repository → name it something like `faithful90` → Public → Create.
2. **Upload these files.** On the repo page, click "Add file" → "Upload files," drag in all 5 files from this folder, commit.
3. **Turn on Pages.** Go to Settings → Pages (left sidebar). Under "Build and deployment," set Source to **Deploy from a branch**, Branch to **main** / folder **/ (root)**. Save.
4. **Wait ~1 minute**, then refresh that Pages settings tab. You'll see a live URL like:
   `https://yourusername.github.io/faithful90/`
5. **Open that link on your phone.**
   - iPhone: Safari → Share icon → "Add to Home Screen"
   - Android: Chrome → ⋮ menu → "Add to Home Screen" / "Install app"

You now have a real icon on your home screen that opens full-screen with no browser bar.

## Data & privacy
Your daily answers and scorecard save to your phone's local browser storage (`localStorage`) — nothing leaves your device, nothing goes to a server. This also means:
- Progress is per-device. Doing Day 12 on your phone won't show up on your laptop unless you're using the same browser/profile.
- Clearing your browser's site data (or uninstalling/reinstalling as a home-screen app in some cases) will erase progress. Not a big risk day-to-day, but worth knowing.

## Making future edits
Since it's plain HTML/React (loaded via CDN, no build tools), you can hand-edit `index.html` directly, or paste it back into a Claude chat and ask for changes — either works.
