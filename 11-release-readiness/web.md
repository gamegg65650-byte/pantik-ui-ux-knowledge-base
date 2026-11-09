# Web release checks

[Start here](../README.md) · [Release test matrix](../07-report/release-matrix.md) · [Source register](../08-sources/sources.md)

Run applicable checks against the release candidate or the approved design. Record the environment and keep the evidence with the audit report.

## REL-WEB-01 — First-visit overlays and primary actions

- **How to test** — Open a clean session at a narrow width with storage preferences unset. Check whether the banner covers the main action, whether its controls work with keyboard input, and whether the underlying task resumes after dismissal.
- **Suggested fix** — Keep the main task visible when possible. Match the overlay's interaction and focus behavior to whether it is modal.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/), [FOCUS](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum)

## REL-WEB-02 — Shareable filter and history state

- **How to test** — Select a meaningful filter, open a detail page, then use Back and Forward. Refresh or open the filtered URL in a fresh tab if the filter is meant to be shareable.
- **Suggested fix** — Encode shareable state in the URL and restore it from navigation. Preserve transient UI state only where the journey calls for it.
- **Sources** — [HIST](https://developer.mozilla.org/en-US/docs/Web/API/History_API/Working_with_the_History_API)

## REL-WEB-03 — Focus after client-side navigation

- **How to test** — With the keyboard, activate a route-changing link. Check the document title, focus position, and next Tab stop. Repeat when returning to a list and check that focus and scroll return to a useful location.
- **Suggested fix** — Define focus behavior for route transitions. Use a meaningful heading or main region as a destination when appropriate, and restore the trigger on return when it still exists.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/), [HIST](https://developer.mozilla.org/en-US/docs/Web/API/History_API/Working_with_the_History_API)

## REL-WEB-04 — Social preview source markup

- **How to test** — Inspect the server-delivered head and the rendered head for the same public route. Compare og:title, og:description, og:image and og:url with the actual project. Check that the preview image loads without a session.
- **Suggested fix** — Generate one intended value for each singleton tag and remove conflicting defaults. Use absolute, publicly accessible image URLs.
- **Sources** — [OG](https://ogp.me/)

## REL-WEB-05 — Real HTTP status for a missing route

- **How to test** — Request an invalid public URL directly and check the HTTP status as well as the visible error page. Check that the recovery link works.
- **Suggested fix** — Return an appropriate 404 or 410 for permanently missing content and render the recovery page with that status.
- **Sources** — [HTTP404](https://developers.google.com/search/docs/crawling-indexing/troubleshoot-crawling-errors)

## REL-WEB-06 — Indexable language URLs

- **How to test** — For languages intended to appear separately in search, open each published locale URL directly in a fresh session. Check the initial language, self or intended canonical URL, and reciprocal hreflang links.
- **Suggested fix** — Use stable locale URLs with matching content and consistent canonical and alternate declarations. Mark this check not applicable if the project has no separate indexable language URLs.
- **Sources** — [LOCALE](https://developers.google.com/search/docs/specialty/international/localized-versions), [CANON](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls)

## REL-WEB-07 — Image variants and LCP priority

- **How to test** — With a cold cache, compare the downloaded image URLs and sizes on narrow and wide screens. Locate the measured LCP element. Check that responsive selection matches layout and that a visible LCP image is not lazy-loaded.
- **Suggested fix** — Use width-appropriate assets with srcset and sizes where suitable. Reserve image dimensions and prioritize the measured LCP image when appropriate.
- **Sources** — [IMG](https://web.dev/learn/images/descriptive), [LCP](https://web.dev/articles/optimize-lcp)

## REL-WEB-08 — Clipboard failure recovery

- **How to test** — Exercise a Copy action when clipboard writing fails or is denied. Confirm that the page does not announce success and the user can still select and copy the content.
- **Suggested fix** — Handle the rejected write and offer a selectable text fallback. Announce success only after the write succeeds.
- **Sources** — [CLIP](https://developer.mozilla.org/en-US/docs/Web/API/Clipboard/writeText)
