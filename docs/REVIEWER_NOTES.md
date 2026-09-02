# Chrome Web Store Reviewer Notes

WebRunner is a local point-and-click website workflow tool. It has no login, subscription, developer-operated backend, remote code, analytics, advertising, or remote logging.

## First use

On first use, WebRunner presents a one-time Terms of Use / Privacy Policy screen. Check the agreement box and click **Continue**. The acceptance version and timestamp are stored locally in Chrome. This screen is intentionally shown before workflows can be created or run.

## Simple test

1. Open https://www.selenium.dev/selenium/web/web-form.html in Chrome.
2. Open the WebRunner side panel from the extension toolbar.
3. If the first-use disclosure is shown, review it, check the agreement box, and click **Continue**.
4. Click **+ New**.
5. Approve access to `www.selenium.dev` when Chrome prompts.
6. Add an **Enter text** step, click **Select on page**, and map the `Text input` field.
7. Enter any test text in WebRunner.
8. Add a **Choose option** step and map the page's `Dropdown (select)` field. WebRunner should load the available choices from the page.
9. Save the workflow and click **Run**.
10. WebRunner reloads the starting page and replays the mapped actions.

## Permission and data behavior

- Website access is optional and requested only for origins the user explicitly chooses to automate.
- A workflow can use multiple explicitly authorized origins; redirect intermediaries do not receive access merely because a workflow passes through them.
- The `bookmarks` permission is optional and is not requested unless the reviewer explicitly creates a launcher bookmark.
- WebRunner does not request Chrome debugger, cookie, history, downloads, clipboard, or network-interception permissions.
- WebRunner's executable code is fully packaged with the extension.
- Workflow definitions and reusable values are stored in `chrome.storage.local`; temporary run state is session-scoped.
- WebRunner does not transmit saved workflows or page content to a developer-operated server.
- On protected sign-in pages, WebRunner may locally detect whether credential fields appear populated so it can request a genuine user click. It does not store those credential contents as workflow values or transmit them to the developer.

Terms: https://ryanpetey.github.io/WebRunner/terms.html
Privacy: https://ryanpetey.github.io/WebRunner/privacy.html
