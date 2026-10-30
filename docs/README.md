# Fatih Restaurant — static site (HTML/CSS/vanilla JS)
Run: open `index.html`, or `python3 -m http.server` in this folder.

## Status (honest)
- Built from the reference image; **not rendered or compared in a browser** (no browser available here). Proportions are estimates.
- **No photos included** (no network). Each image slot has a CSS gradient fallback; drop files at the paths below and they appear automatically.
- Simplified structure: one `css/styles.css` (sections marked by comments) and one `js/main.js`, instead of the suggested 13 CSS / 5 JS files.
- Footer skyline is a CSS clip-path silhouette; social icons are text placeholders.

## Images to supply (all currently "needs replacement")
Paths under `assets/images/`; referenced in `css/styles.css` (search the filename, `grep -n webp css/styles.css`). Run that command for exact line numbers; they were not hand-estimated.
hero/istanbul-restaurant-hero.webp · about/ottoman-restaurant-interior.webp · menu/adana-kebab.webp, turkish-pide.webp, kuzu-tandir.webp, baklava.webp · atmosphere/turkish-tea-service.webp · gallery/restaurant-interior.webp, bosphorus-sunset.webp, turkish-tea.webp, ottoman-dining-table.webp · reservation/luxury-dining-table.webp

## Interactions
Hamburger (keyboard + Esc), active-link tracking, smooth scroll, back-to-top, dish modal, gallery lightbox (buttons, arrows, swipe), testimonial scroller, reservation form with validation, newsletter validation.

## Needs backend / replacement
- Reservation: opens a prefilled `mailto:` (set `CFG.reservationEmail` in `js/main.js`). Nothing is stored.
- Newsletter: validates only; nothing is sent.
- "Tanıtım Videomuz": set `CFG.videoUrl`. "Tüm Menü", privacy/terms, social links: placeholders.
- Demo address, phone, email, prices, and **testimonials (fictional)** must be replaced before launch.
- Testimonial 2 text keeps "ilgilydi" from the reference (likely typo for "ilgiliydi"); fix it in `index.html`.
