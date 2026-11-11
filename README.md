# Orbital Siege

A Galaga-style arcade shooter in a single, dependency-free HTML file (`index.html`). Original sprites, bitmap font and synthesised sound; no build step — open the file in a browser.

## Controls
- Arrows or A/D — move
- Space (also Up/W/Z/X/Enter) — fire; hold for auto-fire
- P or Esc — pause
- On iPad with a keyboard, tap the game once so it receives key presses.

## Gameplay
- 40 enemies per stage fly in as squadrons, then settle into a breathing formation.
- Drones loop-the-loop on their dives; wasps zig-zag and U-turn back to formation; bosses sweep with escorts or use a tractor beam.
- A captured fighter can be rescued (shoot its boss while it dives) for twin fire.
- Every fourth stage from stage 3 is a challenging stage with a hit bonus.

## Code map (`index.html`)
- Sprites & palettes, 5x7 bitmap font
- WebAudio sound effects (with iOS audio unlock)
- Input (keyboard) and layout scaling
- Flight paths (Catmull-Rom splines)
- Stage building, enemy state machine (wait → path → home → form → dive/beam)
- Player, collisions, attack scheduler, rendering, fixed 60 Hz loop
