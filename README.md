# WebRunner

**Point. Save. Run.**

WebRunner is a local-first Chrome extension for creating and replaying point-and-click website workflows without scripts, tab counting, screen coordinates, or fixed sleep times.

## What it does

- Map text fields, dropdowns, buttons, dynamic elements, and manual checkpoints by clicking the page.
- Re-find mapped elements using multiple DOM and accessibility clues instead of tab order.
- Wait for controls to be genuinely ready rather than relying on fixed delays.
- Read available dropdown choices directly from the page when possible.
- Support native controls plus reusable custom-control patterns such as Select2 and multi-selects.
- Save workflows locally and run them from Chrome's side panel or an optional bookmark launcher.

## Privacy and security

WebRunner has no developer-operated backend, account system, analytics, advertising, or remote logging. Site access is granted one website at a time and workflow definitions are stored locally in `chrome.storage.local`.

WebRunner does not request access to cookies, browsing history, downloads, clipboard contents, or network interception APIs. Bookmark permission is optional and requested only when the user creates or updates a launcher bookmark.

Saved workflow values are not separately encrypted by WebRunner. Do not store passwords, authentication tokens, or other secrets as reusable workflow values.

- [Privacy Policy](PRIVACY.md)
- [Security Model](SECURITY.md)
- [Support](https://github.com/ryanpetey/WebRunner/issues/new)

## Status

WebRunner 1.0 is currently a beta release candidate being prepared for Chrome Web Store review.
