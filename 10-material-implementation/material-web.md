# Material Web

[Start here](../README.md) · [Source register](../08-sources/sources.md)

Use for projects that depend on @material/web. The upstream README identifies the library as being in maintenance mode. On other stacks, reuse the test scenarios where relevant and apply that stack's APIs.

Record the component library version and the screen or route you tested. Mark checks for a different platform, library, or migration stage **Not applicable**.

## MAT-WEB-01 — Installed version and component registration

- **How to test** — For projects using @material/web, load the production build in supported browsers. Check that every required md-* element upgrades before its first use, including deep links and routes with lazy-loaded components.
- **Suggested fix** — Pin and record the version. Import the required components at the appropriate entry point and add a smoke test for the built page.
- **Sources** — [MW](https://material-web.dev/about/quick-start/), [MWR](https://github.com/material-components/material-web)

## MAT-WEB-02 — System and component token overrides

- **How to test** — Verify a shared system token and a component-specific override in light and dark themes. Check the rendered states after changing the theme, including overlays and components in separately styled containers.
- **Suggested fix** — Use documented CSS custom properties and ensure the theme scope reaches every component instance.
- **Sources** — [MWT](https://material-web.dev/theming/material-theming/)

## MAT-WEB-03 — Form submission and reset

- **How to test** — In a real form, exercise md-text-field and md-select with valid and invalid values. Inspect submitted entries, including names, selected values, and disabled fields. Reset and confirm the expected initial state returns.
- **Suggested fix** — Set names and defaults, use the component's form integration, and add a regression test for submission and reset.
- **Sources** — [MWF](https://material-web.dev/components/text-field/), [MWS](https://material-web.dev/components/select/)

## MAT-WEB-04 — Native and custom validity

- **How to test** — Trigger a missing required value, then a custom application error, then correct the value. Verify the message, submission behavior, and error clearing. An error style alone does not prove that the form blocks submission.
- **Suggested fix** — Use the validity APIs for constraints that must prevent submission. Keep visual error state and error copy synchronized with validity.
- **Sources** — [MWF](https://material-web.dev/components/text-field/), [MWS](https://material-web.dev/components/select/)

## MAT-WEB-05 — Dialog outcomes and cancellation

- **How to test** — Open an md-dialog and test its confirm and cancel actions, Escape, and scrim dismissal where enabled. Reopen after each exit and check which action or value the application handles.
- **Suggested fix** — Assign explicit action values and handle cancel and close separately as needed. Only run the business action for an explicit confirmation.
- **Sources** — [MWD](https://material-web.dev/components/dialog/), [APG](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/)

## MAT-WEB-06 — Icon toggle state

- **How to test** — Verify icon-only names and that a Material Web toggle's selected state and its exposed pressed state follow the real application value, including after a reset or failed update.
- **Suggested fix** — Bind state to the same application value, use the documented accessible labeling options, and test both states with assistive technology.
- **Sources** — [MWI](https://material-web.dev/components/icon-button/)

## MAT-WEB-07 — Button form behavior

- **How to test** — Place a primary action and a secondary action inside the same form. Test clicking each, Enter in a field, and any action located outside the form that targets it by ID.
- **Suggested fix** — Use explicit button types and form association where needed. Keep secondary actions from submitting accidentally.
- **Sources** — [MWB](https://material-web.dev/components/button/), [MWD](https://material-web.dev/components/dialog/)

## MAT-WEB-08 — Custom element focus and disabled state

- **How to test** — On an md-* button, field, or select, check keyboard focus and disabled behavior in the real page after applying framework bindings and theme overrides. Verify that a disabled action cannot execute.
- **Suggested fix** — Use component properties and supported CSS tokens, then retest with keyboard and pointer. Avoid styling assumptions about private shadow DOM.
- **Sources** — [MWT](https://material-web.dev/theming/material-theming/), [MWB](https://material-web.dev/components/button/), [MWF](https://material-web.dev/components/text-field/), [MWS](https://material-web.dev/components/select/)
