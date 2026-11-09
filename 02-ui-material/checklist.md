# Visual systems and Material 3

[Start here](../README.md) · [Source register](../08-sources/sources.md)

## UI-01 — Color roles

- **Applies to** — All
- **How to test** — Review accent, surface, text, and error roles. For Material 3, check primary/on-primary and surface/on-surface across applicable themes.
- **Suggested fix** — Use semantic color roles and measure contrast.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-02 — Typography

- **Applies to** — All
- **How to test** — Compare headings, body text, labels, line wrapping, and glyph coverage for supported languages.
- **Suggested fix** — Use a consistent type scale and test long copy.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-03 — Grid and spacing

- **Applies to** — All
- **How to test** — Check alignment, visual rhythm, and spacing between related and unrelated elements.
- **Suggested fix** — Use consistent grid and spacing values.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-04 — Component choice

- **Applies to** — All
- **How to test** — Check that buttons, links, switches, tabs, and dialogs match their purpose. For Material 3, compare with the component catalog.
- **Suggested fix** — Choose the matching component and behavior. On the web, links navigate and buttons perform actions.
- **Sources** — [CMP](https://m3.material.io/components)

## UI-05 — Component states

- **Applies to** — All
- **How to test** — Review applicable default, focus, hover, pressed, selected, disabled, error, and loading states.
- **Suggested fix** — Define the variants and their triggers. Make states distinguishable beyond color where needed.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-06 — Themes and surfaces

- **Applies to** — All
- **How to test** — Check text over images, dialogs, overlays, and selected states in every supported theme.
- **Suggested fix** — Use appropriate theme tokens and stable backing surfaces for text.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-07 — Icons

- **Applies to** — All
- **How to test** — Check meaning, size, and alignment. Verify accessible names for interactive icons on the working build.
- **Suggested fix** — Label ambiguous icons and measure the hit area separately from the artwork.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-08 — Responsive layout

- **Applies to** — All
- **How to test** — Check narrow, wide, and intermediate sizes with long strings.
- **Suggested fix** — Allow wrapping and layout changes. Remove dimensions that clip content.
- **Sources** — [M3](https://m3.material.io/foundations/)

## UI-09 — Motion

- **Applies to** — All
- **How to test** — Check whether transitions help explain changes. On the build, test the system reduced-motion setting.
- **Suggested fix** — Provide a reduced or static version where appropriate.
- **Sources** — [M3](https://m3.material.io/foundations/)
