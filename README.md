# Four Rooms

A phone app made of four 3D rooms.

1. **Library** - shelves of classic books. Tap a book.
2. **Game Room** - a desk computer with a retro desktop and 6 games, plus an arcade cabinet with 5 games.
3. **Lounge** - an interactive fireplace, a sofa you can sit on, a TV that plays your own videos, and a radio that plays your own music.
4. **Room 4** - empty for now.

It works offline once it has loaded one time. Scores, saves, imported videos and imported music are stored on your phone only.

## Put it online with GitHub Pages (free)

1. Create a new GitHub repository (for example `four-rooms`). Public is fine.
2. Upload everything in this folder to the repository root: `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll` and the `icons` folder. On github.com use **Add file > Upload files** and drag them in.
3. Open the repository **Settings > Pages**. Under **Build and deployment** choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then **Save**.
4. After a minute your app is at `https://YOUR-NAME.github.io/four-rooms/`.

## Install on your phone

Open that address on your phone first, and keep the screen on until the rooms appear (this saves the app for offline use).

- **Android (Chrome):** menu (three dots) > **Install app** or **Add to Home screen**.
- **iPhone (Safari):** Share button > **Add to Home Screen**.

Open it from the new icon. After that it also starts with no internet.

## Good to know

- Imported videos and music live in the browser storage of the installed app. They stay after you close the app or restart the phone. If you clear the site data for the app, they are removed. Your original files are never touched.
- Video playback uses your phone's own decoders. MP4 (H.264) and WebM play almost everywhere. MKV, AVI, WMV, MPEG, TS, 3GP, H.265 and AV1 depend on the phone. If a file will not play, convert it to MP4 (H.264 and AAC) with a free tool such as HandBrake or VLC.
- iPhone only: if you do not open the app for several weeks, Safari can free up its storage. Re-import if that happens.
- After you replace `index.html` with a newer version, also change `VERSION` in `sw.js` (for example to `four-rooms-v2`) so phones pick up the update.
