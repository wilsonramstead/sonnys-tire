# Sonny's Tire & Automotive — Demo Site

Single-page demo built for **Sonny's Tire & Automotive**, a tire, auto-repair, and
automotive-A/C shop at 5906 Gornto Lake Rd, Riverview, FL 33578 (4.6★ / 202 Google
reviews). The business currently has no website.

**Live demo URL (GitHub Pages):** https://wilsonramstead.github.io/sonnys-tire/

## Pitch angle

**"The A/C rescue crew of Riverview."** In the Tampa Bay summer a dead A/C turns a car
undriveable fast — the site leans into the real reviewer line *"gratefully freezing in my
car in 100 degree weather."* Positioning: fast leak diagnosis (not just a refrigerant
top-off), same-day turnarounds, extended-warranty work handled (e.g. Endurance), and totals
that keep coming in below other shops' quotes. Voice is warm and personable — a front
counter that talks to you (with a light, organic Batman-banter nod) — using **team framing**,
not an owner shrine. Staff named once each, straight from reviews: **Jason** (honest quotes
at the counter) and **Stephanie** (keeps customers updated).

## Contact (used throughout the site)

- **Phone / text:** (813) 626-4556 → `tel:+18136264556` / `sms:+18136264556`
- **Address:** 5906 Gornto Lake Rd, Riverview, FL 33578
- No email, hours, licenses, founding year, or 24/7 claim are published — none were
  verified, so nothing was invented. Phone/text is the only CTA (no contact form).

## Reviews featured (real Google reviewers)

- **Ronald Maupin** (5★) — 2019 Jeep A/C fixed on his extended warranty, done exactly when
  promised — *"gratefully freezing in my car in 100 degree weather."*
- **Taylor Bryant** (5★) — always hesitant about mechanics; Jason's team is *"not the type
  to bs you or waste your time and money."*
- **melmel** (5★) — Stephanie kept her updated the whole process, same-day turnaround, total
  *"well below the other quotes."*

## Design

- **Fonts:** Mitr (display) + Anaheim (body) — Google Fonts. Pre-assigned and grep-verified
  unused across all existing demos before build.
- **Palette — "Riverview Frost":** cool frost-white base (`#eef4fb`), glacier navy-teal ink
  (`#0b2531` / `#0e2c3a`), periwinkle-azure primary (`#3f83f0`, deep fill `#2559c9`, soft
  `#86b6f7`), and a sparing warm heat-relief coral (`#f5744e`) representing the 100° heat the
  A/C rescues you from. Gold review stars (`#ffc94d`). Every hex confirmed globally unused.
  Deliberately distinct from the other cool/climate demos — clearly separated from Custom Air
  (sky ice-blue `#39b0e5` + heat-orange), Andrews (glacier-teal `#17b3aa`), Metron (cyan
  `#22c1e0`), Skamper (spruce/mint), and TJ Tire (deep pine-teal). The icy periwinkle-on-navy
  reads as its own identity vs. the crowded cyan/teal lane.
- Single self-contained `index.html`, inline CSS + minimal vanilla JS, works from `file://`
  and with JS disabled. IntersectionObserver fade-ins respect `prefers-reduced-motion`.
- Mobile guardrails: `overflow-x:clip` on `html,body`, brand name wraps ≤560px under the call
  button, longhand vertical padding on containers, `min-width:0` on grid/flex children,
  `overflow-wrap:break-word`. Sticky-header call button carries click-to-call — **no fixed
  bottom call bar.**
- Semantic HTML, alt text, AA contrast, visible focus states, lazy-loaded below-fold images.
- `AutoRepair` LocalBusiness JSON-LD with `aggregateRating` 4.6 / 202 and the three reviews.
- `og:title` / `og:description` / `og:url` (Pages URL) + **absolute** `og:image` +
  `twitter:card` summary_large_image for iMessage/social link previews.
- `noindex` while it is a demo (remove the meta + the `<!-- DEMO -->` comment when the site
  goes live).

## Imagery

Unsplash only, each verified HTTP 200, viewed for topical fit, and confirmed globally unique
across all `websites/*/index.html` (no photo-ID reuse — re-checked against the concurrent
tire builds too):

- Hero / og:image — `photo-1750568051513-0107108c0bb6` (car A/C climate dials set to max cool —
  directly on the "freezing in your car" angle)
- A/C rescue band — `photo-1554475130-b9114b7e0aac` (steering wheel / dash in warm evening
  light — the "back on the road, cool again" feel)
- Tires showcase — `photo-1664263763412-e22fb3c8af93` (gloved technician mounting a tire onto
  an alloy wheel)

Tire/auto stock is heavily reused across Unsplash and the tread/tire-wall shots collided with
concurrent builds; the final three are all clean. Stock imagery is a placeholder — swap in
real photos of the shop after the sale.

## Domain

`sonnystire.com` is **available** (~$11/yr) — a clean, brandable match if Sonny's wants its
own domain. Otherwise the site runs on the GitHub Pages URL above.

---

Website by [Wilson Innovations](https://wilsoninnovations.net).
