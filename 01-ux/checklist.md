# User journeys and clarity

[Start here](../README.md) · [Source register](../08-sources/sources.md)

## UX-01 — Primary user journey

- **Applies to** — All
- **How to test** — Ask someone to complete the main task without hints. Record the first wrong click and where they stop.
- **Suggested fix** — Clarify the main action, label, or step order.
- **Sources** — [GD](https://design.google/?home=)

## UX-02 — Navigation and return

- **Applies to** — All
- **How to test** — Move forward and back. Check the current section and whether input, filters, and scroll position return when expected.
- **Suggested fix** — Mark the active section and preserve relevant context.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UX-03 — Action hierarchy

- **Applies to** — All
- **How to test** — Identify the heading, primary action, and secondary actions on every key screen.
- **Suggested fix** — Reduce competing emphasis and label the primary action clearly.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UX-04 — Screen states

- **Applies to** — All
- **How to test** — Check loading, empty, error, offline, and success states where applicable. Locate the corresponding frames in a design file.
- **Suggested fix** — Explain the state and show the next step or retry action.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UX-05 — Fields and errors

- **Applies to** — All
- **How to test** — Try empty, invalid, and valid input. Check whether the user can tell which field needs attention and how to correct it.
- **Suggested fix** — Use persistent labels and nearby error text. Associate each message with its field in the implementation.
- **Sources** — [WC](https://www.w3.org/TR/WCAG22/)

## UX-06 — Deletion and data loss

- **Applies to** — All
- **How to test** — Check deletion, cancellation, and leaving with unsaved changes where applicable.
- **Suggested fix** — Offer undo for reversible actions. Explain consequences before irreversible actions.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UX-07 — Interface copy

- **Applies to** — All
- **How to test** — Check that the same actions use consistent terms and messages explain the next step.
- **Suggested fix** — Replace vague labels with specific verbs, such as Retry upload.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UX-08 — Localization

- **Applies to** — All
- **How to test** — Run the journey in all supported languages. Check long strings and date, number, and price formats.
- **Suggested fix** — Allow wrapping and flexible height. Use locale-aware formats.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UX-09 — Repeated submission

- **Applies to** — Web / Native app
- **How to test** — On a slow connection, activate Submit several times. Check the result and retry after a timeout in a safe test environment.
- **Suggested fix** — Show submission progress and prevent duplicates at the appropriate layer.
- **Sources** — [GD](https://design.google/?home=)

## UX-10 — Outcome and next step

- **Applies to** — All
- **How to test** — After the task, check that users can tell what happened and what they can do next.
- **Suggested fix** — Show a confirmation, useful reference, or way to continue.
- **Sources** — [GD](https://design.google/?home=)
