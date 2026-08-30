# CLAUDE.md — project guide for AI assistants

## What this is

Capy Pong: a capybara table-tennis browser game. The maintainer (Kelly) is
learning software development through this project and has no prior
programming background — explain changes in plain English, avoid unexplained
jargon, and prefer walking through *why* over dumping code.

## Architecture

- `index.html` — the entire game: CSS, HTML markup, and all JavaScript in one
  file. Canvas-based rendering, no frameworks, no dependencies.
- `faces.js` — character portrait PNGs embedded as base64 data URIs. Large
  (300KB+) but only 8 lines; treat it as a binary asset, don't reformat it.
- There is deliberately **no build step, no package.json, no tooling**. The
  game runs by opening `index.html` in a browser. Keep it that way unless
  Kelly explicitly decides otherwise.

## Workflow (see DEVELOPING.md for the full loop)

- `main` must always be a playable game. Never commit directly to `main`.
- One branch per idea, merged via pull request on GitHub.
- Test before every commit: open `index.html` in a browser and play a rally.

## Off-limits for git

- `documents/` — Kelly's sensitive artifacts. Gitignored; never commit,
  read only if asked.
- `scratch/`, `notes/` — gitignored scratch space.
