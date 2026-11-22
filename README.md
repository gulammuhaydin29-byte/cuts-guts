# Cuts & Guts Fitness Gym — Official Website

A premium, production-quality single-page website for **Cuts & Guts Fitness Gym**, Mian Channu, Pakistan.

Built with **HTML5, CSS3, and Vanilla JavaScript only** — no frameworks, no build step, no dependencies.

---

## Features

- Premium dark fitness identity (electric lime accent, editorial typography)
- Sticky navigation with transparent → solid scroll transition and active link states
- Full-screen hero with subtle entrance animations
- Scroll-reveal animations via `IntersectionObserver`
- Asymmetrical photo gallery with keyboard-accessible lightbox
- WhatsApp membership enquiry + click-to-call + Google Maps directions
- Fully responsive (desktop, tablet, mobile) with intentional mobile layouts
- Respects `prefers-reduced-motion`
- SEO metadata, Open Graph / Twitter cards, and `ExerciseGym` structured data
- Back-to-top button, lazy-loaded images, layout stability

---

## Project Structure

```
cuts-and-guts-website/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── assets/
│   ├── images/        (placeholder JPGs — replace with real gym photos)
│   ├── icons/         (favicon.svg)
│   └── logo/          (logo.svg — replace with the real gym logo)
└── README.md
```

---

## How to Run

No build tools required. Simply open `index.html` in any modern browser.

For the best experience (and to avoid any local-file restrictions with the map embed), serve it locally:

```bash
# Using Python (no install needed)
python -m http.server 8080
# then open http://localhost:8080

# Or using Node
npx serve .
```

---

## Customization

### Replace placeholder assets

The images in `assets/images/` are **generated placeholders**, clearly labeled "REPLACE WITH REAL GYM PHOTO". Replace them with your actual gym photography (keep the same filenames, or update the paths in `index.html`).

- `assets/logo/logo.svg` is a text placeholder wordmark — replace with the real logo if available.
- `assets/icons/favicon.svg` can be swapped for the final brand favicon.

> Never present unrelated stock photos as real photos of this business. The placeholders exist only so the layout is complete and testable.

### Verified business information

| Field   | Value |
|---------|-------|
| Name    | Cuts & Guts Fitness Gym |
| Address | Allama Iqbal Road, near Children Park, Mian Channu, Pakistan |
| Phone   | +92 305 7789129 |
| Maps    | https://www.google.com/maps/place/Cuts+%26+Guts+Fitness+Gym,+Mian+Channu/ |

The phone number is used in `tel:` and `wa.me` links throughout. Update the `wa.me/923057789129` links if the number changes.

### Edit content

All copy, facilities, and training sections live in `index.html`. Facility and training items are **suggested categories** — replace with facilities the gym has actually confirmed.

### Theme colors

Design tokens are at the top of `css/style.css` under `:root`:

```css
--bg: #101010;      /* main background */
--bg-2: #181818;    /* secondary background */
--lime: #d7ff35;    /* primary accent */
--text: #ffffff;    /* main text */
--text-2: #a1a1a1;  /* secondary text */
--border: #303030;  /* borders */
```

### Canonical URL

Update the `<link rel="canonical">`, Open Graph, and `og:url` values in `index.html` with the real production domain.

---

## Notes Before Publishing

- Confirm facilities with the gym before publishing the Facilities section.
- Confirm opening hours before displaying them (currently intentionally omitted).
- Replace all placeholder images and the logo.
- Update the canonical / social URLs with the real domain.
- Verify the Google Maps embed once the site is hosted.

---

## License

© Cuts & Guts Fitness Gym. All rights reserved.