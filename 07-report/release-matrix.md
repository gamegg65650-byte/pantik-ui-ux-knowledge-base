# Release test matrix

Copy this page into a project audit. Start with the most important user journey, then add supported combinations that could change the outcome. An untested combination stays **Not tested**.

- **Project, build, and date** —
- **Critical journey and expected outcome** —
- **Supported browsers, OS versions, devices, and languages** —
- **Relevant Material implementation and version** —
- **Known exclusions and reasons** —

| Run | Conditions | Evidence to record |
| --- | --- | --- |
| First visit | Fresh session, narrow viewport, storage unset | Whether the primary action is visible and usable while the first-visit banner is present |
| Return and recovery | Filter or draft in progress, detail route, Back or app recreation | Restored filter, draft, selection, focus, or scroll position, as applicable |
| Alternate input | Keyboard or screen reader, reduced motion where applicable | Active element and visible focus, announcement, and animation behavior |
| Slow or interrupted use | Cold cache or controlled network interruption in a test environment | Requested media variant, measured timing, retained inputs, and safe retry outcome |
| International | Supported locales, long text, and separate public URLs if applicable | Text wrapping, page language, metadata, and correct destination |
| Design handoff | Approved frame, view-only reviewer, clean prototype session | Version, token mode, assets, documented state and action behavior |
| External handoff | Open a contact channel or a published deep link | Correct destination and fallback. Use test accounts for sending data or messages. |

## Record a release decision

1. Link open findings to the [audit report](audit-report.md) and identify owners.
2. Review P0 and P1 findings before release. Record a decision and an owner for any accepted exception.
3. Repeat the same steps after each fix. Record the build, environment, and observed result.
4. Report lab and field performance separately. Record automated accessibility findings and manual results separately. A score by itself does not establish conformance.
