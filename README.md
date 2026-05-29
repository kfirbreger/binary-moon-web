# binarymoon.app — site

Static marketing site for [Binary Moon](https://binarymoon.app), the iOS ambient instrument app.

## Files

- `index.html` — landing page
- `privacy.html` — privacy policy (linked from App Store listing)
- `terms.html` — terms of service
- `styles.css` — design tokens + layout (direct port of `Binary Moon/UI/Theme.swift`)
- `assets/` — screenshots, App Store badge, favicon (see `assets/README.md`)

## Preview locally

No build step. Open `index.html` directly, or serve it:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy — Cloudflare Pages

This repo deploys to https://binarymoon.app via Cloudflare Pages.

- **Build command:** *(empty)*
- **Output directory:** `/`
- **Production branch:** `main`

Every push to `main` triggers a redeploy (~30 sec).
