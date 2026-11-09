# Cavern Miner

Platform game that runs in the browser from a single `index.html`. Collect every sparkle in the cavern to open the exit, then reach it before your lamp oil runs out.

## Caverns

There are 7 caverns. The first two are larger than the screen, and the view scrolls to follow the miner:

1. **The Long Drift:** 2 × 2 screens.
2. **Deep Workings:** 3 × 3 screens.
3. **Caverns 3 to 7:** one screen each.

On odd-numbered caverns you play the miner. On even-numbered caverns you play his skeleton, which handles the same way.

## The lamp

As the oil burns down, your circle of light shrinks to 40% of its full size at 20% oil, then holds there. Below 20% the lamp sputters out every 3 seconds. Each blackout lasts longer as the oil runs out, from 0.1 to 0.6 seconds. Sparkles and the open exit still glow in the dark.

**Play:** https://gamingsyzygy.github.io/games/cavern-miner/

## Controls

| Action | Keys |
|---|---|
| Move | Left / Right arrows, or A / D |
| Jump | Space, Up arrow or W |
| Pause | P |
| Sound on/off | M |
| Quit to title | Esc |

## Hazards and pick-ups

| Thing | What it does |
|---|---|
| Sparkle | 100 points. Collect them all to open the exit. |
| Oil flask | 50 points and tops up your lamp. |
| Crumbling ledge | Collapses if you stand on it too long. |
| Stalactite | Shakes, then falls when you pass beneath it. |
| Spikes, slimes, bats | Lose a life on contact. |
| Long falls | Falling more than 8 tiles, measured from the top of a jump, costs a life. |

Lamp oil left when you reach the exit is added to your score. Losing a life resets the cavern, but sparkles you have already collected stay collected. The high score is saved in the browser.

## Cheat mode and level editor

On the welcome screen, type `cheap` (any capitals) to turn cheat mode on or off. With cheat mode on, you lose no lives or oil, scores are not saved, and:

- **1–9** starts at that cavern.
- **K** skips the current cavern during play.
- **L** opens the level editor. Press **H** in the editor for its controls. For caverns larger than the screen, the editor shows only the top-left screen for now.

Saved caverns are stored in the browser and replace the built-in ones there. Use **Shift+C** in the editor to copy all caverns as text, which can be shared or built into the game. The password sits in the page's code, so it is a fun lock, not security.

## Running locally

Open `index.html` in a modern browser. No build step or server is needed. `title.jpg` is the title-screen backdrop.
