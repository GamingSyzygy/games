# games

Browser games, one folder per game. Each game is a self-contained `index.html` that runs in any modern browser with no build step.

## Games

| Game | Folder | Status | Play |
|---|---|---|---|
| Galaxy Raiders | [`galaxy-raiders/`](galaxy-raiders/) | Playable | https://gamingsyzygy.github.io/games/galaxy-raiders/ |
| Manix Miner | [`manix-miner/`](manix-miner/) | In development | Not yet published |

The site root (https://gamingsyzygy.github.io/games/) is a menu linking to each game.

## Repository layout

```
/
├── index.html            Games menu (GitHub Pages root)
├── README.md
├── galaxy-raiders/
│   ├── index.html        Game entry point
│   └── README.md
└── manix-miner/
    └── README.md
```

## Adding a game

1. Create a folder named after the game in lower-case kebab-case, e.g. `my-new-game/`.
2. Put the game's entry point at `my-new-game/index.html`, with any assets alongside it. Use relative paths only.
3. Add a `README.md` in the folder covering what the game is, its controls and its status.
4. Add the game to the table above and to the menu in the root `index.html`.
