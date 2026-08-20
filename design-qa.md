# Design QA — foundations, TL;DR, Daily KPIs and General guidelines

## Evidence

- Source visual truth: `/var/folders/dt/crzw2ggj037964f9hc3swwwr0000gn/T/paseo-attachments-U57W8U/7d4b5accd6339060da5ea6f1cbdd735ff3ec7665a4ab0b464faa95b415c79563.png`
- Browser-rendered implementation region: `/tmp/x-guide-sequence-1120.png`
- Combined side-by-side comparison: `/tmp/x-guide-design-comparison.png`
- Current desktop flow: `/tmp/x-guide-flow-1120.png`
- Current mobile flow: `/tmp/x-guide-flow-375.png`
- Comparison viewport: 1120 CSS px wide, device scale factor 1.
- Source pixels: 1120 × 384.
- Implementation region pixels: 1120 × 292.
- Responsive evidence: 375 CSS px wide, device scale factor 1.
- State: static sequence cards; KPI examples closed by default.

## Full-view comparison

The page now reads in the requested order: opening paragraph fragment, four primary cards,
two de-emphasised gated cards, the simplified remainder of the first paragraph, a ruled TL;DR
of the daily order, and the Daily KPIs heading with the habituation paragraph directly beneath
it. The old order strip is gone. `General guidelines` is the verified heading after the KPI
section. The desktop and mobile captures show the revised top-of-page transition.

## Focused comparison

The combined comparison shows the same four-plus-two hierarchy, type treatment, palette,
rounded cards, number badges, gated styling and alignment as the reference. The implementation
is intentionally denser than the reference: primary cards measure about 231 × 147 px rather
than roughly 258 × 192 px, while gated cards measure about 354 × 85 px rather than roughly
396 × 109 px. This is the requested economy-of-space change, not design drift.

## Required fidelity surfaces

- Fonts and typography: passed. Existing Fraunces display type and the site's sans-serif body
  stack are preserved; hierarchy and wrapping remain clear at 1120 and 375 px.
- Spacing and layout rhythm: passed. The compact grid stays four columns on desktop and becomes
  a 2 × 2 grid on mobile; the gated pair centers below it and stacks on mobile.
- Colors and visual tokens: passed. All treatments continue to use the existing page, ink,
  faint-ink and accent tokens.
- Image quality and asset fidelity: passed. The reference contains UI components rather than
  separate raster assets; no source asset was replaced or approximated.
- Copy and content: passed. The strategy paragraph is now four shorter sentences without
  dropping its timing, in-person, prioritisation or interim-KPI meaning. The TL;DR, habituation
  placement, `Daily KPIs` heading and `General guidelines` heading match the requested order.

## Interaction and browser checks

- Rechecked at 375 and 1120 CSS px; the earlier 768 and 1440 checks remain valid for the
  unchanged KPI and carousel components.
- No page-level horizontal overflow at either current viewport.
- KPI disclosures open and close, and remain closed on initial load.
- Carousel keyboard navigation advances the active card and dot.
- Carousel next-button navigation advances the deck.
- Fonts load; referenced image files remain present and the visual cards are unchanged.
- No duplicate element IDs; the old order-strip component has no remaining instance.

## Findings

No actionable P0, P1 or P2 differences remain. No P3 follow-up is required for this pass.

## Comparison history

- Pass 1: the focused side-by-side comparison confirmed the intended smaller footprint while
  preserving the reference hierarchy and style.
- Pass 2: the revised prose flow, TL;DR placement, KPI intent placement and section naming were
  checked at desktop and mobile widths; no corrective iteration was required.

final result: passed
