# Cavern Miner

Platform game that runs in the browser from a single `index.html`. Collect every sparkle in the cavern to open the exit, then reach it before your lamp oil runs out.

## Caverns

There are 15 caverns, joined up into one mine:

1. **Caverns 1 to 13:** one screen each. Caverns 6 to 13 add conveyor floors.
2. **The Long Drift (14):** 2 × 2 screens, and the view scrolls to follow the miner.
3. **Deep Workings (15):** 3 × 3 screens, the finale.

On odd-numbered caverns you play the miner. On even-numbered caverns you play his skeleton, which handles the same way.

## Exits and the linked mine

Each exit is a hatch set into the cavern's outer wall, roof or floor. It stays dark until you collect every sparkle, then flashes. Touch it to go through. Where you leave sets where you arrive in the next cavern:

| You leave through | You arrive in the next cavern |
|---|---|
| The right wall | On the left, at the same height |
| The left wall | On the right, at the same height |
| The floor | Dropping in from the top. This drop never counts as a fatal fall. |
| The roof | Springing up from the bottom |

Entering one of the larger caverns, you can arrive at any height on that side. After losing a life you start again where you came in.

## Time

Each cavern's lamp oil is 30 seconds a screen, times the larger of its width or height in screens: 30 seconds for one screen, 60 for 2 × 2 and 90 for 3 × 3. An oil flask adds 10 seconds of lamp in any cavern, up to a full lamp. Every built-in cavern can be finished with at least 10 seconds of lamp to spare on its fastest route.

## Extra lives

You start with 3 lives and earn one more at 10,000 points, then at 20,000, 40,000, 80,000 and so on, doubling each time. The HUD shows up to 6 helmets, then one helmet and a count. Extra lives are not awarded in cheat mode or test play.

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
| Frame-time readout on/off | F |

## Hazards and pick-ups

| Thing | What it does |
|---|---|
| Sparkle | 100 points. Collect them all to open the exit. |
| Oil flask | 50 points and tops up your lamp. |
| Crumbling ledge | Collapses if you stand on it too long. |
| Crumbling block | A full square that holds you up from above and collapses if you stand on it too long. You can walk, run or jump through it. |
| Conveyor | A ledge that carries you left or right. Running against it is slower. A solid bar runs underneath, so you can't jump up through one. |
| Open belt | A conveyor with no bar underneath, so you can jump up through it. |
| Stalactite | Shakes, then falls when you pass beneath it, unless rock or a ledge is in the way. |
| Regrowing stalactite | Teal crystal. Falls like a stalactite, and a new one grows back 2 seconds after the last one shatters. |
| Spikes, slimes, bats, mushroom creatures | Lose a life on contact. |
| Spiders | Drop on a thread to the ledge or floor below, then climb back up. The large spider is two squares wide. |
| Flying monster | Flies faster than a bat, bobbing into the row above, and comes for you when you are within a square. A falling stalactite kills it. |
| Flying head | Two squares wide. Moves up to a square up or down to line up with you when you are within 2 squares. A stalactite snaps off a horn and shrinks its reach; lose both and it drops and crumbles. |
| Demon boss | Paces its ledge and throws a fireball along its row every 3 seconds. Three stalactite hits defeat it, for 5,000 points. |
| Skeleton lord | Lunges with its scythe when you are close on its level, then rests. Three stalactite hits defeat it, for 5,000 points. |
| Long falls | Falling more than 8 tiles, measured from the top of a jump, costs a life. |

Lamp oil left when you reach the exit is added to your score, at 20 points for each percent left (up to 2,000 for a full lamp). Losing a life resets the cavern, but sparkles you have already collected stay collected. The high score is saved in the browser.

## Cheat mode and level editor

On the welcome screen, type `cheap` (any capitals) to turn cheat mode on or off. With cheat mode on, you lose no lives or oil, scores are not saved, and:

- **1–9** starts at that cavern.
- **K** skips the current cavern during play.
- **L** opens the level editor. Press **H** in the editor for its controls. Use the arrow keys to scroll around caverns larger than the screen.

In the editor, **Z** and **X** pick the left and right conveyors, and **V** and **B** the open belts. The palette shows every tile in two rows, and the selected tile's key appears beside its name. Place the exit in the outer wall, roof or floor, and place the start where the cavern before it leads in.

Saved caverns are stored in the browser and replace the built-in ones there. Use **Shift+C** in the editor to copy all caverns as text, which can be shared or built into the game. The password sits in the page's code, so it is a fun lock, not security.

## Running locally

Open `index.html` in a modern browser. No build step or server is needed. `title.jpg` is the title-screen backdrop.
