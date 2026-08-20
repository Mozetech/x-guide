# X Daily

A daily X-growth programme for a small cohort of founders and operators. The page combines five monitored daily KPIs with the sequence that makes them specific, four guidance sections, and a closing discipline practice. The methods are documented with real posts.

Live at **https://mozetech.github.io/x-guide/**

## Structure

- `index.html` — the whole site (styles and script inline, no build step, no dependencies)
- `assets/` — Fraunces webfont, retained post images, and the existing social card

The prerequisite sequence and five KPI rows are visible together. KPI examples use native, collapsed disclosures. The four guidance sections remain horizontally swipeable rows of cards, and Discipline is a separate closing block.

## Editing

Open `index.html` and edit directly. Guidance cards live inside `<section class="panel">` blocks; an embedded post is an `<a class="xpost">` with the author block, text, media, and engagement counts.

To add a post example, copy an existing `.xpost` block, swap the href, avatar path, name, handle, text, media, and counts. Images go in `assets/` — resize to roughly 640px wide and save as JPEG to keep the page light.
