# PANTIK UI/UX Knowledge Base

A reusable audit checklist for websites, native apps, and Figma designs. Each of the 95 checks has a stable ID, a test method, a suggested fix, and a reference. The original 55 checks keep their IDs. The 22 Material implementation checks use the MAT prefix. The 18 release checks use the REL prefix.

## Run an audit

1. Copy [Audit-Checklist.csv](Audit-Checklist.csv) and open the copy in a spreadsheet editor. Import it as UTF-8 with a comma delimiter if it opens in one column.
2. Record the build or design version, platform, locale, and main user journey. For a portfolio, try going from the home page to a project and then to the contact action.
3. Select checks marked **All** and checks for the relevant platform. Include **Web / Native app** when auditing either implementation. Run MAT checks for the installed library and platform, then mark irrelevant legacy or migration checks **Not applicable**.
4. Mark each applicable check **Pass**, **Fail**, **Not applicable**, or **Not tested**. Record an observation, screenshot, measurement, or reason alongside the result.
5. Collect confirmed defects in the [audit report](07-report/audit-report.md). Use the [GitHub issue template](.github/ISSUE_TEMPLATE/ui-ux-finding.md) when tracking fixes.
6. Reproduce each fixed issue in the same environment and record the new build and result.

## Checklist by topic

| Topic | Checks |
| --- | ---: |
| [User journeys and clarity](01-ux/checklist.md) | 10 |
| [Visual systems and Material 3](02-ui-material/checklist.md) | 9 |
| [Accessibility](03-accessibility/checklist.md) | 15 |
| [Websites and web apps](04-web/checklist.md) | 7 |
| [Native apps](05-mobile-app/checklist.md) | 7 |
| [Figma and developer handoff](06-figma/checklist.md) | 7 |
| [Material Web implementation](10-material-implementation/material-web.md) | 8 |
| [Android Material implementation](10-material-implementation/android.md) | 8 |
| [iOS Material implementation](10-material-implementation/ios.md) | 6 |
| [Web release checks](11-release-readiness/web.md) | 8 |
| [Web accessibility release checks](11-release-readiness/web-accessibility.md) | 2 |
| [Native app release checks](11-release-readiness/native-apps.md) | 4 |
| [Figma release and handoff checks](11-release-readiness/figma.md) | 4 |

## Quick review

Start with UX-01, UX-04, UI-03, UI-08, and A11Y-01. Add A11Y-04, A11Y-05, WEB-01, and WEB-05 for web. Add APP-01, APP-03, APP-04, and APP-05 for native apps. Add FIG-01, FIG-03, FIG-04, and FIG-06 for Figma.

Use Material 3 as a design-system reference. Apply project-specific visual rules where appropriate. Use WCAG 2.2 AA for web accessibility checks and platform guidance for native apps. Verify runtime behavior on a working build and combine automated checks with manual testing.

- [Release test matrix](07-report/release-matrix.md)
- [Worked example](07-report/example.md)
- [Source register](08-sources/sources.md)
- [Reusable prompt for ChatGPT or Codex](09-codex/run-audit.md)

## Run the audit skill in Codex

Open a checkout of this repository as the Codex workspace. The [PANTIK UX Audit skill](.agents/skills/pantik-ux-audit/SKILL.md) is in the project skill directory. In a different workspace, copy the entire `pantik-ux-audit` folder into that project's `.agents/skills/` directory. The skill can read the canonical knowledge base when there is no local copy of the checklist.

Invoke it in one message after opening the workspace:

```text
$pantik-ux-audit Audit https://pantikdesign.pages.dev/ using Simba's journey from first visit to prepared contact message. Write the report in Polish.
```

For a live website, give the agent a browser with screenshot capability. The report distinguishes observed behavior from checks that require missing access or tools.
