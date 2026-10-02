# MODMASE Website

Static website for https://modmase.vercel.app — plain HTML/CSS/JS, no build step.

## Deploy on Vercel (free)
1. Upload this folder to a GitHub repo.
2. Vercel → **Add New → Project** → import the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Deploy.

## Google Search Console
1. Open https://search.google.com/search-console → **Add property** → **URL prefix** → `https://modmase.vercel.app/`
2. Choose **HTML tag** verification, copy the `content="..."` value.
3. In `index.html`, find the commented `google-site-verification` meta tag, paste your code, remove the comment markers (`<!--` and `-->`). Redeploy, then click **Verify**.
4. **Sitemaps** → submit `sitemap.xml`.
5. **URL Inspection** → paste `https://modmase.vercel.app/` → **Request indexing**.

## Files
- `index.html`, `privacy.html`, `404.html` — pages (title, description, canonical, Open Graph, Twitter cards, JSON-LD)
- `sitemap.xml`, `robots.txt`, `site.webmanifest`, `vercel.json`
- `favicon.ico`, `favicon-*.png`, `apple-touch-icon.png`, `android-chrome-*.png`
- `assets/` — CSS, JS, fonts (Poppins, Pacifico), images (logo, banner, `og-image.jpg`)

## Updating
If you add a page, add it to `sitemap.xml`. Update the `lastmod` date when content changes.
