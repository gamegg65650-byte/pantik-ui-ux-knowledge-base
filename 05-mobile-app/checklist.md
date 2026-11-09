# Native apps

[Start here](../README.md) · [Source register](../08-sources/sources.md)

## APP-01 — Touch targets

- **Applies to** — Native app
- **How to test** — Measure actual hit areas. Android recommends at least 48 by 48 dp. Apple HIG lists 44 by 44 pt as the default control size for iOS and iPadOS.
- **Suggested fix** — Increase hit areas and check that neighboring targets do not overlap.
- **Sources** — [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## APP-02 — Window adaptation

- **Applies to** — Native app
- **How to test** — Check phones, wider windows, orientation, and multitasking where supported.
- **Suggested fix** — Adapt layout to the current window size while preserving context. On Android, use window size classes.
- **Sources** — [ADP](https://developer.android.com/develop/adaptive-apps/guides/use-window-size-classes)

## APP-03 — Larger system text

- **Applies to** — Native app
- **How to test** — Enable larger text on Android or Dynamic Type on iOS. Check menus, forms, and dialogs.
- **Suggested fix** — Allow wrapping, container growth, and scrolling.
- **Sources** — [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## APP-04 — TalkBack and VoiceOver

- **Applies to** — Native app
- **How to test** — Complete the key journey with the platform screen reader. Check reading order, names, and state announcements.
- **Suggested fix** — Improve labels, groups, and traversal order. Retest on a device.
- **Sources** — [AND](https://developer.android.com/develop/ui/compose/accessibility/api-defaults), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## APP-05 — System insets and keyboard

- **Applies to** — Native app
- **How to test** — Check system Back, safe areas or insets, and whether the last field and submit button remain usable when the keyboard opens.
- **Suggested fix** — Account for system insets and allow the form to scroll.
- **Sources** — [ADP](https://developer.android.com/develop/adaptive-apps/guides/use-window-size-classes), [IOS](https://developer.apple.com/design/human-interface-guidelines/accessibility)

## APP-06 — Denied permissions and offline use

- **Applies to** — Native app
- **How to test** — Deny a relevant permission, then test with the network off separately. Check how the user continues or retries.
- **Suggested fix** — Request permissions in context and explain how to proceed after refusal.
- **Sources** — [GD](https://design.google/?home=)

## APP-07 — Return to the app

- **Applies to** — Native app
- **How to test** — Background the app partway through the journey, then reopen it. Check state restoration and completed actions.
- **Suggested fix** — Restore relevant state and prevent duplicate actions.
- **Sources** — [ADP](https://developer.android.com/develop/adaptive-apps/guides/use-window-size-classes)
