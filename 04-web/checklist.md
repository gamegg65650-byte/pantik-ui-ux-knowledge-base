# Websites and web apps

[Start here](../README.md) · [Source register](../08-sources/sources.md)

## WEB-01 — Browsers and viewport widths

- **Applies to** — Web
- **How to test** — Test supported browsers and a real phone. Start with 320, 390, 768, and 1280 CSS pixels and include widths near layout changes.
- **Suggested fix** — Fix overlapping content and horizontal overflow. Verify touch and keyboard navigation.
- **Sources** — [M3](https://m3.material.io/foundations/)

## WEB-02 — Links and routes

- **Applies to** — Web
- **How to test** — Check external links, anchors, direct URLs, refresh, Back, and an invalid route.
- **Suggested fix** — Fix link destinations and routing. Provide a clear way out of the 404 page.
- **Sources** — [GD](https://design.google/?home=)

## WEB-03 — Core Web Vitals

- **Applies to** — Web
- **How to test** — Review field results by device. Good at the 75th percentile means LCP ≤ 2.5 s, INP ≤ 200 ms, and CLS ≤ 0.1. Record lab results separately when field data is unavailable.
- **Suggested fix** — Optimize the largest content resource, reduce long tasks, and reserve media dimensions. Measure again.
- **Sources** — [WV](https://web.dev/articles/vitals)

## WEB-04 — Media and layout shifts

- **Applies to** — Web
- **How to test** — Use a slow connection and watch for shifts when images, video posters, and fonts load.
- **Suggested fix** — Reserve dimensions, add posters, and set loading priorities based on visibility.
- **Sources** — [WV](https://web.dev/articles/vitals)

## WEB-05 — Forms and network failures

- **Applies to** — Web
- **How to test** — In a test environment, check success, server error, timeout, and retry after recovery.
- **Suggested fix** — Explain failure, allow a retry, and retain fields that are safe to restore.
- **Sources** — [GD](https://design.google/?home=)

## WEB-06 — Automated and manual accessibility

- **Applies to** — Web
- **How to test** — Run Lighthouse or axe on key pages and states. Separately test keyboard operation, screen-reader output, form errors, and dialogs.
- **Suggested fix** — Confirm automated signals manually and record reproducible evidence.
- **Sources** — [WAI](https://www.w3.org/WAI/test-evaluate/preliminary/)

## WEB-07 — Metadata and link previews

- **Applies to** — Web
- **How to test** — Check the browser title, page language, heading, and social preview where relevant.
- **Suggested fix** — Use a unique title, correct lang, and a consistent set of preview metadata. Verify the deployed preview.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/), [GD](https://design.google/?home=)
