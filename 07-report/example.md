# Worked example

This is an illustrative issue on a fictional portfolio.

## AUD-001 — Sticky header hides a focused project link

- **Checklist ID and priority** — A11Y-05, P1. The keyboard user loses their visible position in the gallery.
- **Conditions** — Portfolio page at 390 CSS pixels with the sticky header enabled.
- **Steps** — Open the gallery and press Tab until the first project-card link receives focus.
- **Actual result** — The link receives focus, but the header fully covers it.
- **Expected result** — The focused link remains at least partially visible and has a visible focus indicator. See [WCAG 2.2](https://www.w3.org/TR/WCAG22/#focus-not-obscured-minimum).
- **Evidence to attach** — A screenshot and the browser and build versions.
- **Suggested fix** — Account for header height when scrolling focused items into view, for example with scroll-padding-block-start on the relevant scroll container.
- **Acceptance check** — Repeat Tab and Shift+Tab at narrow and wide widths and with any optional banner open and closed.
