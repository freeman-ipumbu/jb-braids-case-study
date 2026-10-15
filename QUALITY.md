# Quality record

## Automated production-equivalent suite

**Result: 109 passed · 0 failed**

Coverage included:

- public home, dedicated `/gallery`, focused `/book`, price list, offline page, manifest, service worker, robots, sitemap and app icons;
- rendered same-origin destination crawling, query-aware booking links and internal-fragment validation;
- strict transport, frame, referrer, permission and content-type headers;
- installable-PWA mode, icons and shortcuts;
- service availability and real start times;
- body-size, honeypot, booking-window, cross-origin and strict-schema rejection;
- Namibia-only phone validation and safe colour input;
- callout address and Namibia map-pin requirements;
- server-calculated totals and 50% deposits;
- reference and referral-code issuance;
- collision prevention and removal of occupied times;
- proof signature sniffing, origin checks, private storage and no-store delivery;
- Crown Club privacy, award logic and idempotency;
- admin origin/authentication enforcement;
- rejection of forged ChatGPT identity headers on Pages;
- service price publishing and restoration;
- calendar override publishing and restoration;
- booking rate limiting.

## Live release smoke test

The deployed `jb-braids.pages.dev` environment was checked separately:

- owner PIN accepted and signed session issued;
- wrong owner PIN rejected;
- forged identity header rejected with 403;
- live booking accepted;
- simultaneous duplicate rejected with 409;
- cancellation released the booked interval;
- released time returned to public availability;
- temporary booking and customer QA records removed from production.

## Responsive and interaction audit

- 320 × 568 compact mobile, 390 × 844 mobile and 1280 × 720 laptop visual passes;
- 390 × 844 rendered heights: 13,293 px home, 3,653 px gallery and 5,157 px booking desk;
- the laptop hero occupies the exact 642 px available below the 78 px header, with heading, actions, proof and video all inside the first viewport;
- four home signature cards, five portfolio-preview frames, three default TikTok features and five switched Instagram favourites verified;
- eight gallery editorial frames and six bookable signature cards verified;
- 0 horizontal page overflow;
- 0 missing internal anchors;
- 0 empty buttons or links;
- no visible mobile buttons below the 44 px target size;
- Explore opens from the header and dock, locks the page, remains internally scrollable, closes by button or Escape, and restores focus;
- the Signature Twists focal crop was verified at `50% 18%`, preserving the full head and braid silhouette;
- social switching, story and booking disclosures, query-aware service preselection, Namibia-only client fields, Windhoek callout map, admin lock/logout, calendar selection and service save verified through the UI;
- no live-site browser console errors observed.
