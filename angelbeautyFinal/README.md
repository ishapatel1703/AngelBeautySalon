# Angel Beauty Salon

A five-page, dependency-free static website built with semantic HTML, CSS and JavaScript. Its pages are Home (`/`), Services (`/services/`), Gallery (`/gallery/`), Contact us (`/contact/`) and Book Appointment (`/book-appointment/`). Shared responsive navigation includes a Book Appointment button on every page.

## Run and build

Use Node.js 20 or later. Start the preview with `npm run dev`; it listens on port 3000 by default, and accepts a custom port through `PORT`. Run `npm run build` to copy the full static site into `dist/`.

## Automatic service sliders

The home page shows a separate, seamless image slider for each of the nine services. Neighboring rows move in opposite directions. Use the pause/resume control to stop or restart every row; the sliders respect the device’s reduced-motion preference.

## Salon photos

The supplied salon photos are optimized WebP files in `public/images/`. The Gallery page displays all 64 photos; each service on Services automatically cycles through three or four service-specific photos. Home gives every service its own animated strip. Keep meaningful `alt` text when replacing photos.

## Contact and bookings

The Contact and Book Appointment forms are front-end demos: they validate fields but do not send or store visitor details. WhatsApp chat is linked to +91 79999 24521. The salon street address and opening hours were not supplied, so visitors can ask for them over WhatsApp instead of seeing invented details.

## Project files

- `public/index.html` — Home page and nine individual alternating-direction service sliders.
- `public/services/index.html` — nine-service catalogue.
- `public/gallery/index.html` — salon photo gallery.
- `public/contact/index.html` — contact information placeholders and demo enquiry form.
- `public/book-appointment/index.html` — appointment request form.
- `public/styles.css` and `public/main.js` — shared responsive design and interactions.
- `public/images/` — optimized WebP salon photography supplied for this site.
- `public/manus-routes.json` — declared public page routes.
- `server.mjs` and `scripts/build.mjs` — clean static route preview and build helpers.
