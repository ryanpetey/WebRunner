# WebRunner Legal & Risk Release Checklist

This checklist tracks risk controls for the current local-first Chrome extension architecture.

## Completed for the first unlisted/free release

- [x] Publish an accurate Privacy Policy and link it from the product/support site and Store materials.
- [x] Publish Terms of Use and link them from the product/support site.
- [x] Add explicit first-use Terms/Privacy assent before workflows can be created or run after a material legal-policy update.
- [x] Block bookmark launches from bypassing required legal acceptance.
- [x] Keep marketing claims narrow and avoid absolute compatibility/security claims.
- [x] State that WebRunner executes user-defined actions that can submit forms or change records.
- [x] State that WebRunner is not a password manager and reusable workflow values should not contain passwords, tokens, private keys, or other secrets.
- [x] State that users are responsible for authorization to automate third-party sites and for applicable site/employer policies.
- [x] Prohibit use to bypass authentication, CAPTCHAs, access controls, rate limits, or other technical restrictions.
- [x] Preserve the trusted-click handoff instead of using Chrome debugger access to defeat browser credential protections.
- [x] Keep permissions least-privilege: no `tabs`, debugger, cookie, history, clipboard, downloads, or network-interception permissions.
- [x] No third-party runtime libraries, bundled web fonts, or remotely hosted executable code in the packaged extension.
- [x] Keep support instructions warning users not to post sensitive/confidential data publicly.
- [x] Stage Chrome Web Store privacy disclosures to match current local-only behavior and cross-site workflow behavior.

## Required immediately before submission

- [ ] Confirm the final Chrome Web Store Privacy-tab checkboxes match the final manifest and the current policy text.
- [ ] Confirm 2-step verification and publisher recovery methods on the Sidecar Works publisher account.
- [ ] Run the complete regression suite and final manual smoke tests against the exact release package.
- [ ] Archive the exact release ZIP and source snapshot with version, date, and SHA-256 hash.
- [ ] Use real screenshots from non-confidential/demo websites and avoid implying third-party endorsement.
- [ ] Submit the first release as **Unlisted** and test the Store-installed build before widening distribution.

## Before a broadly public or paid release

- [ ] Perform a proper trademark clearance for **WebRunner**, **Sidecar Works**, and the W+arrow logo.
- [ ] Consider a Washington LLC or other appropriate entity if minimizing personal exposure remains a priority.
- [ ] Have a software/technology attorney review the Terms, Privacy Policy, Store disclosures, entity setup, trademark position, and liability model.
- [ ] Evaluate technology errors & omissions / cyber liability insurance once usage becomes meaningful.
- [ ] Establish a non-public security-reporting route for vulnerability reports.

## Before adding accounts, sync, analytics, or a backend

- [ ] Re-review the Privacy Policy, Terms, and Chrome Web Store disclosures before any new developer-controlled data flow ships.
- [ ] Define collection, retention, deletion, and security practices for any remotely stored data.
- [ ] Perform a separate compliance review before WebRunner-controlled infrastructure processes regulated data.
- [ ] Do not claim HIPAA, PCI, SOC 2, GDPR, or similar compliance without a real basis.

These controls reduce practical risk but do not substitute for individualized legal advice. A focused technology-lawyer review is recommended before a broadly public or paid launch.
