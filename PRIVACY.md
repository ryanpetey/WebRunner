# WebRunner Privacy Policy

**Effective date: September 2, 2026**

WebRunner is a local-first Chrome extension for creating and replaying user-defined website workflows.

## Information WebRunner handles

When you map or run a workflow on a website you explicitly authorize, WebRunner may process website content needed for that workflow, including page URLs, field labels, accessibility attributes, dropdown choices, mapped-control information, values you choose to save, page readiness, and interactions needed to continue the workflow.

Values you choose to save in a workflow may include personally identifiable information, such as names, email addresses, usernames, or mailing addresses, if you choose to place that information in a workflow. WebRunner stores those saved workflow values locally in Chrome and does not transmit them to the developer.

On sign-in pages, WebRunner may locally detect whether credential fields appear populated so it can determine whether the browser requires a real user click. WebRunner does not store those credential contents as workflow values or send them to the developer.

Workflow definitions, reusable values, workflow settings, and the record that you accepted the current Terms and Privacy Policy are stored locally in Chrome extension storage. Temporary run state is stored for the browser session.

## How information is used

WebRunner uses this information only to map, save, and replay the workflows you create, including continuing across explicitly authorized sites and handing control back to you when a real user interaction is required.

## Data transmission and sharing

WebRunner has no developer-operated backend, account system, analytics service, advertising SDK, or remote logging endpoint. WebRunner does not transmit page content or saved workflows to the developer and does not sell user data.

When WebRunner fills, clicks, or submits a third-party website at your direction, that website may process or transmit the resulting data according to its own behavior and privacy practices. That transmission is between your browser and the website you chose to automate, not a WebRunner service.

## Permissions

WebRunner requests website access only for origins you choose to authorize. A workflow can use more than one explicitly authorized site and can pass through redirect sites without receiving access to those intermediary sites.

Bookmark access is optional and is requested only when you ask WebRunner to create or update a bookmark launcher.

WebRunner does not request access to browser cookies, browsing history, downloads, clipboard contents, network interception APIs, or Chrome's debugger API.

## Retention and deletion

Saved workflows and legal-acceptance metadata remain in Chrome's local extension storage until you delete them, clear extension data, or uninstall WebRunner. Temporary workflow-run state is session-scoped. You can revoke a website's access from WebRunner or Chrome's extension settings.

## Security

WebRunner does not separately encrypt saved workflow values. Do not save passwords, authentication tokens, private keys, or other secrets as reusable workflow values.

WebRunner intentionally does not attempt to bypass browser protections that require a real user gesture for protected sign-in behavior. When necessary, WebRunner pauses and asks you to perform the click yourself.

## Chrome Web Store Limited Use

WebRunner's use of information received from Chrome APIs complies with the Chrome Web Store User Data Policy, including the Limited Use requirements. WebRunner uses authorized website and browser data only to provide or improve its user-facing workflow automation features. WebRunner does not use or transfer user data for personalized advertising, retargeting, credit-worthiness, lending, or unrelated profiling, and the developer does not permit humans to read user data except where you specifically provide information for support or where otherwise allowed by the Chrome Web Store User Data Policy.

## Contact

For support or privacy questions, use the [WebRunner issue tracker](https://github.com/sidecarworks/WebRunner/issues/new). Do not include passwords, authentication tokens, confidential form contents, protected health information, personal data, or other sensitive information in an issue.
