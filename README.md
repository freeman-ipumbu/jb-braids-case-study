<p align="center">
  <img src="assets/jb-braids-mark.svg" width="112" alt="JB.Braids continuous-line feminine portrait mark" />
</p>

<h1 align="center">JB.Braids — Wear Your Story</h1>

<p align="center">
  A monochrome booking flagship and private studio system for Windhoek hairstylist Jessica Autoni.<br />
  Editorial discovery, a curated gallery, live booking, client rewards and private owner operations—designed as one unmistakably JB experience.
</p>

<p align="center">
  <a href="https://jb-braids.pages.dev/"><strong>Enter the live experience ↗</strong></a>
  &nbsp;·&nbsp;
  <a href="https://www.instagram.com/_jb.braids_/">JB.Braids Instagram ↗</a>
  &nbsp;·&nbsp;
  <a href="https://www.instagram.com/jessica_autony/">Meet Jessica ↗</a>
  &nbsp;·&nbsp;
  <a href="https://www.tiktok.com/@jb.braids7">TikTok ↗</a>
</p>

<p align="center">
  <strong>Now live:</strong> the monochrome release is deployed at the canonical production domain and has completed its post-deployment verification gate.
</p>

<p align="center">
  <a href="https://jb-braids.pages.dev/"><img src="assets/jb-braids-release-2026.webp" width="100%" alt="Final black-and-white JB.Braids launch artwork featuring the continuous-line feminine portrait identity and Jessica Autoni founder lockup" /></a>
</p>

<table>
  <tr>
    <td width="20%"><img src="assets/jessica-autoni-founder-2026.webp" alt="Jessica Autoni, founder and lead stylist of JB.Braids" /></td>
    <td width="20%"><img src="assets/burgundy-river-locs.webp" alt="Burgundy river locs by JB.Braids" /></td>
    <td width="20%"><img src="assets/burgundy-beaded-cornrows.webp" alt="Burgundy beaded cornrows by JB.Braids" /></td>
    <td width="20%"><img src="assets/midnight-pixie-mullet.webp" alt="Midnight pixie mullet by JB.Braids" /></td>
    <td width="20%"><img src="assets/golden-passion-twists.webp" alt="Golden passion twists by JB.Braids" /></td>
  </tr>
</table>

## The brief

JB.Braids began as Jessica’s student hustle in 2022 and grew into a high-demand home studio with a loyal social audience. The business already had the craft, personality and proof. It needed a digital home that could carry that energy while turning a message-heavy booking process into something clearer, safer and easier to run.

The result is not a generic salon template. It is a distinctly African, founder-led editorial system built around Jessica’s real operating rhythm: advance bookings, a verified 50% deposit, only 3–5 clients per day, home-studio privacy, Windhoek house calls, away calls and return-client rewards.

## The creative direction

**Hair as authorship. Booking as choreography.**

The live release pairs a strict black, white and graphite foundation with the natural colour and texture of Jessica’s work. Manrope brings compact clarity to navigation, labels and operational screens; Newsreader adds warmth and fashion-editorial contrast to selected statements. A new one-colour **continuous-line feminine portrait** leads the identity: its long braid suggests a subtle **J**, while the sculpted hair loops hint at a **B**. The mark stays legible from editorial scale down to the favicon and install icon.

The restraint is intentional: the interface recedes, the hairstyles own the colour, and every dense area is broken into curated previews, horizontal rails, disclosures or dedicated pages rather than one endless wall of content.

## What was built

| Client experience | Studio operations | Trust and resilience |
| --- | --- | --- |
| Curated home edit, 12-look `/gallery` and six-film studio player | Authenticated private studio desk | Server-controlled pricing, totals and 50% deposit |
| Complete `/price-list` and focused `/book` journey | Booking, status and proof workflow | Atomic collision and daily-capacity protection |
| 2–90 day availability calendar | Calendar capacity and blocked days | Namibia-only phone validation |
| Home-studio, house-call and away-call routes | Service pricing and duration editor | Strict origin, schema and upload validation |
| Windhoek address search and map pin | Crown Club and referral ledger | Private payment-proof storage |
| Optional colour, prep, reference and custom-request details | Founder-specific embedded operating guide | 24-hour provisional unpaid hold |
| Crown Club return-client rewards | Mobile-first booking management | Installable PWA with versioned line-art icons and truthful offline handling |

## Jessica is part of the brand

The live experience gives the founder a visible role instead of hiding her behind a business handle. Jessica appears in the hero, a dedicated founder story, the launch preview and structured business identity, with a direct route to [her personal Instagram](https://www.instagram.com/jessica_autony/). The final founder portrait was selected by Jessica; her portrait and the JB.Braids portfolio are used with permission.

That presence matters: clients are not only choosing a hairstyle. They are trusting a person, her taste and her hands.

## Social proof became product content

JB.Braids’ public Instagram and TikTok work was treated as evidence, not decoration. The final experience separates a tight home edit from a deliberately ordered 12-look gallery, presents six original vertical studio films through one active player rather than six competing embeds, switches cleanly to selected TikTok and Instagram channels, and links back to Jessica’s original profiles.

This keeps the site anchored in real work without forcing every visitor to scroll through every asset before they can understand the offer or book.

Link previews now use a cache-busted 1200 × 630 black-and-white line-art launch card, canonical URLs, route-specific Open Graph fields, route-specific Twitter card fields and descriptive image text, so JB.Braids is represented consistently when the production link is shared.

## The booking system

```mermaid
flowchart LR
    A[Choose a look] --> B[Choose studio or callout]
    B --> C[Live date and time availability]
    C --> D[Client details and optional requests]
    D --> E[Server recalculates total and 50% deposit]
    E --> F[Atomic slot claim]
    F --> G[24-hour provisional payment window]
    G --> H[Jessica verifies and confirms]
    H --> I[Completed visit earns a Crown]
```

Services with longer chair times consume more daily-capacity units, overlapping appointments cannot be claimed twice, and expired unpaid requests stop reserving capacity after 24 hours. Completed, cancelled and no-show requests are excluded from active capacity. Clients never control their own price, deposit, after-hours fee or reward totals. A start time at or after 17:00 adds the server-owned N$100 after-hours fee before the 50% deposit is calculated.

Gallery and menu choices deep-link into `/book?service=…`, so the selected look arrives prefilled. Colour, beads, prep, takedown, email, referral and custom-request fields remain available behind clear optional disclosures rather than lengthening everyone’s first pass.

## Policy without the wall of text

The website intentionally presents Jessica’s terms as a concise four-card summary: the mandatory non-refundable 50% deposit; the 20-minute grace period and N$50 late fee; the N$100 after-hours or accepted urgent-booking fee; and the timing of the final balance. Clients acknowledge the current policy version inside the booking journey, and the server rejects stale acknowledgements rather than silently accepting changed terms.

The complete supplied Terms & Conditions wording is preserved in the private handover source for the separate poster designer. It is not repeated as a long legal page on the public website.

## Crown Club

Each completed appointment adds one Crown. On the fourth completed appointment, the server converts four Crowns into **N$150 of recorded service credit** for a future service. The booking form does not automatically spend that credit or reduce the required deposit. Referral credits are ledger-backed and awarded only after the referred client’s first completed appointment.

The public lookup requires both a booking reference and the matching Namibian phone number; it does not expose client information from a reference alone.

## Platform

The public site and server-rendered application run on Cloudflare Pages. Operational records use Cloudflare KV, payment proofs are private in R2, and a service-bound Durable Object provides the atomic booking lock that prevents collision and daily-capacity races.

The installable PWA uses the final line-art identity across standard, maskable and Apple-touch icons and caches the discovery shell and assets, but the booking desk is deliberately live-only. An offline visitor receives a clear reconnect state instead of a stale form that appears able to submit.

The production implementation remains private. This repository is a portfolio-safe design and engineering case study.

## Release quality

The deployed monochrome release passed lint, TypeScript, production-mode build, current-tree route/PWA/asset probes and the final production contract: **146 passed · 0 failed**. Live visual smoke review covered 1440 × 900 desktop, 390 × 844 mobile, 320 × 568 compact mobile and 844 × 390 compact landscape. The line-art identity, film switcher, gallery actions, booking entry, founder crop, concise policy, exact 2-day/90-day booking boundaries, 17:00 fee boundary, header, mobile dock and route-specific social metadata were included in the final scrutiny. An isolated synthetic production run was fully cleaned, and aggregate post-clean verification found no booking, customer, loyalty or proof artifacts remaining.

See the [quality record](QUALITY.md) and [architecture notes](ARCHITECTURE.md) for the evidence boundary and system design.

## Credits

**[Jessica Autoni](https://www.instagram.com/jessica_autony/)** — Founder, stylist and creative subject<br />
**JB.Braids** — Original hair work, images and social content<br />
**SolarSpin Technologies** — Brand direction, experience design, engineering and launch

Built in Windhoek, Namibia.<br />
[A Digital Experience by SolarSpin Technologies](https://solarspin-namibia.pages.dev/)

---

<sub>All JB.Braids brand assets, photography and client imagery are used with permission and remain the property of their respective owners. This public repository is a portfolio case study, not an open-source distribution of the production application.</sub>
