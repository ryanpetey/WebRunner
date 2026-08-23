# Chrome Web Store Reviewer Notes

WebRunner is a local point-and-click website workflow tool. It has no login, subscription, backend service, remote code, analytics, advertising, or remote logging.

## Simple test

1. Open https://www.selenium.dev/selenium/web/web-form.html in Chrome.
2. Open the WebRunner side panel from the extension toolbar.
3. Click **+ New**.
4. Click **Allow this site** and approve access to `www.selenium.dev` when Chrome prompts.
5. Add an **Enter text** step, click **Select on page**, and map the `Text input` field.
6. Enter any test text in WebRunner.
7. Add a **Choose option** step and map the page's `Dropdown (select)` field. WebRunner should load the available choices from the page.
8. Save the workflow and click **Run**.
9. WebRunner reloads the starting page and replays the mapped actions.

## Permission behavior

- Website access is optional and requested only for the specific origin being automated.
- The `bookmarks` permission is optional and is not requested unless the reviewer explicitly clicks **Create bookmark**.
- WebRunner's executable code is fully packaged with the extension.
- Workflow definitions are stored in `chrome.storage.local`.
- WebRunner does not transmit saved workflows or page content to a developer-operated server.
