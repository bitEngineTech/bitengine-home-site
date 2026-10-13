# home.bitengine.tech

Landing page for bitEngine Hub. Plain HTML, no build step; served by GitHub Pages.

## Files

- `index.html` — the page
- `images/hub-front.jpg` — product photo (replace with a clean-background shot when you have one; keep the file name or update the `<img>` and `og:image`)
- `images/architecture.png` — block diagram
- `CNAME` — custom domain for GitHub Pages

## Before going live

1. In `index.html`, replace `YOUR_BUTTONDOWN_USERNAME` with your Buttondown username.
2. ~~Discussion thread link~~ (done)

## Deploy

1. Create a public repo in your GitHub org, e.g. `bitengine-home-site`, and push these files to `main`.
2. Repo **Settings → Pages**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`.
3. Custom domain: `home.bitengine.tech`. Once the DNS check passes, tick **Enforce HTTPS**.
4. At your DNS provider for `bitengine.tech`, add one record and leave the main site's records untouched:

   | Type  | Name | Value                      |
   |-------|------|----------------------------|
   | CNAME | home | `<your-github-org>.github.io` |
