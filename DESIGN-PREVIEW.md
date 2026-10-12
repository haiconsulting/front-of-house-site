# FOH design preview

- URL: https://designpreview.fohrestaurants.com
- Repository: `haiconsulting/front-of-house-site` (current GitHub location)
- Branch: `codex/foh-design-preview`
- Coolify GitHub source: `hai-coolify`
- Base: `bb6c086` (latest main when prepared on October 12, 2026)
- Coolify application: `foh-design-preview` (`wax2i2ymhmv6e1m541a6blxn`)
- Server: Vultr `foh-edge-01`; Cloudflare proxied A record.

This standalone Coolify application builds the branch using the repository Dockerfile on port 4321. Production continues to track main in its existing application. Do not merge or promote this branch until the redesign is approved.

Set the public build variable `PUBLIC_PREVIEW_ORIGIN=https://designpreview.fohrestaurants.com` only on this preview application. It adds noindex metadata and uses preview-hosted social images. Leave it unset for production. Runtime contact and Host variables are configured in Coolify, never committed.

The preview includes the redesigned brand, full Templates studio, current media, Privacy page, and the existing local Terms/provider pages. Contact inquiries use the existing studio email delivery configuration; team submissions are real inquiries.

Build locally with `npm ci` then `npm run build`. Use `npm run dev` for port 4999. For preview metadata, set the public build variable above when building.

Verified October 12, 2026: production build, HTTPS and HTTP redirect, primary routes and assets, preview noindex metadata, 375px mobile navigation, Templates name/color personalization, full template opening, and API input validation. No test inquiry email was sent.
