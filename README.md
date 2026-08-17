# 4-Week Trainer

A single-page workout tracker: Piernas / Espalda / Hombro / Brazos over 4 weeks,
with a session chronometer, per-block timers, 2-minute rests and statistics.

## Put it on your phone's home screen

1. Upload every file in this folder to a repository, keeping them at the top level.
2. Repository **Settings -> Pages -> Source: Deploy from a branch -> main / (root)** -> Save.
3. Wait a few minutes, then open `https://<your-user>.github.io/<repo>/` on your phone in Chrome.
4. Chrome menu (three dots) -> **Add to Home screen** / **Install app**.

It then opens full screen with its own icon, and works offline after the first load.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app - exercises, illustrations, timers, statistics |
| `manifest.webmanifest` | Name, icon and full-screen behaviour for the home-screen shortcut |
| `sw.js` | Service worker; caches the app so it runs without internet |
| `icon-*.png` | App icons |

## Updating

Replace `index.html`, then bump `CACHE = "gym-trainer-v1"` to `v2` in `sw.js`
so phones pick up the new version instead of the cached one.

## Credits

Exercise illustrations by [Everkinetic](https://github.com/everkinetic/data),
licensed [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
