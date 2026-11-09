# Source register

Sources were reviewed on November 9, 2026 for the original checklist. Check the applicable criteria and library status before a new release.

| Code | Source | Use |
| --- | --- | --- |
| GD | [Google Design](https://design.google/?home=) | Design research, practical examples, and perspectives. |
| M3 | [Material Design 3](https://m3.material.io/foundations/) | Foundations, color roles, typography, layout, tokens, and interaction states. |
| CMP | [Material 3 Components](https://m3.material.io/components) | Component purpose, anatomy, states, and behavior. |
| WC | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) | Web accessibility criteria, thresholds, and exceptions. |
| WAI | [W3C WAI Easy Checks](https://www.w3.org/WAI/test-evaluate/preliminary/) | Introductory accessibility checks and their limits. |
| APG | [WAI-ARIA APG Modal Dialog](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/) | Keyboard and focus patterns for web dialogs. |
| WV | [web.dev Web Vitals](https://web.dev/articles/vitals) | Field and lab measurements, including LCP, INP, and CLS. |
| AND | [Android Developers Compose accessibility](https://developer.android.com/develop/ui/compose/accessibility/api-defaults) | Touch targets and platform semantics. |
| ADP | [Android Developers window size classes](https://developer.android.com/develop/adaptive-apps/guides/use-window-size-classes) | Adaptive Android layouts. |
| IOS | [Apple HIG Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) | Control sizes, text scaling, and accessible interactions. |
| FG | [Figma Learn](https://help.figma.com/) | Components, variables, Auto Layout, and prototyping. |

## Material Components on GitHub

- [Material Components organization](https://github.com/material-components) lists platform implementations. Check each repository's README, archive status, and releases.
- [Material Web](https://github.com/material-components/material-web/blob/main/README.md) reported maintenance mode pending new maintainers at the review date.
- [Material Components for Android Views](https://github.com/material-components/material-components-android) reported maintenance mode. See [Material 3 in Jetpack Compose](https://developer.android.com/develop/ui/compose/designsystems/material3) for Google's Compose guidance.
- [Material Components for iOS](https://github.com/material-components/material-components-ios) was archived at the review date. Consult Apple HIG for iOS platform patterns.

Additional references include the [Material 3 overview](https://m3.material.io/) and [Figma component properties](https://help.figma.com/hc/en-us/articles/5579474826519-Explore-component-properties).

## Material implementation references

Use the component documentation for the dependency version in the audited build. The checks describe observable behavior. Each platform may expose a different implementation API.

| Code | Source |
| --- | --- |
| MW | [Material Web Quick Start](https://material-web.dev/about/quick-start/) |
| MWT | [Material Web Theming](https://material-web.dev/theming/material-theming/) |
| MWF | [Material Web Text Field](https://material-web.dev/components/text-field/) |
| MWS | [Material Web Select](https://material-web.dev/components/select/) |
| MWD | [Material Web Dialog](https://material-web.dev/components/dialog/) |
| MWB | [Material Web Buttons](https://material-web.dev/components/button/) |
| MWI | [Material Web Icon Buttons](https://material-web.dev/components/icon-button/) |
| MWR | [Material Web repository](https://github.com/material-components/material-web) |
| MDA | [MDC Android getting started](https://github.com/material-components/material-components-android/blob/master/docs/getting-started.md) |
| MDAF | [MDC Android Text Field](https://github.com/material-components/material-components-android/blob/master/docs/components/TextField.md) |
| MDAS | [MDC Android Bottom Sheet](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomSheet.md) |
| C3 | [Material 3 in Compose](https://developer.android.com/develop/ui/compose/designsystems/material3) |
| CIN | [Compose window insets](https://developer.android.com/develop/ui/compose/system/insets) |
| CAT | [Compose accessibility testing](https://developer.android.com/develop/ui/compose/accessibility/testing) |
| MDI | [MDC iOS repository](https://github.com/material-components/material-components-ios) |
| MDIF | [MDC iOS Text Controls](https://github.com/material-components/material-components-ios/blob/develop/components/TextControls/README.md) |
| MDIT | [MDC iOS Typography](https://github.com/material-components/material-components-ios/blob/develop/components/Typography/README.md) |
| IA | [Apple accessibility modifiers](https://developer.apple.com/documentation/swiftui/view-accessibility) |
| IT | [Apple Dynamic Type and custom fonts](https://developer.apple.com/documentation/swiftui/applying-custom-fonts-to-text) |
| IIN | [Apple Accessibility Inspector](https://developer.apple.com/documentation/accessibility/accessibility-inspector) |
| IRM | [Apple accessibilityReduceMotion](https://developer.apple.com/documentation/swiftui/environmentvalues/accessibilityreducemotion) |
