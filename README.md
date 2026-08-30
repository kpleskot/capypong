# capypong
A capybara table-tennis game in the browser

**Play it:** https://kpleskot.github.io/capypong (once GitHub Pages is turned on)

## How to play

Keep the rally going and beat the opposing capybara.

| Input | Action |
|-------|--------|
| Arrow keys or `A` / `D` | Move your paddle left and right |
| Mouse or touch | Steer the paddle directly |
| `Space` or click/tap | Serve the ball |
| `P` | Pause / unpause |
| `Esc` | Open the pause menu |

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
  drafts that shouldn't be published, and local session files.

To ignore something new, add one pattern per line: a trailing `/` means
"a folder", and `*` is a wildcard (so `*.bak` ignores every backup file).

## Roadmap

Ideas for future improvement. Each one becomes its own branch.

- [ ] (to be decided)

## Credits

Made by Kelly Lin.
