# Arcane & Starlight Defense

A fantasy-and-sci-fi tower defense game that runs in a single web page. Built phase by phase from the project brief.

**Play:** https://luv4440sharma.github.io/Starlight-Defense/

## Current build: Phase 1 (engine, 2.5D)

- 2.5D Three.js scene with a fixed angled camera, lights and shadows
- One path from the spawn portal to the crystal, goblins that walk it
- Lives, coins, one Arcane Archer tower, one wave of 18 goblins
- Select a tower to see its range and stats, or sell it for 70%
- Pause, 1×/2× speed, settings and run stats saved in the browser
- Mouse and touch: on a phone, tap once to preview a tower, tap again to build

Visuals are placeholder shapes until a style is picked in Phase 2.

## How it's built

- `index.html` is the whole game. Three.js loads from the jsDelivr CDN, so it needs internet.
- Towers, enemies, maps and waves live in the `CONTENT` block at the top of the script. New content is added there without changing the engine.
- The simulation runs at a fixed 60 steps per second, separate from drawing, so it plays the same at any frame rate.
- Add `?fps` to the link to show a frame counter.

## Controls (keyboard)

`1` Arcane Archer · `Enter` start wave · `Space` pause · `F` speed · `S` sell selected · `Esc` cancel
