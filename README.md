# RETRO RACER '92

A small browser-based homage to the top-down arcade racers of the early 90s. Pure HTML/CSS/JavaScript — no build step, no dependencies.

## Play

Open `index.html` in any modern browser, or visit the deployed site.

### Controls

| Key            | Action       |
| -------------- | ------------ |
| `Left / Right` | Steer        |
| `Up`           | Accelerate   |
| `Down`         | Brake        |
| `Space`        | Start / Restart |
| `P`            | Pause        |

## Features

- Pixelated cars drawn entirely on `<canvas>` (no image assets)
- Classic arcade palette: yellow road edges, dashed white lane lines, green grass shoulders
- 8-bit "Press Start 2P" font for the HUD
- Three-lane traffic with random spawn patterns
- Difficulty ramps with score: faster scroll, denser traffic
- Persistent high score via `localStorage`
- Attract-mode title screen with blinking "PRESS SPACE"

## Tech

Single static file — `index.html` — containing the markup, styles, and game loop. Render uses `requestAnimationFrame`; collisions are simple AABB rectangle checks. The Google Fonts "Press Start 2P" face is the only external dependency.

## Deploy

The repository is Netlify-ready. The included `netlify.toml` sets the publish directory to the repo root, so connecting the repo on Netlify (or dragging the folder into the Netlify deploys UI) is enough.
# retro-racer-92
