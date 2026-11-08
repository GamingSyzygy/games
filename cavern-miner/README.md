# Cavern Miner

Single-screen platform game that runs in the browser from a single `index.html`. Collect every sparkle in the cavern to open the exit, then reach it before your lamp oil runs out. As the oil burns down, your circle of light shrinks.

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

Lamp oil left when you reach the exit is added to your score. Losing a life resets the cavern, but sparkles you have already collected stay collected. The high score is saved in the browser.

## Cheat mode and level editor

On the welcome screen, type `cheap` (any capitals) to turn cheat mode on or off. With cheat mode on, you lose no lives or oil, scores are not saved, and:

- **1–9** starts at that cavern.
- **K** skips the current cavern during play.
- **L** opens the level editor. Press **H** in the editor for its controls.

Saved caverns are stored in the browser and replace the built-in ones there. Use **Shift+C** in the editor to copy all caverns as text, which can be shared or built into the game. The password sits in the page's code, so it is a fun lock, not security.

## Running locally

Open `index.html` in a modern browser. No build step or server is needed. `title.jpg` is the title-screen backdrop.
