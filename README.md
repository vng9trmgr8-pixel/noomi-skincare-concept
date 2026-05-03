# Noomi Skin Care — Concept Site

A redesigned, marketing-and-SEO-optimized concept for [noomidayspa.com](https://www.noomidayspa.com) — a boutique facial studio on Esplanade in Chico, CA.

## What's here

- `index.html` — single-file static site, Tailwind via CDN, custom CSS for typography and motion.
- LocalBusiness schema (`@type: DaySpa`), `og:` and `twitter:` tags, canonical, descriptive alt text on every image.

## Design notes

Built with the [taste-skill](https://github.com/Leonxlnx/taste-skill) anti-slop frontend rules:

- **Type:** Fraunces (display) + Geist (body) — no Inter.
- **Palette:** warm cream `#FAF6F0`, off-black `#1C1714`, single terracotta accent `#B65D44`. No purple, no neon glows.
- **Layout:** asymmetric 12-col grid, zig-zag sections, no 3-equal-card rows.
- **Motion:** CSS-only reveal-on-scroll via IntersectionObserver, marquee announce strip, tactile button press.
- **Hero:** `min-h-[100dvh]` (no `h-screen` mobile bug), 7/5 text-image split.
- **Performance:** grain effect on a fixed pseudo, animations on `transform`/`opacity` only.

## Sections

1. Hero — *"Custom facials, built around your skin."*
2. Service marquee — keyword-rich, scrolling
3. About Carla — zig-zag with editorial pull-quote
4. Treatments — divided list with prices and durations
5. The Veranda — full-bleed editorial spread (the unique group-booking patio)
6. Testimonials — paired editorial pull-quotes, no card chrome
7. Products — PCA Skin / Cosmedix / Sorella Apothecary
8. Visit / final CTA — booking + hours + address

## Run locally

```bash
# any static server works
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Auto-deploys on push to Vercel (see preview link in PR / repo description).

## SEO meta

- Title: `Custom Facials in Chico, CA | Noomi Skin Care on Esplanade`
- Description: `Custom facials, chemical peels and dermaplane in Chico, CA by Carla — 10+ years experience. Group bookings on The Veranda patio. Book online or call 530-514-0632.`

## Photo credits

Images are referenced from Noomi's existing Squarespace CDN for the concept preview. Replace with originals before production.
