# Material on Android

[Start here](../README.md) · [Source register](../08-sources/sources.md)

Use MDC Android checks for existing XML Views, and Compose checks for screens that use Jetpack Compose. Google lists MDC Android Views in maintenance mode and directs new Material development toward Compose.

Record the component library version and the screen or route you tested. Mark checks for a different platform, library, or migration stage **Not applicable**.

## MAT-AND-01 — Identify Views or Compose

- **How to test** — Inventory the Material dependencies and note which audited screens are XML Views, Compose, or mixed. Run a representative screen from each in the supported build.
- **Suggested fix** — Record the exact versions and use the matching theme and component docs. Treat MDC Android Views as a maintained legacy stack and follow the Compose-first guidance for new Material work.
- **Sources** — [MDA](https://github.com/material-components/material-components-android/blob/master/docs/getting-started.md), [C3](https://developer.android.com/develop/ui/compose/designsystems/material3)

## MAT-AND-02 — Views theme inheritance and overlays

- **How to test** — On a Views screen, compare the base activity theme with the component theme and any dialog or sheet overlays. Switch light and dark mode and inspect the same field or button.
- **Suggested fix** — Use compatible Material theme parents and documented widget styles or overlays. Test inside the actual screen and dialog context.
- **Sources** — [MDA](https://github.com/material-components/material-components-android/blob/master/docs/getting-started.md), [MDAF](https://github.com/material-components/material-components-android/blob/master/docs/components/TextField.md), [MDAS](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomSheet.md)

## MAT-AND-03 — TextInputLayout ownership and error lifecycle

- **How to test** — For an MDC Android Views field, verify where the hint is set. Trigger and clear an error, change any end-icon state, and check the result with TalkBack.
- **Suggested fix** — Set the hint on TextInputLayout, keep helper and error text in sync, and verify the end icon has a meaningful accessible description.
- **Sources** — [MDAF](https://github.com/material-components/material-components-android/blob/master/docs/components/TextField.md)

## MAT-AND-04 — Bottom-sheet expansion and dismissal

- **How to test** — Test a legacy MDC bottom sheet in its supported collapsed and expanded states. If it uses BottomSheetDragHandleView, verify the accessibility actions and dismissal without requiring a drag gesture.
- **Suggested fix** — Use the documented drag handle or another accessible control and provide a clear dismissal path where appropriate.
- **Sources** — [MDAS](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomSheet.md)

## MAT-AND-05 — Sheet and keyboard insets

- **How to test** — In the real bottom sheet or Compose screen, open the IME and scroll to the last action. Repeat with gesture navigation and verify status-bar and navigation-bar areas.
- **Suggested fix** — Use the appropriate edge-to-edge and inset APIs. Check for double padding and controls hidden by system UI.
- **Sources** — [MDAS](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomSheet.md), [CIN](https://developer.android.com/develop/ui/compose/system/insets)

## MAT-AND-06 — Dynamic color and fallback theme

- **How to test** — When dynamic color is supported by the app, run it with different system palettes and compare it with the app fallback on an unsupported or disabled configuration. Check meaningful color pairs in both themes.
- **Suggested fix** — Provide explicit light and dark fallback schemes and use paired color roles for content and surfaces.
- **Sources** — [C3](https://developer.android.com/develop/ui/compose/designsystems/material3)

## MAT-AND-07 — Compose semantics on custom controls

- **How to test** — Inspect the semantics of a custom composable with an icon, text, and a state. Use TalkBack to check whether it exposes one coherent control and the intended action and state.
- **Suggested fix** — Use Material composables or appropriate Compose semantics. Merge only where the child content belongs to one control.
- **Sources** — [CAT](https://developer.android.com/develop/ui/compose/accessibility/testing), [C3](https://developer.android.com/develop/ui/compose/designsystems/material3)

## MAT-AND-08 — Compose accessibility regression checks

- **How to test** — On a Compose build, run automated accessibility checks on a representative user journey and verify that the relevant actions actually trigger checks. Repeat key states with TalkBack.
- **Suggested fix** — Enable supported Compose accessibility testing in the instrumented test suite and keep a manual device pass.
- **Sources** — [CAT](https://developer.android.com/develop/ui/compose/accessibility/testing)
