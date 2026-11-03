# FEMBOD Faith Home website

Responsive, multi-page static HTML/CSS/JavaScript website for FEMBOD Faith Home, described by the owner as a clinic.

## Project structure
- `index.html` — homepage
- `about.html` — about and values
- `services.html` — service enquiry information (does not guarantee unconfirmed services)
- `locations.html` — both branches, opening hours and map-search links
- `contact.html` — contact details and directions
- `faq.html` — common visitor questions
- `professional-development.html` — professional development enquiries
- `styles.css`, `script.js` — styling and mobile navigation/year helper
- `assets/` — logos and favicon
- `robots.txt`, `sitemap.xml` — crawl configuration (sitemap needs real URLs before launch)
- `vercel.json` — static hosting security headers

## Preview locally
Open `index.html` in a browser, or run a simple local server from this directory:
`python -m http.server 8000`
Then visit `http://localhost:8000`.

## Vercel deployment
This is a static site. Import the project directory into Vercel or deploy the extracted directory.

- Framework preset: **Other**
- Build command: **Leave empty**
- Install command: **Leave empty**
- Output directory: **`.` (project root)**
- Root directory: the directory containing `index.html`

No package installation or build step is required.

## Before publishing (important)
1. **Confirm branch phone mapping.** The project contains `0703 368 9206` and `0813 780 6991`, but the supplied material does not establish which number belongs to which branch. Both are shown as general contact options on the locations page, not assigned to a branch.
2. Confirm both addresses exactly and verify each Google Maps result/pin. Current directions links are address-based Google Maps searches, not verified pins.
3. Confirm the exact registered business descriptor and any registration details the owner wants published.
4. Confirm the actual services offered at each branch. Do not add unconfirmed services as facts.
5. Confirm the professional-development offering and supervision details before making specific training claims.
6. Confirm the owner approves the personal TikTok link being used as a supporting contact/social link.
7. Replace external Unsplash stock photography with owner-approved clinic photographs when available. Current stock images are external and are not represented as actual FEMBOD premises or staff.
8. Supply the real production domain. Then add canonical tags and Open Graph URLs, populate `sitemap.xml` with absolute production URLs, add a Sitemap directive to `robots.txt`, and add accurate JSON-LD structured data. These are intentionally not fabricated while the domain and final business details are unconfirmed.
9. Confirm the slogan and final brand/logo asset with the owner.

## Current technical notes
- Pure static HTML/CSS/JS; no build process or dependencies.
- `vercel.json` applies basic security headers and does not force a framework build.
- Fonts are loaded from Google Fonts; Unsplash photos require internet access.
- This package has not been deployed. Browser-based visual testing and live Google/schema validation were not available in this environment.
