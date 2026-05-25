# Law Office of Joseph D. Grisanti — Site Preview

A redesign of [jgrisantilaw.com](https://www.jgrisantilaw.com/), built as a static site so it can be hosted free on GitHub Pages.

Single-page site. Two files do all the work: `index.html` and `styles.css`. No build step, no framework, no dependencies — just open `index.html` in a browser.

---

## What's here

- **Editorial / noir aesthetic** — midnight navy + brass, serif headlines (Fraunces) + clean sans body (Manrope)
- **Hero leads with Joe's actual differentiator** — FBI + Prosecutor + Licensed PI, not buried in paragraph 3
- **Click-to-call everywhere** — header, hero, contact, floating mobile button. Phone is the primary CTA per criminal-defense best practices.
- **Four practice area cards** — Municipal/DWI, Real Estate, Wills & Estates, Personal Injury — each with sub-services pulled from the existing site copy
- **"The Grisanti Difference" section** — three editorial blocks (FBI / DA / PI) that explain *why* three perspectives change outcomes
- **Process section** — 3 steps from first call to resolution
- **FAQ accordion** — six common questions covering all practice areas
- **Embedded Google map** + click-for-directions
- **NJ Bar-compliant footer** — "Attorney Advertising," "Prior results do not guarantee a similar outcome," no claims that violate RPC 7.1
- **Mobile-first responsive**, dark sticky header, smooth scroll, fade-in reveal animations
- **Performance**: ~25KB HTML + ~15KB CSS, two fonts from Google CDN, no JS framework

---

## Deploy to GitHub Pages

1. Create a new public repo (e.g. `grisanti-preview`).
2. Drop `index.html` and `styles.css` into the root.
3. In the repo: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. GitHub will give you a URL like `https://<your-username>.github.io/grisanti-preview/` in 1–2 minutes.
5. Send that to Joe.

If he wants the real domain later (`jgrisantilaw.com`), it's the same flow as your other site: add a `CNAME` file with `www.jgrisantilaw.com`, and point the DNS A records at GitHub's IPs.

---

## What I made up vs. what's from the existing site

Joe should review and correct anything off — I worked only from his current site.

**From his existing site (verified):**
- Name, address, phone, fax
- "Former FBI agent and prosecutor"
- "Licensed private investigator for the State of New Jersey"
- "30 years of experience"
- All four practice areas and their descriptions
- "Free initial consultations"
- "No fee if there is no recovery" (personal injury)

**Inferred / added (he should confirm or change):**
- Tagline "Established 1995" — math from "30 years," may be off by a year or two
- Service area cities (Toms River, Lakewood, etc.) — assumed based on Brick location in Ocean County
- Email `office@jgrisantilaw.com` in the contact form — placeholder, change to his actual email
- "By appointment. Free, on-site parking." — guess; tell me if wrong
- Educational FAQ content — written from general NJ law knowledge; Joe should review for anything he'd phrase differently

**Not included (no info on existing site, would need from Joe):**
- Headshot — high-impact addition; should be a professional photo, ideally B&W or muted to match aesthetic
- Specific bar admissions, year admitted, law school
- Office hours
- Testimonials (intentionally omitted — fake testimonials violate NJ RPC 7.1; need real reviews with client consent)

---

## Easy edits

- **Phone number** — search-replace `732-534-9005` in `index.html`
- **Address** — search the address string in `index.html` and the map iframe `src`
- **Color palette** — top of `styles.css`, the `:root` block. `--brass` and `--ink` are the two main levers.
- **Add a headshot** — drop a photo at the top of the About section; the layout already reserves the left column with a sticky tag.

---

Built with Claude, May 2026.
