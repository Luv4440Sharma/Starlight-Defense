# Arcane & Starlight Defense

A fantasy-and-sci-fi tower defense game that runs in a single web page. Built phase by phase from the project brief.

**Play:** https://luv4440sharma.github.io/Starlight-Defense/

## Current build: Phase 2 (visual direction, style D)

Style D: crisp sci-fi with magic accents. World 1 is an overgrown outpost.

- Board: metal deck tiles with moss, vines and grass, a glowing hologram path that flows toward the core, and a forest with tech beacons around the platform
- Models: Arcane Archer turret with a hologram bow and a spinning rune ring, goblins in tech gear, an energy core in a metal cradle, and a rift gate
- Lighting: cool key light, cyan and violet rim lights, soft shadows, metal reflections, and bloom (glow) on High quality
- Effects: towers scan in as holograms and scan out when sold, defeated enemies dissolve, shots leave trails and sparks, wave banners
- Sci-fi screen layout, plus a Settings screen (graphics quality High/Low, screen shake On/Off) saved in the browser
- All colours and materials come from one `STYLE` kit, so later towers and enemies match

Phase 1 engine features are unchanged: one Arcane Archer tower, one wave of 18 goblins, sell for 70%, pause and 1×/2× speed, mouse and touch.

## How it's built

- `index.html` is the whole game. Three.js (and its glow add-ons) loads from the jsDelivr CDN, and fonts from Google Fonts, so it needs internet.
- Towers, enemies, maps and waves live in the `CONTENT` block at the top of the script. New content is added there without changing the engine.
- The simulation runs at a fixed 60 steps per second, separate from drawing, so it plays the same at any frame rate.
- Add `?fps` to the link to show a frame counter.

## Controls (keyboard)

`1` Arcane Archer · `Enter` start wave · `Space` pause · `F` speed · `S` sell selected · `Esc` cancel
