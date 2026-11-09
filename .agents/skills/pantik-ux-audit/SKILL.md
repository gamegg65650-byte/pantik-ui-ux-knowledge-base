---
name: pantik-ux-audit
description: Audit a live website, native app, or Figma design with the PANTIK UI/UX Knowledge Base. Use for evidence-based UX reviews, accessibility checks, persona journeys, or release audits that need screenshots, a complete checklist matrix, severity-ranked findings, and verifiable fixes.
---

# PANTIK UX Audit

## Inputs and scope

- Require a target URL, build, design, or supplied screenshots. Infer the platform and an explicit primary user goal if the request omits them.
- Use the requested report language. Treat an invented persona as a scenario assumption, and distinguish expert walkthroughs from participant research.
- Resolve the checklist from the containing repository or the [canonical knowledge base](https://github.com/gamegg65650-byte/pantik-ui-ux-knowledge-base). Read the actual `Audit-Checklist.csv`, `07-report/audit-report.md`, `07-report/release-matrix.md`, and relevant topic pages. Record the repository revision when available. If the checklist cannot be opened, report the blocker instead of inventing its IDs or requirements.
- Keep every checklist ID in the coverage matrix. Select All, the matching platform, and shared platform rows. Apply MAT checks only to the verified installed implementation, and REL checks to the relevant release conditions. If a dependency or condition cannot be determined, mark that check Not tested. Give a reason for each out-of-scope row.

## Capture and test

1. Record date, target, visible build identifier if available, browser or device, viewport, input method, locale, and assumptions. Define the primary task, expected outcome, and route through representative screens.
2. Observe the real product. Capture a named screenshot at each important step and preserve the state shown. Use relevant empty, error, success, and recovery states. For a site, sample mobile and desktop widths and check history, direct links, focus, forms, and contact handoff. Use test data and stop before sending or submitting to an external recipient unless the user authorizes it.
3. Execute each applicable row using its test method. Pair screenshots with measurements, accessibility tree observations, keyboard interaction, or runtime evidence where needed. Check browser width and text zoom separately. Distinguish an accessibility tree from screen-reader output, a visible error page from its HTTP status, and lab timing from field Web Vitals.
4. Mark each row Pass, Fail, Not applicable, or Not tested. A partial result is Not tested with the observed subset and remaining conditions, unless the available evidence already establishes a failure. Record every confirmed failure against the original criterion and source. Keep hypotheses separate.
5. Check coverage before delivery. Every checklist ID occurs exactly once in the matrix. Every finding points to at least one row and concrete evidence. Every route step has a screenshot or a named capture blocker.

## Deliver

- Provide the persona, goal, environment, numbered route, annotated screenshots or screenshot references, and results matrix. For artifact requests, produce the requested format if available and verify the rendered result.
- For each distinct finding include linked IDs, severity, screen and viewport, reproduction, actual and expected behavior, proof, proposed fix, and a retest condition. Use the repository report scale: P0 blocks the main task with no workaround, P1 seriously disrupts a key task, P2 adds meaningful friction, P3 is minor. Explain the selected severity in terms of the observed user impact.
- Summarize the top three fixes, coverage counts, and outstanding checks. Describe results as scoped to the observed environments. Avoid claiming WCAG conformance from a sampled walkthrough.
- Keep the audit read-only unless the user explicitly requests changes, publication, or issue creation.
