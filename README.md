# Risk Board Game Online

A browser version of the classic **Risk** board game — no install, no server, no build step. Two to six players share one screen (hot-seat) and take turns.

## Play it

The whole game is a single `index.html`, so it runs anywhere:

- **GitHub Pages (recommended):** go to this repo's **Settings → Pages**, set *Source* to **Deploy from a branch**, pick your branch (e.g. `main`) and the `/ (root)` folder, and save. After a minute the game is live at `https://<your-username>.github.io/riskboardgameonline/`.
- **Locally:** just open `index.html` in a browser.

## Features

- Classic world map: 42 territories, 6 continents, standard Risk adjacencies (including Alaska ↔ Kamchatka).
- 2–6 players, hot-seat on one screen; starting armies per the official rules (40/35/30/25/20).
- Random territory deal, then alternating initial placement (with an auto-place option).
- Reinforcements: `max(3, territories ÷ 3)` + continent bonuses (NA 5, SA 2, EU 5, AF 3, AS 7, AU 2).
- Dice battles: attacker up to 3 dice, defender up to 2, ties go to the defender, with a Blitz button to roll until decided.
- Full 44-card deck (42 territory cards + 2 wilds) with escalating trade-ins (4, 6, 8, 10, 12, 15, +5…), the +2 owned-territory bonus, forced trades at 5+ cards, and card capture on elimination.
- One fortify move per turn, game log, and auto-save to `localStorage` so a refresh doesn't lose the game.

## How to play

Click **Rules** in the game header for the full rules summary. Quick version: each turn you **Reinforce** (place new armies), **Attack** (pick your territory, then an adjacent enemy, and roll), and **Fortify** (one move between adjacent friendly territories). Conquer at least one territory in a turn to draw a card. Conquer the world to win.
