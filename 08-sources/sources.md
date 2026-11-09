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

## Release-readiness references

| Code | Source |
| --- | --- |
| FOCUS | [W3C Focus Not Obscured](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum) |
| HIST | [MDN History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API/Working_with_the_History_API) |
| OG | [Open Graph protocol](https://ogp.me/) |
| HTTP404 | [Google Search crawling errors](https://developers.google.com/search/docs/crawling-indexing/troubleshoot-crawling-errors) |
| LOCALE | [Google localized pages](https://developers.google.com/search/docs/specialty/international/localized-versions) |
| CANON | [Google canonical URLs](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls) |
| IMG | [web.dev responsive images](https://web.dev/learn/images/descriptive) |
| LCP | [web.dev LCP optimization](https://web.dev/articles/optimize-lcp) |
| CLIP | [MDN Clipboard.writeText()](https://developer.mozilla.org/en-US/docs/Web/API/Clipboard/writeText) |
| CAR | [WAI-ARIA carousel pattern](https://www.w3.org/WAI/ARIA/apg/patterns/carousel/) |
| MOT | [MDN prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-reduced-motion) |
| STATE | [Android Compose state saving](https://developer.android.com/develop/ui/compose/state-saving) |
| LIST | [Android adaptive list-detail layout](https://developer.android.com/develop/adaptive-apps/guides/list-detail) |
| ALINK | [Android verified App Links](https://developer.android.com/training/app-links/verify-applinks) |
| ULINK | [Apple universal links](https://developer.apple.com/documentation/xcode/supporting-universal-links-in-your-app) |
| XCA | [Apple accessibility audits](https://developer.apple.com/documentation/accessibility/performing-accessibility-audits-for-your-app) |
| FMODE | [Figma modes for variables](https://help.figma.com/hc/en-us/articles/15343816063383-Modes-for-variables) |
| FDEV | [Figma Dev Mode guide](https://help.figma.com/hc/en-us/articles/15023124644247-Guide-to-Dev-Mode-in-Figma) |
| FSTATUS | [Figma Dev Mode statuses](https://help.figma.com/hc/en-us/articles/26781702258583-Dev-Mode-statuses-and-notifications) |
| FFLOW | [Figma prototype flows](https://help.figma.com/hc/en-us/articles/360039823894-Create-and-manage-prototype-flows) |
| FPM | [Figma variable modes in prototypes](https://help.figma.com/hc/en-us/articles/15253268379799-Variable-modes-in-prototypes) |
