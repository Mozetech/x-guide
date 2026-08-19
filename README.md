# Growing on X

Notes on audience growth on X. Six sections covering ranking signals, timing and search behavior, accounts without an audience, access to established audiences, offline gatherings, and publication of ongoing work. Each method is documented with a real post.

Live at **https://mozetech.github.io/x-guide/**

## Structure

- `index.html` — the whole site (styles and script inline, no build step, no dependencies)
- `assets/` — Fraunces webfont, post images, the Forkcast trailer, social card

Each section is a horizontally swipeable row of cards. A card states a method, explains the mechanism behind it, and where possible embeds the post that demonstrates it.

## Editing

Open `index.html` and edit directly. Cards live inside `<section class="panel">` blocks; an embedded post is an `<a class="xpost">` with the author block, text, media, and engagement counts.

To add a post example, copy an existing `.xpost` block, swap the href, avatar path, name, handle, text, media, and counts. Images go in `assets/` — resize to roughly 640px wide and save as JPEG to keep the page light.
