# WebRunner 1.0 Beta

WebRunner is a Chrome extension for point-and-click website workflows.

## What it does

- Maps text fields, dropdowns, buttons, dynamic elements, and manual checkpoints by clicking the page.
- Re-finds mapped elements using multiple DOM and accessibility clues instead of tab order or screen coordinates.
- Waits for controls to be genuinely ready rather than relying on fixed sleep times.
- Reads available dropdown choices directly from the page when possible.
- Supports native controls plus common custom patterns such as Select2 and multi-selects.
- Saves workflows locally and can run them from the side panel or an optional bookmark launcher.

## Privacy and access

WebRunner has no account, backend service, analytics, advertising, or remote logging. On websites the user explicitly authorizes, WebRunner reads the page information needed to map and run the user's workflow. Workflow definitions and reusable values are stored in `chrome.storage.local` on the device.

Website access is requested one origin at a time. Bookmark permission is optional and requested only when the user creates or updates a launcher bookmark.

Saved workflow values are not encrypted by WebRunner. Do not store passwords, authentication tokens, or other secrets as reusable workflow values.
