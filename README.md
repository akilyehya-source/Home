# Four Rooms

A phone app made of eleven 3D rooms.

1. **Library** - shelves of classic books. Tap a book.
2. **Game Room** - a desk computer with a retro desktop and 6 games, plus an arcade cabinet with 5 games.
3. **Lounge** - an interactive fireplace, a sofa you can sit on, a TV that plays your own videos, and a radio that plays your own music. Lights panel (dimmer, scenes, per-lamp switches, auto lights-off while a video plays), sleep timer and subtitles (.srt/.vtt).
4. **Observatory** - a telescope, orrery and globe.
5. **Tokyo Apartment** - a rainy city apartment.
6. **Forest Cabin** - a walkable forest with a two-story cabin, lake, boat, fishing, campfire, cooking, weather, seasons and a photo mode. Progress is saved on your phone.
7. **Office** - a classical executive office and personal workspace: a desk with four real drawers (media, books, professional files, and a private drawer with an optional passcode), a laptop with its own small desktop, file manager and careful web browser, a notebook that supports Arabic and English, tasks and projects, a photo frame, an adjustable brass lamp, curtains, an opening window, a fireplace, a book shelf you can read from, and five times of day. Everything is stored only on your phone.
8. **Sakura Garden** - a walkable Japanese garden: giant sakura trees with falling petals, four armchairs around a fire pit (firewood, ignite, extinguish, intensity), a koi pond with feeding, a waterfall and stream, a red arched bridge, a pavilion with sliding shoji doors and a working tea set, lanterns, six times of day, seven weather types, a relax mode and a photo album. Everything is saved on this device only.
9. **Engineering Studio (stages 1-2)** - a walkable design studio with working tools. Architectural floor-plan editor (walls, rooms, doors, windows, stairs, dimensions, exact numeric input, snapping, 3D view). NEW: urban planning and terrain editor (buildings with zoning, straight and curved roads, parks, water, parcels with exact areas, trees, streetlights, parking, bridges, grouping, layers, distance and area measurement, terrain raise/lower/smooth/flatten/slope brushes saved as a separate layer, plan and 3D views, JSON/PNG/OBJ export). The central city table shows the active urban project live. The terrain is a synthetic sample, not real geography. Not built yet: mechanical CAD, engine model, assembly, PDF/GLB/DXF export.
11. **Nexora Command Center (stages 1-2)** - six reassignable monitors (world dashboard, desktop, notes, browser, clock, phone, world map, engine viewer, retro games), presets, sit/stand, RGB gaming PC, four drawers, notebook, window with motorized blinds, lighting zones, save/restore. NEW: offline world-map table (political, simplified terrain, day/night layers, country facts, search, distance measure), four-stroke engine viewer (cutaway, transparent, solid, exploded, part info) and four original retro games (Cedar Run, Snake, Brick Smash, Merge). ChatGPT, TradingView and YouTube cannot be embedded (they show an explanation). The phone is simulated, not Android. Not built: real Android apps, multi-cylinder or 3D engine, real elevation data.

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
- After you replace `index.html` with a newer version, also change `VERSION` in `sw.js` (for example to `four-rooms-v15`) so phones pick up the update.
