# WebRunner

**Point. Save. Run.**

WebRunner is a free, local-first Chrome extension for creating and replaying point-and-click website workflows without scripts, tab counting, screen coordinates, or fixed sleep times.

## What it does

- Map text fields, dropdowns, buttons, dynamic elements, and manual checkpoints by clicking the page.
- Re-find mapped elements using multiple DOM and accessibility clues instead of tab order.
- Wait for controls to be genuinely ready rather than relying on fixed delays.
- Read available dropdown choices directly from the page when possible.
- Support native controls plus reusable custom-control patterns such as Select2 and multi-selects.
- Save workflows locally and run them from Chrome's side panel or an optional bookmark launcher.
- Continue across explicitly authorized sites and hand control back to the user when a protected sign-in requires a real click.

## Privacy and security

WebRunner has no developer-operated backend, account system, analytics, advertising, or remote logging. Site access is granted only to origins the user explicitly authorizes and workflow definitions are stored locally in `chrome.storage.local`.

WebRunner does not request access to cookies, browsing history, downloads, clipboard contents, network interception APIs, or Chrome's debugger API. Bookmark permission is optional and requested only when the user creates or updates a launcher bookmark.

Saved workflow values are not separately encrypted by WebRunner. Do not store passwords, authentication tokens, private keys, or other secrets as reusable workflow values.

## Authorized use

Use WebRunner only on websites, accounts, systems, and data you are authorized to access and automate. Do not use it to bypass authentication requirements, CAPTCHAs, access controls, rate limits, or other technical restrictions.

WebRunner executes user-defined actions and can submit forms or change records when a workflow tells it to. Users should review and test consequential workflows before relying on them.

- [Terms of Use](TERMS.md)
- [Privacy Policy](PRIVACY.md)
- [Security Model](SECURITY.md)
- [Support](https://github.com/ryanpetey/WebRunner/issues/new)

## Status

WebRunner 1.0 is the free first release being submitted to the Chrome Web Store.
