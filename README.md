# Ben Patalano — Resume Website

A clean, fast, responsive resume site built as a static single-page site, optimized for Cloudflare Pages.

## What's Included

```
├── index.html          ← Main resume page (all CSS inline, zero JS dependencies)
├── robots.txt          ← SEO: tells search engines to index everything
├── sitemap.xml         ← SEO: sitemap for search engines
├── _headers            ← Cloudflare Pages: security headers + PDF download header
├── _redirects          ← Cloudflare Pages: /resume → PDF shortcut
├── 404.html            ← Custom 404 page
└── Ben_Patalano_-_Senior_Software_Engineer_-_2025.pdf  ← Downloadable resume
```

## Customization

- **Canonical URL:** `index.html` has `<link rel="canonical" href="https://benpatalano.com/">` — update if using a different domain.
- **Open Graph URL:** Same for the `og:url` meta tag.
- **Sitemap:** Update the domain in `sitemap.xml` to match.
- **Resume PDF:** Replace the PDF file and redeploy.
- **Short URL:** `/resume` redirects to the PDF via `_redirects`.

## SEO

- Semantic HTML5 with proper heading hierarchy
- JSON-LD structured data (Person schema)
- Open Graph and Twitter Card meta tags
- Canonical URL
- robots.txt with sitemap reference
- XML sitemap
- Descriptive title and meta description
- `aria-label` attributes for accessibility
- Print stylesheet included

## Performance

- Zero JavaScript dependencies (pure HTML + CSS)
- All CSS inlined (no render-blocking resources)
- Only external request: Google Fonts (preconnected)
- Cloudflare's edge network handles caching and CDN
- Typical Lighthouse score: 95-100 across all categories
