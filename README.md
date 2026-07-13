# Spin It — Decision Picker

A wheel that makes small decisions for you. Add options, spin, get an answer.
No accounts, no backend, no tracking — everything lives in your browser's local storage.

**Live:** `https://<your-username>.github.io/spin-it/`

## Features

- **Spinner wheel** — slice sizes reflect the real odds, and the wheel always lands where it says it will.
- **Saved lists** — keep separate wheels for dinner, movies, workouts, chores. Switch with the dropdown.
- **Weights** — bump an option's weight from 1 to 10 with `−` / `+`. Its slice grows and the `%` next to it shows the true chance. "Even odds" resets everything to 1.
- **Never repeat the last pick** — a toggle that excludes the previous winner, so you don't get "Tacos" three nights running.
- **History** — the last 100 spins, with the list they came from.
- **Installs like an app** — add it to your phone's home screen and it opens fullscreen, works offline.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app — HTML, CSS, and JS in one file. This is the only file you need to edit. |
| `manifest.json` | Makes it installable as a phone app (name, icons, colors). |
| `sw.js` | Service worker. Network-first, so your edits always show up right away; the cache is only an offline fallback. |
| `icon.svg`, `icon-*.png` | App icons. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is. |

## Editing it

**On desktop (here):** just ask, and the change gets made and pushed.

**On your phone:** open the repo in the GitHub mobile app → `index.html` → pencil icon → edit → Commit.
GitHub Pages redeploys in about a minute, then pull the app down to refresh.

**In the browser:** press `.` on the repo page to open the github.dev editor — a full VS Code, no install.

## Installing on your phone

- **iPhone:** open the live URL in Safari → Share → *Add to Home Screen*.
- **Android:** open in Chrome → menu → *Install app* / *Add to Home Screen*.

## Handy details

- Press <kbd>Space</kbd> on desktop to spin.
- The wheel picks the winner *first*, then animates to it — so the odds are exactly what the `%` says, not whatever the animation happens to land on.
- Your lists and history never leave your device. Clearing your browser data clears them too.
