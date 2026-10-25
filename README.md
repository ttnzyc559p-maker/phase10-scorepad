# Phase 10 Scorepad

A phone-friendly scorekeeper for the Phase 10 card game. One person keeps score on their phone while everyone plays.

## What it does

- Set up 2 to 6 players in seating order. The app shows who deals each hand.
- After each hand, tick whether each player made their phase and enter the points left in their hand. Card buttons add the right value: +5 for 1–9, +10 for 10–12, +15 for Skip, +25 for Wild.
- Standings rank players by phases completed, then by fewest points, with a 10-step progress bar for each player.
- Tap any past hand to fix or delete it.
- When someone completes Phase 10, the app names the winner: the player who finished Phase 10 with the fewest points.
- A built-in reference lists all 10 phases and the card values.

The game is saved in the browser's local storage, so it survives a refresh or closing the tab. It does not sync between devices.

## Run it

It's one static page with no build step. Open `index.html` in a browser, or serve the folder:

```sh
npx serve .
```

## Publish it with GitHub Pages

1. Push this repository to GitHub.
2. In the repository, go to **Settings → Pages** and set **Source** to **GitHub Actions**.
3. The workflow in `.github/workflows/deploy.yml` publishes the site on every push to `main`. The address is `https://<your-username>.github.io/phase10-scorepad/`.

On a phone, open that address and use **Add to Home Screen** to get an app icon.
