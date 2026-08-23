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
- WebRunner has no developer-operated backend, analytics service, advertising SDK, or remote logging endpoint.

WebRunner does not auto-submit forms unless the user's workflow explicitly contains the relevant click action. Users should review workflows before using them on consequential forms.

## Reporting a security issue

For ordinary bugs, use the public issue tracker. Do not include passwords, authentication tokens, confidential form contents, protected health information, or other sensitive data in a public issue.

For the current beta, there is no developer-operated service or credential store to compromise; the extension's source is kept in this repository to make its behavior auditable.
