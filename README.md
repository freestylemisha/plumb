# Plumb

Play: **https://plumb.dailyplumb.workers.dev**

A daily test of physical intuition. Five tests, two rounds each, scored out of 1000:

- **Level**: a glass of water tilts. Draw where the surface sits.
- **Spin**: a wheel slows down behind a cover. Mark where the red slice stops.
- **Lamp**: posts cast shadows. Find the hidden lamp.
- **Fold**: paper is folded once or twice and a hole is punched through it. Mark where all the holes are.
- **Bank**: a pool shot vanishes. Mark where it meets the far rail.

Every test starts with a short how-it-works card and an optional practice round that doesn't count. Everyone gets the same set each day. Puzzle No. 1 is 9 November 2026.

## Files

- `index.html`, `style.css`, `plumb.js`: the whole game. Plain HTML, CSS and JavaScript with no build step.
- `supabase-setup.sql`: creates the leaderboard table. Run it once in the Supabase SQL Editor.

## Leaderboard

Scores go to Plumb's own Supabase project (`qxlixocgdmhgxwwpfwta`). Its URL and **publishable** key are set in `LB` in `plumb.js`; the publishable key is meant to be public, and the table's rules decide what it can do. Clear both and the game still works, with the leaderboard switched off.

## Hosting

Hosted on Cloudflare Workers as static files (`wrangler.jsonc`). Every push to `main` redeploys it. `.assetsignore` keeps everything except the game files off the site.
