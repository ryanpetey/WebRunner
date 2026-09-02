# WebRunner Security Model

WebRunner follows a least-access model:

- No blanket required access to all websites.
- Website access is requested only for origins the user explicitly authorizes for a workflow.
- Authorized page agents run only on sites WebRunner has been granted access to. Redirect intermediaries do not need access merely because a workflow passes through them.
- Site access can be revoked from WebRunner or Chrome's extension settings.
- Bookmark access is optional and requested only when the user asks WebRunner to create or update a launcher bookmark.
- WebRunner does not request cookie access, browsing-history access, downloads access, clipboard access, network-interception permissions, or Chrome debugger access.
- Workflow definitions and reusable values are stored locally in Chrome. Temporary run state is session-scoped.
- WebRunner contains no remotely hosted executable code and has no developer-operated backend, analytics, advertising, or remote logging.

WebRunner does not auto-submit forms unless the user's workflow explicitly contains the relevant click action. Users should review and test workflows before using them on consequential forms.

WebRunner does not attempt to defeat authentication, CAPTCHA, access-control, rate-limit, or trusted-user-gesture protections. If a browser requires a real user click before protected sign-in information can be used, WebRunner pauses and asks the user to perform that click.

Saved workflow values are not separately encrypted by WebRunner. Passwords, authentication tokens, private keys, and other secrets should not be saved as reusable workflow values.

## Reporting a security issue

For ordinary bugs, use the public issue tracker. Do not include passwords, authentication tokens, confidential form contents, protected health information, personal data, or other sensitive information in a public issue.

For the current release candidate, there is no developer-operated service or credential store. This repository contains the public product, privacy, security, reviewer, and release documentation used for the Chrome Web Store release.
