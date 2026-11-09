# Native app release checks

[Start here](../README.md) · [Release test matrix](../07-report/release-matrix.md) · [Source register](../08-sources/sources.md)

Run applicable checks against the release candidate or the approved design. Record the environment and keep the evidence with the audit report.

## REL-APP-01 — Recreation and interrupted drafts

- **How to test** — On Android, interrupt the journey and reproduce activity or process recreation in a test build. Verify the selected item, position, or safe-to-restore draft and check that completed actions do not repeat.
- **Suggested fix** — Save minimal restorable UI state and reload durable data from its owner. Combine local state tests with an app-level recreation test.
- **Sources** — [STATE](https://developer.android.com/develop/ui/compose/state-saving)

## REL-APP-02 — List-detail continuity across pane changes

- **How to test** — On a screen with adaptive list-detail navigation, select an item and resize the app between single and dual panes. Check the selected item and Back behavior at each size.
- **Suggested fix** — Keep selection and navigation state consistent across pane changes. Define what Back should do in each layout.
- **Sources** — [LIST](https://developer.android.com/develop/adaptive-apps/guides/list-detail)

## REL-APP-03 — Verified deep links and web fallback

- **How to test** — For a feature with Android App Links or iOS universal links, open a documented URL with the app installed and again without it. Test the intended detail screen and a safe fallback for invalid or unauthorized destinations.
- **Suggested fix** — Validate app and domain association. Route supported links to the intended screen and keep a usable browser destination.
- **Sources** — [ALINK](https://developer.android.com/training/app-links/verify-applinks), [ULINK](https://developer.apple.com/documentation/xcode/supporting-universal-links-in-your-app)

## REL-APP-04 — iOS accessibility audit in UI tests

- **How to test** — In an iOS UI test on a supported test target, run the accessibility audit after navigating to key states such as form errors and modal screens. Confirm and triage findings and repeat the important flows with VoiceOver.
- **Suggested fix** — Add screen-specific audit steps and document any narrowly scoped exceptions. Keep manual device testing.
- **Sources** — [XCA](https://developer.apple.com/documentation/accessibility/performing-accessibility-audits-for-your-app)
