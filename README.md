# Arcane & Starlight Defense

A fantasy-and-sci-fi tower defense game that runs in a single web page. Built phase by phase from the project brief.

**Play:** https://luv4440sharma.github.io/Starlight-Defense/

## Current build: Phase 3 (towers)

All 12 towers from the brief, each with three tiers. At tier 2 you pick Branch A or B; tier 3 finishes that branch.

- Towers: Arcane Archer, Fire Brazier, Frost Obelisk, Rune Shrine, Thornwall, Ballista (fantasy); Tesla Coil, Laser Turret, Plasma Mortar, Gravity Well, Drone Hive, Ion Pulse (sci-fi)
- Attack types: homing shots, piercing bolts, lobbed shells with bomblets, chain lightning, ramping lasers, pulses, close-range auras, gravity pulls, hunting drones, and a support shrine that boosts nearby towers
- Effects on enemies: slow, freeze, stun, root, burn, bleed, armor removed, extra damage taken, knockback and pull, each with its own look
- Damage types (Pierce, Magic, Energy, Blast) and resistances are in the engine, ready for the Phase 4 enemies
- Targeting per tower: First, Last, Strong or Close
- Upgrade costs: tier 2 is 1.2x the build cost, tier 3 is 2x. Selling returns 70% of everything spent
- **Play** gives World 1 with its three towers. **Test mode** unlocks all 12 towers with 3000 coins and 12 waves of goblins that get tougher, plus +1000 coins and wave skip in the pause menu

## How it's built

- `index.html` is the whole game. Three.js (and its glow add-ons) loads from the jsDelivr CDN, and fonts from Google Fonts, so it needs internet.
- Towers, enemies, maps and waves live in the `CONTENT` block at the top of the script. New content is added there without changing the engine.
- The simulation runs at a fixed 60 steps per second, separate from drawing, so it plays the same at any frame rate.
- Add `?fps` to the link to show a frame counter.

## Controls (keyboard)

`1`-`9`, `0`, `-`, `=` towers · `T` change target · `U` upgrade to tier 3 · `Enter` start wave · `Space` pause · `F` speed · `S` sell selected · `Esc` cancel
