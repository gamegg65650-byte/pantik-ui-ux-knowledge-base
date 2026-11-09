# Figma release and handoff checks

[Start here](../README.md) · [Release test matrix](../07-report/release-matrix.md) · [Source register](../08-sources/sources.md)

Run applicable checks against the release candidate or the approved design. Record the environment and keep the evidence with the audit report.

## REL-FIG-01 — Token mapping from design to build

- **How to test** — Pick representative semantic tokens and compare the Figma variable and mode with the implemented token name and value in the same theme. Repeat on a nested component.
- **Suggested fix** — Document the design-to-code mapping and resolve conflicting aliases or overrides.
- **Sources** — [FMODE](https://help.figma.com/hc/en-us/articles/15343816063383-Modes-for-variables), [FDEV](https://help.figma.com/hc/en-us/articles/15023124644247-Guide-to-Dev-Mode-in-Figma)

## REL-FIG-02 — Approved design and change tracking

- **How to test** — Open the handoff as a developer. Find the approved frame, its linked assets, and changes since the previous delivery. Where Dev Mode is available, check the relevant ready-for-dev status and changed frames.
- **Suggested fix** — Use a single approved entry point, visible revision notes, and the applicable handoff status.
- **Sources** — [FDEV](https://help.figma.com/hc/en-us/articles/15023124644247-Guide-to-Dev-Mode-in-Figma), [FSTATUS](https://help.figma.com/hc/en-us/articles/26781702258583-Dev-Mode-statuses-and-notifications)

## REL-FIG-03 — Interaction details for a custom component

- **How to test** — Ask a reviewer to implement a custom control from the handoff alone. Check whether states, focus order, accessible name, keyboard actions, and failure behavior are specified for the target platform.
- **Suggested fix** — Add missing interaction details to the approved component and link the testable prototype state.
- **Sources** — [FDEV](https://help.figma.com/hc/en-us/articles/15023124644247-Guide-to-Dev-Mode-in-Figma), [WC](https://www.w3.org/TR/WCAG22/)

## REL-FIG-04 — Prototype starts from a clean state

- **How to test** — Open each shared flow in a fresh viewer session. Verify the starting frame, default variable mode, branch behavior, and expected reset or restart. Repeat in a different flow.
- **Suggested fix** — Set explicit flow starts, confirm shared links, and reset or initialize prototype variables where the experience requires it.
- **Sources** — [FFLOW](https://help.figma.com/hc/en-us/articles/360039823894-Create-and-manage-prototype-flows), [FPM](https://help.figma.com/hc/en-us/articles/15253268379799-Variable-modes-in-prototypes)
