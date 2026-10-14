# rightpath.foundation — placeholder site

A single static page for RightPath Foundation stating its pending 501(c) application. No framework, no build step, no JavaScript, no forms, no analytics.

This project is separate from rightpathmethod.com. Do not share code or assets between them.

## Files

| File | Purpose |
|---|---|
| `index.html` | The page (copy, meta tags, Open Graph) |
| `styles.css` | All styling. Colors and fonts are CSS variables at the top of the file |
| `favicon.svg` | Simple "path" icon in brand colors |
| `robots.txt` | Allows crawling, points to the sitemap |
| `sitemap.xml` | One URL |

## Preview locally

Open `index.html` in a browser. That's it.

## Deploy

Upload the five files (everything except this README) to the web root of any static host:

- **Netlify / Cloudflare Pages / Vercel:** drag-and-drop the folder, or connect a repo with no build command and the folder as the publish directory.
- **GitHub Pages:** push to a repo, enable Pages on the main branch root.
- **Traditional hosting (cPanel, S3, etc.):** copy the files into the public root (e.g. `public_html/`).

Then point the `rightpath.foundation` DNS records at the host and enable HTTPS.

## When the 501(c) status changes

The status wording appears in three places in `index.html`. Update all three:

1. The **Organizational Status** card (`<section class="status">`).
2. `<meta name="description">` in the `<head>`.
3. `<meta property="og:description">` in the `<head>`.

Rules until status is formally granted **and** the client confirms the exact wording:

- Do not say "501(c)(3)", "tax-exempt", or "tax-deductible".
- Do not add a donate button, donation form, or fundraising language.

If status is granted, the client should supply the exact designation (e.g. 501(c)(3)), and whether to show an EIN. Only then consider donation language, and have it reviewed.

Also update `<lastmod>` in `sitemap.xml` whenever the page changes.

## Yearly maintenance

The footer year (`© 2026`) is hardcoded because the page has no JavaScript. Update it each January.

## Open items for the client

1. What is the exact current 501(c) status (applied, pending, or granted), and the wording the client prefers?
2. How does the foundation relate to the "RightPath Institute" described on rightpathmethod.com (same entity or separate)?
3. Real contact email (`info@rightpath.foundation` is a **placeholder**), and any logo or branding assets.
4. Who manages DNS and hosting for this domain?
