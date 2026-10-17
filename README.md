This repository contains the entire source code for my website [michaelmassoni.com].

Plain HTML and CSS, deployed with Cloudflare Pages. There is no build step: every file in the repo root is served as-is.

- `_headers`: security headers (CSP, HSTS) applied by Cloudflare Pages. Any new third-party resource must be allowed here.
- `fonts/`: self-hosted JetBrains Mono (SIL Open Font License, see `fonts/OFL.txt`).
- `feed.xml` and `sitemap.xml`: update both when adding a post.
- `.github/workflows/checks.yml`: HTML validation and a link check on every push and weekly.

To validate locally: `npx html-validate '*.html' 'posts/*.html'`
