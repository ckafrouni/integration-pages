# Executor Personal documentation

Static, documentation-only pages for **Executor Personal**, operated by **Christophe Kafrouni** for personal use. Executor Personal is a private, self-hosted integration layer supporting authorized personal AI-assisted workflows. It is not a public SaaS service or a Zentio offering.

This repository contains no runtime, application login, OAuth callback implementation, or connected-account processing. It uses plain HTML and CSS, native system fonts, and no scripts, external assets, remote fonts, or added analytics/tracking.

## Files

- `index.html`: purpose and integration status
- `privacy.html`: authorization, storage, AI processing, disclosure, revocation, and deletion
- `terms.html`: private-use terms and limitations
- `integrations.html`: provider overview
- `google.html`: Google integration being configured, not claimed connected
- `microsoft.html`: future planned integration, not live
- `contact.html`: private requests and public documentation links
- `styles.css`: shared responsive black-and-white design
- `README.md`: repository purpose, Pages setup, maintenance, and safety guidance
- `.nojekyll`: serve as a plain static site without Jekyll processing

## GitHub Pages configuration

Repository: `ckafrouni/integration-pages` (public personal repository).

In GitHub repository **Settings → Pages**, select **Deploy from a branch**, choose **main**, and choose **/ (root)**. Keep all files listed above at the repository root. No build step is required.

Site base URL (after GitHub Pages deployment):

`https://ckafrouni.github.io/integration-pages/`

Expected page paths under that base URL:

- `index.html` (also the root landing page)
- `privacy.html`
- `terms.html`
- `integrations.html`
- `google.html`
- `microsoft.html`
- `contact.html`

All local links use relative paths so privacy and terms remain on the same origin. A custom domain is optional and is **not configured** by these files; no CNAME file is included.

## Content boundaries

Documentation date: **14 October 2026**.

- Google is being configured; no active connection, provider approval, or formal verified status is claimed.
- Microsoft is future planned and not live.
- OAuth access is limited by granted scopes and provider rules.
- OAuth tokens are stored encrypted in Executor. This is not a statement about encryption of all histories, logs, or backups.
- Authorized data and results may persist in task histories, logs, or backups, depending on configuration. No exact retention schedule is verified.
- The operator handles deletion, including local stores. Revoking permissions does not automatically delete previously retained histories or backups.
- AI workflows may share relevant data with configured agent or model providers. No definitive provider list or zero-retention/no-training configuration is verified.
- Google user data use is subject to Google API Services User Data Policy, including Limited Use. Its restrictions on selling, advertising, and general-purpose model training are not a guarantee of provider zero retention.
- This static site processes no integration data. GitHub may log visitor IP addresses and security data under its own privacy policy.

## Adding future integrations

1. Add a provider-specific root-level HTML page using the shared layout and stylesheet.
2. Clearly distinguish planned, configuring, and live status. Only claim a live connection after confirmation.
3. Document actual products, granted/requested permissions as appropriate, supported operations, authorization and revocation behavior, storage, disclosure, and deletion.
4. Link the provider’s real applicable policies. Do not reuse Google-specific policy language as a substitute for another provider’s requirements.
5. Update `integrations.html`, the homepage, privacy policy, and terms where applicable. Date the content changes.
6. Verify statements about AI providers, retention, training settings, encryption, or formal review before making affirmative claims. If details remain unknown, say so.
7. Check relative links, semantic headings, keyboard focus, readable contrast, and narrow-screen layout.

## Public repository safety

Do not commit secrets, credentials, OAuth client IDs, cloud project identifiers, server addresses, internal URLs, email addresses, account data, or private workflow logs. This repository should contain public documentation only.

Use an existing private communication channel with the operator for private account or deletion requests. Never put sensitive information into public issues. Non-sensitive documentation corrections can be filed at:

https://github.com/ckafrouni/integration-pages/issues

Operator profile: https://github.com/ckafrouni
