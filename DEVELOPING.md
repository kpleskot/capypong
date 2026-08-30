# Developing capypong

The rule: `main` is always a working game. Every new feature or fix gets
its own branch, and reaches `main` through a pull request.

```
  main ─●───────────────────────────●──── merge ──►
         \                         /
          └─► my-feature ─●───●───┘
```

## The loop (repeat for every feature)

```bash
# 0. start from fresh main
git switch main
git pull

# 1. branch for ONE idea, named after it
git switch -c add-sound-effects

# 2. edit index.html, test by opening it in a browser

# 3. snapshot whenever something works (repeat with step 2)
git add .
git commit -m "Add paddle hit sound"

# 4. upload the branch
git push -u origin add-sound-effects

# 5. on github.com/kpleskot/capypong: click the yellow
#    "Compare & pull request" banner, describe the change,
#    create the PR, read your own diff, then Merge.

# 6. bring the merge home and clean up
git switch main
git pull
git branch -d add-sound-effects
```

## Rules of thumb

- One branch = one idea. "Sounds AND new levels AND a bug fix" is three branches.
- Commit small and often. A commit should finish one thought.
- Never commit directly on `main`. If `git status` says "On branch main"
  and you've edited files, make the branch first, then commit; the edits
  come with you.
- Stuck or broken? `git status` first. It almost always names the way out.
- Test in the browser before every commit: open `index.html`, play a rally.

## Where things go

- Game logic, styles, markup: all live in `index.html`
- Capybara faces: `faces.js`
- Messy experiments: a `scratch/` folder (gitignored, never published)
