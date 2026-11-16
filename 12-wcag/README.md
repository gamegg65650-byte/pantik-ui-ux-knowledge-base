# WCAG 2.2 for PANTIK audits

[Knowledge map](../KNOWLEDGE-MAP.md) · [All criteria](criteria.md) · [Audit spreadsheet CSV](WCAG-2.2-Audit.csv) · [W3C sources](sources.md)

## Versions and conformance

- WCAG 2.2 is a W3C Recommendation. The [dated December 2024 publication](https://www.w3.org/TR/2024/REC-WCAG22-20241212/) identifies the edition for reproducible audit reports.
- Levels build on each other. Level A covers 31 active criteria. AA adds 24 and AAA adds 31. Check each applicable requirement across full pages and complete processes, including alternate states and technologies relied upon.
- WCAG 2.2 adds nine criteria to 2.1. Criterion 4.1.1 Parsing is recorded as removed in 2.2. Refer to the applicable Recommendation when an audit specifies an older edition.
- W3C publishes Understanding, Techniques and ACT rules as implementation and evaluation aids. Match each technique or rule to its applicability and test environment. Supplemental guidance covers needs beyond the Recommendation.
- For native apps and documents, use [WCAG2ICT](https://www.w3.org/TR/wcag2ict/) with the applicable platform requirements. For web design in Figma, document intent and verify semantics, keyboard behavior, scaling and announcements in the implementation. The [WCAG 3 introduction](https://www.w3.org/WAI/standards-guidelines/wcag/wcag3-intro/) tracks the draft.

## Audit a website

1. Record the version, target level, routes, locales, devices, templates, third-party widgets and complete processes. Include steps that appear only after an action or error.
2. Copy [the audit CSV](WCAG-2.2-Audit.csv). In Excel, import the file as UTF-8 with a comma delimiter and keep criterion IDs as text. Use A and AA for the AA baseline and review all applicability decisions.
3. Use an automated scanner to identify candidates. Then test keyboard interaction, accessibility tree output, screen reader behavior, zoom and reflow, contrast, pointer interactions, media alternatives and forms manually.
4. Record one result per criterion and evaluated page or state. Use Pass, Fail, Not applicable or Not tested. Record the observed behavior, evidence and exception where relevant.
5. Link duplicate observations across checklist criteria with a common finding ID. Capture the problem and fix in the [report template](../07-report/audit-report.md), then retest in the same environment.
6. Review [W3C conformance requirements](https://www.w3.org/TR/WCAG22/#conformance) before making a conformance claim. A scope implied by one path, a design mockup or one automated scan leaves conditions unverified.

## What WCAG 2.2 adds

| Criterion | Level | Where to test |
| --- | --- | --- |
| [2.4.11 Focus Not Obscured (Minimum)](https://www.w3.org/TR/WCAG22/#focus-not-obscured-minimum) | AA | Sticky navigation, cookie banners and overlays during tabbing. |
| [2.4.12 Focus Not Obscured (Enhanced)](https://www.w3.org/TR/WCAG22/#focus-not-obscured-enhanced) | AAA | Any partial obstruction of the focused component. |
| [2.4.13 Focus Appearance](https://www.w3.org/TR/WCAG22/#focus-appearance) | AAA | Focus indicator area and state-change contrast. |
| [2.5.7 Dragging Movements](https://www.w3.org/TR/WCAG22/#dragging-movements) | AA | Sliders, kanban, sorting, maps and drag interactions. |
| [2.5.8 Target Size (Minimum)](https://www.w3.org/TR/WCAG22/#target-size-minimum) | AA | Icon controls, close buttons, pagination and dense lists. |
| [3.2.6 Consistent Help](https://www.w3.org/TR/WCAG22/#consistent-help) | A | Repeated contact and help affordances across related pages. |
| [3.3.7 Redundant Entry](https://www.w3.org/TR/WCAG22/#redundant-entry) | A | Repeated contact or address input in one flow. |
| [3.3.8 Accessible Authentication (Minimum)](https://www.w3.org/TR/WCAG22/#accessible-authentication-minimum) | AA | Sign-in, multi-factor authentication and account recovery. |
| [3.3.9 Accessible Authentication (Enhanced)](https://www.w3.org/TR/WCAG22/#accessible-authentication-enhanced) | AAA | Authentication steps with cognitive tests including recognition. |

## Existing PANTIK checks

| Existing check | Related WCAG criteria |
| --- | --- |
| A11Y-01, A11Y-02, A11Y-03 | 1.4.3, 1.4.11, 1.4.1 |
| A11Y-04 | 2.1.1, 2.1.2, 2.4.3 |
| A11Y-05, A11Y-06 | 2.4.7, 2.4.11, 2.5.8 |
| A11Y-07 | 1.4.4, 1.4.10 |
| A11Y-08, A11Y-09 | 4.1.2, 1.3.1, 2.4.1, 3.1.1, 3.1.2 |
| A11Y-10 | 2.1.1, 2.1.2, 2.4.3, 4.1.2 |
| A11Y-11 | 1.1.1 and applicable 1.2 criteria |
| A11Y-12, A11Y-13 | 4.1.3, 2.5.1, 2.5.7 |
| A11Y-14, A11Y-15 | 1.4.2, 2.2.2, 2.3.3, 3.3.8 |
| REL-A11Y-01, REL-A11Y-02 | 2.2.2, 2.3.3 |

The associations connect project checks to related requirements. Design and release checks may also include platform conventions and guidance from [WAI-ARIA APG](https://www.w3.org/WAI/ARIA/apg/).

For a portfolio, start with the home page, a project case study and the contact flow. Repeat with the RU, EN and PL interfaces. Include the keyboard behavior of the language switcher, navigation and media, plus any sticky element that can cover focus.
