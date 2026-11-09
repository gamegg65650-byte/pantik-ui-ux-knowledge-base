# Accessibility

[Start here](../README.md) · [Source register](../08-sources/sources.md)

## A11Y-01 — Text contrast

- **Applies to** — All
- **How to test** — Measure actual text and background pairs. On the web, WCAG AA requires 4.5:1 for regular text and 3:1 for large text of at least 18 pt, or 14 pt bold. Check exceptions in 1.4.3.
- **Suggested fix** — Adjust foreground, background, or backing surface and measure again.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-02 — Non-text contrast

- **Applies to** — All
- **How to test** — On the web, WCAG 1.4.11 generally requires 3:1 against adjacent colors for visual information needed to identify active controls, their states, and meaningful graphics. Check exceptions.
- **Suggested fix** — Strengthen the required border, icon, or other visual cue.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-03 — Meaning beyond color

- **Applies to** — All
- **How to test** — Check that users can recognize errors, selection, and status without relying on color.
- **Suggested fix** — Add text, shape, pattern, or another distinct cue.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-04 — Keyboard operation

- **Applies to** — Web
- **How to test** — Use Tab, Shift+Tab, Enter, Space, arrow keys, and Escape where appropriate. Check order and keyboard traps.
- **Suggested fix** — Use native elements and the expected keyboard pattern.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-05 — Visible focus

- **Applies to** — Web
- **How to test** — Tab through the page. Verify a visible focus indicator and check that sticky headers or banners do not fully obscure focused elements.
- **Suggested fix** — Add a visible focus style and adjust scrolling or overlay placement.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-06 — Target size

- **Applies to** — Web
- **How to test** — Measure pointer targets. WCAG 2.2 AA 2.5.8 specifies 24 by 24 CSS pixels or an applicable exception. Verify the geometry if relying on the spacing exception.
- **Suggested fix** — Increase the target area or separate nearby targets. Document any exception.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-07 — Text resizing and reflow

- **Applies to** — Web
- **How to test** — Test text resizing to 200%. Separately check vertically scrolling content at an equivalent width of 320 CSS pixels, with the exceptions in 1.4.10.
- **Suggested fix** — Allow wrapping and growth. Fix clipping and unnecessary overflow.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-08 — Accessible names and roles

- **Applies to** — Web / Native app
- **How to test** — With a screen reader, check the names, roles, values, and states of key controls.
- **Suggested fix** — Provide programmatic labels and use native semantics or platform accessibility APIs.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/), [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## A11Y-09 — Structure and language

- **Applies to** — Web
- **How to test** — Inspect heading hierarchy, landmarks, page language, and passages in a different language.
- **Suggested fix** — Use semantic markup and appropriate lang attributes.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-10 — Modal dialogs

- **Applies to** — Web / Native app
- **How to test** — Check the dialog name, initial focus, and closing mechanism. On the web, check that focus stays within the modal and returns logically.
- **Suggested fix** — Use the platform dialog pattern and repeat the keyboard and screen-reader checks.
- **Sources** — [APG](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/), [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## A11Y-11 — Images and media alternatives

- **Applies to** — Web / Native app
- **How to test** — Check text alternatives for meaningful images and captions, descriptions, or other media alternatives where applicable.
- **Suggested fix** — Write alternatives that convey the purpose of the image or media.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/), [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## A11Y-12 — Dynamic status messages

- **Applies to** — Web / Native app
- **How to test** — Check whether a screen reader announces errors, confirmations, and updated results at the right time without duplication.
- **Suggested fix** — Associate errors with fields and expose statuses through platform APIs.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/), [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## A11Y-13 — Alternatives to gestures

- **Applies to** — Web / Native app
- **How to test** — Try completing drag or complex gesture actions with a simple pointer action where applicable.
- **Suggested fix** — Provide an accessible alternative, such as Move up and Move down buttons.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-14 — Autoplay and animation

- **Applies to** — Web / Native app
- **How to test** — Review looping media and movement. On the web, WCAG 2.2.2 generally requires a way to pause, stop, or hide nonessential movement that starts automatically, lasts over five seconds, and appears alongside other content.
- **Suggested fix** — Add accessible motion controls and test reduced-motion behavior.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## A11Y-15 — Accessible authentication

- **Applies to** — Web
- **How to test** — Where sign-in exists, test paste and password managers. Check applicable alternatives to cognitive tests under 3.3.8.
- **Suggested fix** — Support paste and autofill. Verify the full sign-in flow and any alternative.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)
