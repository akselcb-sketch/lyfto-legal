# lyfto-legal

Privacy Policy and Terms of Service for the Lyfto iOS / Android app.

## Hosting

Served via GitHub Pages. After the first push:

1. Repo Settings → Pages → Source = `main` branch, `/ (root)` folder
2. URL becomes `https://akselcb-sketch.github.io/lyfto-legal/`
3. Pages: `/privacy.html`, `/terms.html`

## Custom domain (later)

When `lyfto.app` is purchased:

1. Repo Settings → Pages → Custom domain → `lyfto.app`
2. Add DNS records at the registrar:
   - `A` records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Or `CNAME` `akselcb-sketch.github.io`
3. Tick "Enforce HTTPS" once DNS resolves

`constants/legal.ts` in the main app already references `https://lyfto.app/privacy` + `/terms`, so once the custom domain is wired no client change is needed.

## Updating

Edit the HTML directly. Bump the "Last updated" date at the top of each policy. Push — Pages auto-deploys in ~30 seconds.
