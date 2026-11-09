# Web accessibility release checks

[Start here](../README.md) · [Release test matrix](../07-report/release-matrix.md) · [Source register](../08-sources/sources.md)

Run applicable checks against the release candidate or the approved design. Record the environment and keep the evidence with the audit report.

## REL-A11Y-01 — Auto-rotating carousel while browsing

- **How to test** — If a carousel rotates automatically, move keyboard focus into it and hover over it. Check the stop control, that it does not resume after focus enters unless the user restarts it, and that slide changes do not displace the active task.
- **Suggested fix** — Follow the carousel pattern for rotation controls, focus, and announcements. Keep manual navigation available.
- **Sources** — [CAR](https://www.w3.org/WAI/ARIA/apg/patterns/carousel/), [WC](https://www.w3.org/TR/WCAG22/)

## REL-A11Y-02 — Reduced motion across animation engines

- **How to test** — Enable system reduced motion before opening a web build. Check CSS transitions, JavaScript animation, canvas or decorative media if used. Navigate to another route and retest.
- **Suggested fix** — Apply the preference wherever motion is generated. Use stable static or reduced states and preserve task feedback.
- **Sources** — [MOT](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-motion), [WC](https://www.w3.org/TR/WCAG22/)
