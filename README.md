# ebur-dev.github.io

The website for [Ebur](https://github.com/ebur-dev/ebur), served by GitHub
Pages at https://ebur-dev.github.io.

Plain HTML and CSS: no build step, no JavaScript, no trackers, and no
third-party requests (fonts are served from this repository). Edit
`index.html` or `style.css` and push to `main`; GitHub Pages publishes
within a minute.

- `assets/`: logo and screenshots (copied from the Ebur repo's
  `docs/screenshots/`).
- `fonts/`: Inter and JetBrains Mono, under the SIL Open Font License
  (texts alongside).
- `.nojekyll`: serve the files as they are.

## Moving to a custom domain

When the domain is bought (for example `ebur.dev`):

1. In this repository's **Settings > Pages**, enter the domain under
   **Custom domain** (GitHub adds a `CNAME` file).
2. At the domain registrar, point the apex domain at GitHub Pages with A
   records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and
   `185.199.111.153` (and AAAA records if wanted), and `www` with a CNAME
   to `ebur-dev.github.io`.
3. Once the check passes, tick **Enforce HTTPS**.
4. Replace `https://ebur-dev.github.io/` with the new address everywhere it
   appears: `index.html` (canonical, Open Graph, Twitter and JSON-LD
   tags), `robots.txt` and `sitemap.xml`. The canonical tag is what moves
   search ranking to the new domain.

## Search engines

- `robots.txt` and `sitemap.xml` tell crawlers what to index.
- `index.html` carries a canonical URL, Open Graph and Twitter card tags
  (preview image `assets/og.png`, 1200x630) and a schema.org
  `SoftwareApplication` block.
- Register the site in [Google Search Console](https://search.google.com/search-console)
  and [Bing Webmaster Tools](https://www.bing.com/webmasters), and submit
  the sitemap there.
- Bump `<lastmod>` in `sitemap.xml` when the page changes meaningfully.

The old `ebur-dev.github.io` address then redirects to the new domain.

## Licence

MIT, see [LICENSE](LICENSE).
