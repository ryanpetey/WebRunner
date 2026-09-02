# WebRunner 1.0 — Chrome Web Store Submission Guide

## Upload package

Upload `WebRunner-1.0.0-Chrome-Web-Store.zip`.

WebRunner 1.0 is free. There is no paid functionality, subscription, account, or in-extension purchase flow in this release.

## Store listing

**Name**
WebRunner

**Category**
Productivity → Workflow & Planning

**Summary**
Point at website fields, save reliable workflows, and run them again without scripts, tab counting, or fixed delays.

**Detailed description**
WebRunner is a free Chrome extension for creating and replaying repetitive website workflows by pointing directly at the fields and controls you want to use.

Map text fields, dropdowns, multi-selects, buttons, dynamic controls, waits, and manual checkpoints from Chrome's side panel. Save the workflow once, then run it again without writing scripts, counting Tab presses, relying on screen coordinates, or building fixed delays.

WebRunner is designed for websites that change as you interact with them. It waits for controls to become genuinely ready, re-finds mapped elements using multiple page and accessibility clues, reads available choices directly from the page when possible, and supports common custom-control patterns such as Select2 and multi-selects.

WebRunner can continue workflows across explicitly authorized sites. When a browser requires a genuine user gesture for protected sign-in behavior, WebRunner pauses and asks the user for that click rather than attempting to bypass the browser protection.

Privacy is intentionally conservative. Website access is granted only to origins the user explicitly authorizes. Workflow definitions and reusable values are stored locally in Chrome. WebRunner has no account, developer-operated backend, analytics, advertising, or remote logging. Bookmark permission is optional and requested only if the user creates a launcher bookmark.

WebRunner executes user-defined actions and can submit forms or change records when a workflow tells it to. Users should test workflows before relying on consequential actions. Do not save passwords, authentication tokens, private keys, or other secrets as reusable workflow values.

## Public URLs

- Product site: https://ryanpetey.github.io/WebRunner/
- Terms of Use: https://ryanpetey.github.io/WebRunner/terms.html
- Privacy policy: https://ryanpetey.github.io/WebRunner/privacy.html
- Support: https://ryanpetey.github.io/WebRunner/support.html
- Project/security: https://github.com/ryanpetey/WebRunner

## Privacy practices

**Single purpose**
Let users create and replay local point-and-click website workflows on sites they explicitly authorize.

**sidePanel justification**
Provides WebRunner's user-facing workflow editor, workflow list, run controls, mapping controls, legal-policy review, and status UI in Chrome's side panel.

**storage justification**
Stores user-created workflow definitions, local settings, legal-policy acceptance metadata, and temporary run state so workflows persist and can resume reliably.

**scripting justification**
Injects WebRunner's packaged page agent only on websites the user has authorized. The page agent locates and interacts with mapped controls and reports workflow readiness/status locally to the extension.

**activeTab justification**
Allows WebRunner to connect to the current page when the user explicitly invokes the extension and creates/maps a workflow.

**optional bookmarks justification**
Used only when the user explicitly asks WebRunner to create or update a one-click launcher bookmark. WebRunner works without this permission.

**optional host access justification**
WebRunner is a general website workflow tool, so users may choose different HTTP/HTTPS sites. Host access is optional and requested at runtime only for origins the user chooses to map or automate. Redirect intermediaries do not receive access merely because a workflow passes through them.

**Remote code**
No. All executable extension code is included in the uploaded package.

## Data disclosure guidance

Disclose website content and user interactions because WebRunner processes them locally to map and run workflows. If the dashboard presents a separate category for form data or user-provided content, disclose it because workflow values can contain text the user chooses to save.

WebRunner may locally detect whether credential fields appear populated in order to determine whether a real user click is required. It does not store those credential contents as workflow values or transmit them to the developer. If the Chrome Web Store dashboard asks broadly whether authentication information is processed rather than collected/transmitted, choose the conservative disclosure and explain that processing is local-only and used solely for protected sign-in handoff.

WebRunner uses handled data only for its user-facing workflow functionality; it is not sold, used for advertising or unrelated profiling, or transmitted to a developer-operated backend.

## First-use legal disclosure

Before a workflow can be created or run after a material legal-policy update, WebRunner shows a one-time Terms/Privacy screen. The user must explicitly agree to the Terms of Use and acknowledge the Privacy Policy. The acceptance version and timestamp are stored locally. Bookmark launchers cannot bypass this requirement.

## Distribution

For the first submission choose **Unlisted**. After approval, test the Store-installed build on personal Chrome and then test the direct Store URL on the managed work computer. Store installation remains subject to enterprise Chrome policy.

## Reviewer notes

Use `docs/REVIEWER_NOTES.md` as the reviewer/testing instructions.
