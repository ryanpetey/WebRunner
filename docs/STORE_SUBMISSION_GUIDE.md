# WebRunner 1.0 Beta — Chrome Web Store Submission Guide

## Upload package

Upload `WebRunner-1.0.0-Chrome-Web-Store.zip` from the release kit.

## Store listing

**Name**
WebRunner

**Category**
Productivity

**Summary**
Point at website fields, save reliable workflows, and run them again without scripts, tab counting, or fixed delays.

**Detailed description**
WebRunner lets you teach Chrome repetitive website workflows by pointing at the page.

Map text fields, dropdowns, buttons, dynamic controls, and manual checkpoints, then replay the workflow from the Chrome side panel or an optional one-click bookmark launcher.

WebRunner is designed to be resilient instead of timing-dependent. It waits for controls to be genuinely ready rather than relying on fixed sleep times, reads dropdown choices directly from the page when possible, supports native controls plus common custom patterns such as Select2 and multi-selects, and can remap or resume a workflow from a specific step when a website changes.

Privacy is intentionally conservative. WebRunner requests site access one website at a time. Workflow definitions and reusable values are stored locally in Chrome. WebRunner has no account, developer-operated backend, analytics, advertising, or remote logging. Bookmark permission is optional and requested only if you create a launcher bookmark.

Do not store passwords, authentication tokens, or other secrets as reusable workflow values.

## Public URLs

- Product site: https://ryanpetey.github.io/WebRunner/
- Privacy policy: https://ryanpetey.github.io/WebRunner/privacy.html
- Support: https://ryanpetey.github.io/WebRunner/support.html
- Source/security: https://github.com/ryanpetey/WebRunner

## Privacy practices

**Single purpose**
Let users create and replay local point-and-click workflows on websites they explicitly authorize.

**sidePanel justification**
Provides WebRunner's user-facing workflow editor, workflow list, run controls, mapping controls, and status UI in Chrome's side panel.

**storage justification**
Stores user-created workflow definitions and settings locally in Chrome so workflows persist between browser sessions.

**scripting justification**
Injects WebRunner's packaged page runner only when the user maps or runs a workflow on a website the user has authorized. The injected runner locates and interacts with the mapped page controls.

**activeTab justification**
Allows WebRunner to identify and interact with the currently active page when the user explicitly opens and uses the extension, including creating a workflow from the current page.

**optional bookmarks justification**
Used only when the user explicitly asks WebRunner to create or update a one-click launcher bookmark for a saved workflow. WebRunner works without this permission.

**optional host access justification**
WebRunner is a general website automation tool, so users may choose different HTTP/HTTPS sites. Host access is optional and requested at runtime only for the specific website origin the user chooses to map or automate. No site is granted access automatically.

**Remote code**
No. WebRunner does not execute remotely hosted code. All executable extension code is included in the uploaded package.

## Data disclosure guidance

Disclose website content and user interactions because WebRunner processes them locally to run workflows. If the dashboard presents a separate category for form data or user-provided content, select it because workflow values can contain text the user chooses to save.

WebRunner uses data only for its user-facing workflow functionality; it is not sold, used for advertising or unrelated profiling, or transferred to the developer or third parties by WebRunner.

## Distribution

For the first submission choose **Unlisted**. After approval, test the store-installed build on personal Chrome and then test the direct Store URL on the managed work computer.

## Reviewer notes

Use `docs/REVIEWER_NOTES.md` as the reviewer/testing instructions.
