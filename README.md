# Jubair Ahamed — Portfolio

A single-page, panel-based portfolio site (no build tools required — just one `index.html` file).

## Deploy with GitHub Pages

1. Create a new repository on GitHub (e.g. `jubairahamedgenz/portfolio`).
2. Add `index.html` and `resume.pdf` to the root of the repo (`index.html` must be named exactly that; `resume.pdf` is linked from the "Download Resume" button on the site, so keep that filename too).
3. Commit and push:
   ```bash
   git init
   git add index.html resume.pdf
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/jubairahamedgenz/portfolio.git
   git push -u origin main
   ```
4. On GitHub: go to **Settings → Pages**.
5. Under **Source**, choose the `main` branch and `/ (root)` folder, then **Save**.
6. GitHub will publish the site at:
   ```
   https://jubairahamedgenz.github.io/portfolio/
   ```
   (First deploy can take a minute or two.)

## Custom domain (optional)

If you want it at `jubairahamed.com` instead:
1. Add a file named `CNAME` (no extension) to the repo root containing just:
   ```
   jubairahamed.com
   ```
2. At your domain registrar, point an `A` record to GitHub's Pages IPs, or a `CNAME` record to `jubairahamedgenz.github.io`.
3. Enable "Enforce HTTPS" in the Pages settings once DNS propagates.

## Notes

- No build step — it's plain HTML/CSS/JS, so any static host (GitHub Pages, Netlify, Vercel) works as-is.
- Fonts load from Google Fonts via CDN, so an internet connection is needed when the page loads.
