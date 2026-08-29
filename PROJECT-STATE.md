# Great Lakes Exterior Cleaning — project state (Aug 22, 2026)

## Where things stand

The site is **built and approved by the owner**. Live file:
`Great Lakes Exterior Cleaning Site.dc.html` — Home, Before/After, Contact + quote
request, plus a Design system page (palette, type scale, spacing scale, buttons,
form fields, cards, all states).

Logo (`uploads/8CBD5356-FF59-44CD-833B-A4779E469937.PNG`) is in the header and footer.
All real details are in place: phone, email, hours, service area, offers, insurance,
two real reviews, owner portrait, three real before/after pairs. No [CHECK] markers left.

`Brand Directions.dc.html` keeps the five original directions plus the settled one,
for reference.

### To finish on return
1. Confirm the four services are the ones to sell (Residential Windows, Screens & Tracks,
   Hard Water Removal, Storefront Glass).
2. ~~Quote form has no backend~~ — **done.** The form POSTs to FormSubmit
   (`https://formsubmit.co/ajax/contact@greatlakesexteriorcleaning.com`), which forwards
   each request to that inbox. No server or account needed; works on any static host.
   **One activation step:** the first request sent from the live domain triggers a
   confirmation email to that address — click the link in it once and delivery is live.
   The endpoint is a single constant (`QUOTE_ENDPOINT`) in the page's logic block if the
   service ever needs swapping. Success is only shown when the send actually succeeds;
   on failure the visitor gets the phone number and a pre-filled email link.
3. Social / Google Business links: none supplied yet.
4. Optional: vector version of the logo for crisp scaling.
5. **Resize the photos before launch.** The five main photos are unmodified 5712x4284
   (24.5MP) camera files, 4-6 MB each, displayed in containers a few hundred pixels wide.
   Home is ~19 MB of images and Before/After ~24 MB. Every file resolves and is committed,
   so the site works — it just loads very slowly on phones. Resizing the long edge to
   ~1600px at quality 80 cuts each to roughly 200-400 KB with no visible change at the
   sizes used. `uploads/` also holds ~28 MB of unused duplicates
   (`IMG_2681.jpeg`, `IMG_2742.jpeg`, `uploads/attachments/`, unused gallery shots).

Scope stays base website only — no login, admin, database or payments.

## Confirmed business details (from owner's business card)

- Business name: **Great Lakes Exterior Cleaning** (legal/brand name kept; services are window cleaning only)
- Owner/Operator: **Logan Mucha**
- Location: Buffalo, NY
- Phone: **716-218-0749**
- Email: **contact@greatlakesexteriorcleaning.com**
- Website: **greatlakesexteriorcleaning.com**
- Logo: house + wand mark, navy/green/blue — matches the chosen palette. Vector file still needed.

## Confirmed insurance (ACORD certificate, dated 08/20/2026)

- Insured: **Logan Mucha dba Great Lakes Exterior Cleaning**, 33 Carlyle Ave, Buffalo, NY 14220
- Carrier: **Utica First** (NAIC 15326), via Progressive Advantage Agency
- Commercial General Liability, occurrence form — effective **08/21/2026**
- Each occurrence **$1,000,000** · General aggregate **$2,000,000** · Products/comp-op agg $2,000,000
- Damage to rented premises $100,000 · Med exp $5,000 · Personal & adv injury $1,000,000
- No auto, umbrella, or workers' comp coverage listed on the certificate
- Policy number is on file but deliberately **not published** on the site

Street address (33 Carlyle Ave) is **personal — never publish**. Sole proprietorship — no separate license or company number exists, none displayed.
Policy number stays off the site (available on request). Still [CHECK]:
opening hours, social links, service-area list, real reviews and rating.

Status: **paused before design-system build.** Directions explored and one settled.
Nothing to build until real photos, insurance details, service availability, and
remaining business details arrive.

## Scope — window cleaning only

Reset Aug 22, 2026: the business is a **window cleaning company only**. No soft washing,
pressure washing, or gutter work anywhere on the site.

Services shown: Residential Windows · Screens & Tracks · Hard Water Removal · Storefront Glass.
**[CHECK]** confirm this four-service list. Name and domain resolved: Great Lakes Exterior Cleaning / greatlakesexteriorcleaning.com.

Before/after emphasis moved from trim, edging and downspouts to **corners, sills and tracks**.

Directions 1–5 in `Brand Directions.dc.html` are kept as a historical record and still
carry the old exterior-cleaning copy. Only the settled direction was rescoped.

## Settled direction — CONFIRMED by owner Aug 22, 2026

"Ledger — refined palette" (top section of `Brand Directions.dc.html`).
Origin: Ledger & Trust layout + Porch Light typography feel, then revised twice by the owner.

- Layout: Ledger & Trust — ruled, structured grid; hairline dividers; bordered
  sections instead of shadows; even, gallery-like photo rhythm.
- Corners: sharp (2px). Shadows: none — borders do the work.
- Density: structured but not cramped; photography given even spacing.

## Type

- Display / headings: **Manrope** (bold modern sans — replaced the earlier Lora serif;
  owner: the serif read "landscaping magazine", logo is bold and modern).
- Body: **Karla**.

## Palette

| Role | Hex |
| --- | --- |
| Background (warm white, from Porch Light) | `#FBF6EE` |
| Primary navy | `#16365E` |
| Lake blue — links, small accents, water-related | `#0785C1` |
| Green — CTA highlights, checkmarks, small accents | `#4F9B2E` |
| White — service cards, quote forms, before/after containers | `#FFFFFF` |
| Rule / border neutral | `#E2E5DE` |
| Body text | `#25303B` |
| Secondary text | `#4A5158` |

Owner-supplied reference values were `#F7F8F5` background and `#082B5C` / `#4C9A2A`;
current file carries the warm-white background plus the slightly adjusted navy/green
above. **[CHECK]** on resume: confirm whether to hold current values or snap navy/green
back to `#082B5C` / `#4C9A2A`.

## Files

- `Brand Directions.dc.html` — five original directions plus the settled direction at
  the top. Preserved as-is; do not overwrite when the build resumes.
- `uploads/Great-Lakes-Exterior-Cleaning-Brand-Essence-Brief (1).md` — source brief.

## Still needed from the owner before building

1. Real before/after photos (close-up: corners, sills, tracks — not wide shots).
2. Photos of the owner working, and the crew.
3. Final insurance / licensing wording and any license or company number.
4. Final window-cleaning service list and availability (residential only, or storefront routes too).
5. Phone, email, address or service-area wording, opening hours, social links.
6. Pages wanted (proposed set: Home, Services, Before/After, About, Reviews,
   Service Area, Contact + quote request, FAQ).
7. Anything that must appear, anything that must not, and any offers, guarantees
   or prices to show.

## On resume

Interview in short batches on the seven items above (defaults suggested, skippable),
then build the full design system from the settled direction: type scale, spacing
scale, components with all states, and every page with real details. Mark anything
skipped `[CHECK]`.

Scope: base website only — no login, no admin panel, no database, no payments.
