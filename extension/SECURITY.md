# WebRunner Security Model

WebRunner follows a least-access model:

- No blanket access to all websites.
- Website access is requested only for the specific origin used by a workflow.
- The page runner is injected only when WebRunner is actively used or a saved workflow is launched on an authorized site.
- Site access can be revoked from the workflow editor or Chrome's extension settings.
- Bookmark access is optional and requested only when the user asks WebRunner to create or update a launcher bookmark.
- WebRunner does not request cookie access, browsing-history access, downloads access, clipboard access, or network interception permissions.
- Workflow definitions are stored locally in Chrome.
- WebRunner contains no remotely hosted executable code.

WebRunner does not auto-submit forms unless the user's workflow explicitly contains the relevant click action. Users should review workflows before using them on consequential forms.
