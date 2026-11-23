# HUNCHBACK

A browser remake of the classic **Commodore 64** platformer *The Hunchback* — rebuilt with modern, hand-polished graphics, 16-bit-style animation and sound, while keeping the original's simple, brutal, one-button-jump gameplay.

Play it on your phone, tablet or PC. No App Store, no account, no download of a big app: open the link, add it to your Home Screen, and play full-screen — even offline.

![Hunchback](img/icon_512.png)

---

## The game

You are **Quasimodo**. Run along the castle walls, leap over the gaps between the battlements, dodge arrows, spears, boulders and fireballs, and ring the **bell** at the end of every level. After 15 levels you reach the tower where the **Princess** is waiting.

- **15 levels** per stage, from a sunny dawn to starry night skies
- Pits guarded by **knights with spears**, flying **arrows and spears**, catapult **boulders**, **fireballs**
- Big pits crossed by a **swinging rope** (levels 4, 8 and 12)
- A **knight chasing you** along the walls — don't let him catch you
- **5 lives**, shown as bells in the HUD; earn extra lives with the bonus levels
- **Bonus rounds** and a **Super Bonus** at the end of each stage
- After every stage the whole castle comes back **faster** and meaner
- **High-score table** with 3-letter names, just like in the old days
- Rare surprises in the sky and on the ground... keep your eyes open

Scoring is based on how fast you reach the bell, but the timer is hidden — you'll just have to be quick.

### Controls

| | Move | Jump | Pause |
|---|---|---|---|
| **Keyboard** | Arrows or Z / X | Space | P or Esc |
| **Touch (phone/tablet)** | On-screen arrows | JUMP button | — |
| **Gamepad** | D-pad / stick | A or X | Start |

Menus: arrows or W A S Z to move, Space / Enter to select.

---

## Inspiration

*The Hunchback* is a 1980s home-computer classic that many of us played on the **Commodore 64**: a simple, addictive side-scrolling run along castle ramparts, with Quasimodo racing to ring the bell and rescue Esmeralda. Chunky pixels, bleeping jingles and a game that was fair only if you had perfect timing.

This project is a **tribute and a remaster** of that experience: the same structure and spirit — jump the gaps, avoid the arrows, ring the bell, reach the Princess — with redrawn artwork, parallax-style backgrounds, animated torches, flags, dragons and horses, and an orchestral soundtrack, plus modern controls (touch, keyboard and gamepad).

The credits screen even hides a link to the **original C64 version**, so you can compare then and now.

> This is an unofficial, non-commercial fan project, made with love for retro gaming. It is not affiliated with or endorsed by the original game's authors or publishers. All trademarks belong to their respective owners.

---

## Install on iPhone (and iPad)

Hunchback is a **PWA** (Progressive Web App): it installs from Safari and behaves like a normal app.

1. On your iPhone, open the game link **in Safari** (it must be Safari, not Chrome or other browsers):
   **`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`**
2. Tap the **Share** button (the square with an arrow, at the bottom of the screen).
3. Scroll down and tap **"Add to Home Screen"**, then tap **Add**.
4. Open **Hunchback** from your Home Screen. It runs full-screen, with no browser bars.

Tips:

- **Turn the phone sideways.** In portrait mode the game asks you to rotate it.
- **Use Wi-Fi the first time.** The first launch downloads about 50 MB of graphics and music; after that, the game works **offline**.
- **Sound starts after your first tap** (an iOS rule for every web app).
- Updating: when a new version is published, open the app while online and **close and reopen it once or twice** to refresh the cache. If it doesn't update, delete the Home Screen icon and add it again.
- Android works the same way: open the link in Chrome → menu → **Install app** / **Add to Home screen**.

On a computer just open the link in any modern browser (Chrome, Edge, Firefox, Safari).

---

## Technical notes

- Pure HTML5 canvas, vanilla JavaScript, one `index.html`; no frameworks, no external servers.
- Offline support through a Service Worker (`sw.js`) and a Web App Manifest (`manifest.json`).
- Images are WebP; the music loops use WAV/M4A, effects use MP3.
- Also available as a Windows desktop app (Electron).

### Run it locally

Browsers block some features on `file://`, so serve the folder with any static server, for example:

```
python -m http.server 8000
```

then open `http://localhost:8000/`.

### Publish your own copy (GitHub Pages)

Upload the files so that `index.html` sits in the repository root, then go to **Settings → Pages → Deploy from a branch → `main` / `(root)`**. When you update the game, change `VER` in `sw.js` so players get the new version.

---

## Credits

- Game design, art direction and testing: **Gigi Giublena**
- Built with **Claude** by Anthropic
- Inspired by *The Hunchback* for the Commodore 64

© Gigi Giublena. All rights reserved.
