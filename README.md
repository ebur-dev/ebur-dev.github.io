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
4. Update `og:image` in `index.html` to the new address.

The old `ebur-dev.github.io` address then redirects to the new domain.

## Licence

MIT, see [LICENSE](LICENSE).
