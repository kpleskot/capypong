# capypong
A capybara table-tennis game in the browser

**Play it:** https://kpleskot.github.io/capypong (once GitHub Pages is turned on)

## What's in the game

- **Six playable capybaras**, each with their own style and special serve:
  Mochi the All-Rounder, Turbo the Speedster, Boba the Wall, Yuzu the
  Trickster, Sakura the Flutterer, and Momo the Slugger.
- **Three modes:** Quick Match (first to 3–15 points, your choice),
  Survival (play till you lose, difficulty keeps climbing), and
  Tournament (beat all five rivals in a row).
- **Obstacle Course toggle:** crated capy pups, steamy hot springs,
  yuzus, and warm rocks dot the table and boomerang the ball back.
- **Onsen Rating:** a chess-style skill rating that rises and falls
  with your wins and losses, saved in your browser.
- **Milestones and a leaderboard** to track your best runs.

## How to play

Keep the rally going and beat the opposing capybara.

| Input | Action |
|-------|--------|
| Arrow keys or `A` / `D` | Walk your capybara left and right |
| Mouse or touch | Your capybara follows the cursor (or your finger) |
| `Space` or click/tap | Serve the ball |
| `P` | Pause / unpause |
| `Esc` | Open the pause menu |

### Power-ups (optional)

Tick the **Power-Ups** box on the menu and treats appear on the table
during rallies. Whoever touched the ball last collects them:

- 🍃 **Leaf** — your capy snacks it and grows extra chonky for about
  ten seconds, blocking more shots.
- 🔥 **Flame** — arms your next return: one fiery, extra-fast shot.
- 🐾 **Capy pup** — a little helper guards your back line for about
  fifteen seconds.
- **Combo:** grab a leaf while your pup is out and the pup shares the
  snack and grows big too.

The rival capybara can collect power-ups the same way, so watch who
touched the ball last.

## Run it locally

1. Download or clone this repo.
2. Open `index.html` in any browser. No install, no build step.

## What each file is

| File | What it is |
|------|-----------|
| `index.html` | The whole game: HTML, CSS, and JavaScript in one file |
| `faces.js` | Capybara face graphics used by the game |
| `README.md` | This page. GitHub shows it on the repo's front page |
| `.gitignore` | Tells git which files to pretend don't exist (see below) |
| `LICENSE` | Apache 2.0: anyone may use this code if they credit the author |

## About the .gitignore

Anything matching a pattern in `.gitignore` never shows up in `git status`
and never gets committed or pushed. This repo's file has two parts:

- **GitHub's Python template** (the long top section), kept in case the
  project grows Python tooling later.
- **Web project extras** (the short bottom section): operating system junk
  files, personal editor settings, `scratch/` and `notes/` folders for
  drafts that shouldn't be published, a `documents/` folder for sensitive
  artifacts that must never reach GitHub, and local session files.

To ignore something new, add one pattern per line: a trailing `/` means
"a folder", and `*` is a wildcard (so `*.bak` ignores every backup file).

## Roadmap

Ideas for future improvement. Each one becomes its own branch.

- [ ] **Power-ups** — leaf (your capy grows chonky), flame (one fiery
  return), and a capy pup helper. In progress on the `add-power-ups` branch.
- [ ] **Hot-springs progression** — the reward for winning a round is a
  trip to a different hot spring to chill in.
- [ ] **Multiball mode** — more than one ball in play at once, possibly
  as a power-up.
- [ ] **Extra points** — special ways to score bonus points; many kinds
  are possible.
- [ ] **Sabotage items** — Mario Kart-style: boost yourself, or briefly
  (and visibly, and funnily) inconvenience your rival.

## Credits

Made by Kelly Lin.
