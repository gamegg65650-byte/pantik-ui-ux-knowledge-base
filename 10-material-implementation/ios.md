# Material Components on iOS

[Start here](../README.md) · [Source register](../08-sources/sources.md)

Use the MDC iOS checks for existing dependencies or migration builds. The repository is archived. For current iOS development, use platform guidance and run the relevant native app checks.

Record the component library version and the screen or route you tested. Mark checks for a different platform, library, or migration stage **Not applicable**.

## MAT-IOS-01 — Archived dependency inventory

- **How to test** — Identify the Material iOS components still in the app and record their exact versions, ownership, and flows. Verify a representative flow on supported iOS versions.
- **Suggested fix** — Keep a regression list for existing MDC iOS screens and plan replacements using SwiftUI or UIKit where appropriate.
- **Sources** — [MDI](https://github.com/material-components/material-components-ios), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## MAT-IOS-02 — MDC text-field announcements

- **How to test** — With VoiceOver, move to a legacy Material text field before input, after input, and after validation fails. Listen for the floating label, value, and assistive or error text. Repeat for any custom label override.
- **Suggested fix** — Preserve the necessary label, value, and error information without repetition. Verify any explicit accessibility label with VoiceOver.
- **Sources** — [MDIF](https://github.com/material-components/material-components-ios/blob/develop/components/TextControls/README.md), [IA](https://developer.apple.com/documentation/swiftui/view-accessibility)

## MAT-IOS-03 — MDC text-control sizing

- **How to test** — In legacy filled or outlined text fields and text areas, test long floating and assistive labels at large text sizes. Check the actual Auto Layout or manual sizing behavior.
- **Suggested fix** — Allow the field to use its intrinsic or measured height, and remove fixed heights that clip labels or errors.
- **Sources** — [MDIF](https://github.com/material-components/material-components-ios/blob/develop/components/TextControls/README.md)

## MAT-IOS-04 — Legacy typography and Dynamic Type

- **How to test** — Test legacy Material typography or custom fonts at standard and accessibility text sizes. Check headings, labels, buttons, and error text for correct scaling.
- **Suggested fix** — Use Dynamic Type-aware typography. In SwiftUI, choose the appropriate relative text style and scale layout values where needed.
- **Sources** — [MDIT](https://github.com/material-components/material-components-ios/blob/develop/components/Typography/README.md), [IT](https://developer.apple.com/documentation/swiftui/applying-custom-fonts-to-text), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## MAT-IOS-05 — Accessibility parity after component replacement

- **How to test** — Replace or test a mapped native control in a migration build. Compare VoiceOver labels, traits, values, and actions with the intended behavior, and inspect the resulting element tree.
- **Suggested fix** — Prefer native control semantics. Add labels, values, or traits only where needed and verify with Accessibility Inspector and VoiceOver.
- **Sources** — [MDI](https://github.com/material-components/material-components-ios), [IA](https://developer.apple.com/documentation/swiftui/view-accessibility), [IIN](https://developer.apple.com/documentation/accessibility/accessibility-inspector)

## MAT-IOS-06 — Motion parity after migration

- **How to test** — With system Reduce Motion enabled, run the original and replacement transitions for a legacy Material flow. Check that completion and state remain understandable.
- **Suggested fix** — Use a reduced transition, such as a simple fade where appropriate, and honor the system preference through the platform APIs.
- **Sources** — [MDI](https://github.com/material-components/material-components-ios), [IRM](https://developer.apple.com/documentation/swiftui/environmentvalues/accessibilityreducemotion), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)
