# Chicken Road

A small browser game: guide a chicken across lanes of traffic. Every lane you cross raises your multiplier, and you can cash out at any time, or get hit and lose the round.

It is a single HTML file with no build step and no server. It uses **virtual coins only** (you start with 100). No real money, no accounts and no data is collected.

> **Play it:** https://linuxnicola007.github.io/chicken-road-game/

## How to play

1. Choose a bet (5, 10, 15 or 20 coins, or type 1 to 100).
2. Choose a difficulty. A harder level means a higher chance of being hit on each lane, and a bigger reward.
3. Press **PLAY**, then move the chicken one lane at a time:
   - `Space` or `→` : move forward
   - click the game area : move forward
   - `C` : cash out and keep the current multiplier
4. If a car hits the chicken, the round is lost.

| Difficulty | Chance of being hit per lane |
|---|---|
| Easy | 12% |
| Medium | 22% |
| Hard | 34% |
| Hardcore | 48% |

## Run it on your computer

No install is needed.

1. Download or clone this repository.
2. Double-click `index.html`. It opens in your browser.

```bash
git clone https://github.com/linuxnicola007/chicken-road-game.git
```

The page loads two fonts (Orbitron, Exo 2) from Google Fonts. Offline, the game still works with your system fonts.

## Good to know

- This is a **fun project, not a gambling product.** It uses play coins that cannot be bought or withdrawn.
- The "Live wins" ticker is decoration. It does not show real players.
- The round hash is built from random seeds created in your own browser, so it is **a visual effect, not a real "provably fair" guarantee**. A real provably fair system must publish a hash of the server seed *before* the round starts, which a pure browser game cannot do.
- This project is not affiliated with any commercial game or company that uses a similar name.

## Built with

Plain HTML, CSS and JavaScript (Canvas API, Web Crypto API for SHA-256).

## License

MIT. See [LICENSE](LICENSE).
