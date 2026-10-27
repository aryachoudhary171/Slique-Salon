# [Salon Name] — premium salon demo

A responsive, animated, multi-page salon website demo for a Pune salon. Built with plain HTML, CSS and JavaScript so it runs without a build step or dependencies.

## Run locally

1. Edit `config.js` to update the salon name, contact details, social links, services, prices, stylists, theme colors and image paths.
2. From this folder, start a local static server:

   ```bash
   python3 -m http.server 8080
   ```

3. Open <http://localhost:8080>.

You can also open `index.html` directly, though a local server is recommended for browser APIs and consistent routing.

## Pages

- Home: animated hero, service preview, counters, team, draggable before/after, reviews, gallery and offers.
- Services: category tabs, INR pricing, durations, descriptions and direct booking links; package cards.
- Booking: multi-service selection, stylist, date/time, notes, browser validation, localStorage demo persistence and pre-filled WhatsApp handoff.
- Gallery: category filters and accessible lightbox; add real YouTube, Vimeo or Instagram embed URLs in `config.js` (poster/social-link placeholders show until you add them).
- About: story, milestones and team.
- Offers: seasonal promotions, referral idea and membership tiers.
- Contact: phone, email, hours, map placeholder, social links and locally stored demo contact messages.
- Beauty notes: sample blog cards and FAQ accordion.

## Customize before launch

- **Salon details and prices:** `config.js` is the single source of truth for business details and service menu.
- **Photos:** replace the image paths in `config.js` (the files live in `assets/images/`). Images are included for offline demo use.
- **Map:** update the Google Maps query in `app.js` to the precise address or embed URL.
- **WhatsApp:** set `whatsapp` in `config.js` to the international country-code + phone number, digits only.
- **Colors and identity:** adjust CSS variables at the top of `styles.css`; update the simple S brand mark in `index.html`/`app.js` as desired.
- **Real booking:** booking and contact submissions are stored only in the visitor's browser and do not notify staff. Connect a booking API or backend before production.
- **Reviews, team and offers:** replace all illustrative content with approved salon details. The Google rating badge, stories, sample reviews, team details, offer terms and memberships in this demo are fictional placeholders.

## Notes

- Hash-based routes make this demo work as a static site: `#home`, `#services`, `#booking`, `#gallery`, `#about`, `#offers`, `#contact`, `#journal`.
- Motion respects reduced-motion preferences. No front-end framework or animation package is required.
- Google Fonts are remote assets; use local font files if you need fully offline operation.
