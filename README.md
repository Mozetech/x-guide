# Growing on X

A short guide to growing on X: six chapters of tactics, each illustrated with real posts that worked.

Live at **https://mozetech.github.io/x-guide/**

## Structure

- `index.html` — the whole site (styles and script inline, no build step, no dependencies)
- `assets/` — Fraunces webfont, post images, the Forkcast trailer, social card

Chapters: the basics, riding trends, starting from zero, borrowing audiences, in person, sharing your work. Each chapter is a swipeable carousel of cards; most cards embed a real post as evidence.

## Editing

Open `index.html` and edit directly. Cards live inside `<section class="panel">` blocks; an embedded post is an `<a class="xpost">` with the author block, text, media, and engagement counts.

To add a post example, copy an existing `.xpost` block, swap the href, avatar path, name, handle, text, media, and counts. Images go in `assets/` — resize to roughly 640px wide and save as JPEG to keep the page light.
