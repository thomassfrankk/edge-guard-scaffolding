# Edge Guard & Scaffolding — Website

Static marketing landing page for Edge Guard & Scaffolding (EGS), a Brisbane-based edge protection & scaffolding business.

## Stack

Plain HTML/CSS/JS, no build step. Designed to host on [Netlify](https://netlify.com) (free tier) with auto-deploy on push to `main`.

## Structure

- `index.html` — the landing page (single page, no subpages)
- `success.html` — Netlify Forms redirect target after a quote enquiry is submitted
- `privacy.html`, `terms.html` — legal pages (placeholder drafts, need a legal review + real details before launch)
- `images/` — logo and hero photo
- `robots.txt`, `sitemap.xml` — SEO basics
- `netlify.toml` — Netlify build/publish config (safe to ignore if not using Netlify)

## Before launch — replace placeholders

- Phone: `0400 000 000`, Email: `info@edgeguardscaffolding.com.au`, ABN: `00 000 000 000` (in `index.html`, `success.html`, footer, and the JSON-LD schema)
- Google Ads conversion tracking ID `AW-XXXXXXXXX` (in `index.html` and `success.html`) and the conversion label on `success.html`
- Testimonials (currently 3 generic placeholders)
- Domain used in the JSON-LD schema and `sitemap.xml`/`robots.txt` (currently `edgeguardscaffolding.com.au`)
- Fill in `[DATE]`, `[ABN]`, `[PHONE]` in `privacy.html` / `terms.html` and get them reviewed
- Add real social links to the footer once available

## Local preview

Just open `index.html` in a browser, or run a quick local server:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
