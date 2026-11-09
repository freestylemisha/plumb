# Plumb

A daily test of physical intuition. Five tests, two rounds each, scored out of 1000:

- **Level**: a glass of water tilts. Draw where the surface sits.
- **Spin**: a wheel slows down behind a cover. Mark where the red slice stops.
- **Lamp**: posts cast shadows. Find the hidden lamp.
- **Hold**: hold for as long as a real event lasts.
- **Bank**: a pool shot vanishes. Mark where it meets the far rail.

Everyone gets the same set each day. Puzzle No. 1 is 9 November 2026.

## Files

- `index.html`, `style.css`, `plumb.js`: the whole game. Plain HTML, CSS and JavaScript with no build step.
- `supabase-setup.sql`: creates the leaderboard table. Run it once in the Supabase SQL Editor.

## Leaderboard

Set `LB.url` and `LB.key` near the top of the leaderboard section in `plumb.js` to the Supabase project's URL and **publishable** key. With both empty, the game still works and the leaderboard says it isn't switched on yet.

## Hosting

Any static host works. On GitHub Pages: Settings → Pages → Deploy from a branch → `main`, folder `/ (root)`.
