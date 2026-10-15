# Quality record

## Evidence boundary

This file records current-tree and deployed-origin checks for the monochrome release now live at [jb-braids.pages.dev](https://jb-braids.pages.dev/). Numeric production claims below come from the final deployed run, not the previous release.

## Current-tree evidence

- ESLint passed on the current source tree.
- TypeScript completed with no emitted files and no type errors.
- The production-mode application build completed successfully.
- 21 public-route, preset and PWA probes passed in the current-tree regression check; `/admin` correctly redirected to authentication.
- 36 referenced media and font assets returned successful, non-empty responses.
- All 24 explicit service-worker shell entries were retrievable after the live-only booking route was removed from the cache list.
- The generated content-security policy permits the intended TikTok frame origin while retaining strict frame and resource boundaries.
- Completed, cancelled and no-show records are excluded consistently from availability and booking-capacity checks.
- Global PWA registration covers direct visits to the gallery, price list and other public routes.
- The booking desk is not precached and falls back to the offline screen when its live API cannot be reached.

## Deployed production verification

- The final production contract completed with **110 passed · 0 failed** against the canonical origin.
- Live visual smoke checks passed at 1440 × 900 desktop and 390 × 844 mobile.
- The isolated production QA cleanup removed exactly the seven KV keys and one R2 object created by the verification run.
- Aggregate post-clean verification reported 0 booking records, 0 customer records, 0 loyalty records and a 0 B proof bucket.
- No record identifiers, proof names, contact details, credentials or raw cleanup output are included in this public repository.

## Responsive visual audit

The current interface was inspected at:

- 1440 × 900 desktop;
- 390 × 844 mobile;
- 360 × 800 mobile; and
- 320 × 568 compact mobile.

The review covered:

- hero composition, header height and founder card;
- Manrope and Newsreader scaling at smaller viewports;
- hamburger-menu scroll, close control and background locking;
- gallery rails and the Signature Twists focal crop;
- service-card media fit on desktop and mobile;
- price-list masthead and badge separation;
- Crown Club lookup and reward-summary widths;
- admin mobile density and empty-space removal;
- text contrast across image overlays and dark panels; and
- progressive-reveal fallback when JavaScript is unavailable.

The corrected layouts were rechecked at the affected breakpoints after the fixes.

## Interaction and hardening coverage

The deployed 110-check production contract covers the following release-critical behavior:

- public routes, same-origin destinations and internal fragment targets;
- manifest, app icons, shortcuts, service-worker shell and offline fallback;
- transport, framing, referrer, permission and content-type headers;
- booking-window, request-size, anti-spam, cross-origin and strict-schema rejection;
- Namibia-only phone validation and safe free-text normalization;
- callout address and Namibia map-pin requirements;
- server-calculated totals and 50% deposits;
- collision prevention, daily chair capacity and occupied-time removal;
- bounded 24-hour provisional unpaid holds;
- proof-file signature validation, private storage and no-store delivery;
- Crown Club privacy, completion awards, referral logic and idempotency;
- authenticated admin access, price publishing and calendar overrides; and
- booking and authentication rate limits.

## Completed launch gate

The private production repository completed:

1. lint, typecheck and production build;
2. Cloudflare bundle preparation;
3. booking-lock Worker deployment;
4. Pages deployment to the canonical origin;
5. the 110-check production contract against the deployed origin;
6. live desktop and compact-mobile smoke passes; and
7. removal and aggregate verification of every synthetic QA artifact.

Private credentials, raw proof files and client data are intentionally absent from this public record.

The canonical monochrome release is live and verified.
