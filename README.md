# chrisclarkcio.clarkfamilyusa.com

Premium CIO / Chief AI Officer personal site for Chris Clark. Static, single page, no build step.

## Files
- `index.html` — the full site (self-contained HTML and CSS)
- `CNAME` — custom domain (`chrisclarkcio.clarkfamilyusa.com`)
- `.nojekyll` — tells GitHub Pages to serve files as-is
- `assets/` — downloadable PDFs linked from the Recruiter Toolkit
  - `Chris-Clark-CIO-CAIO-Resume.pdf`
  - `Chris-Clark-Intro-Slide.pdf`
  - `Chris-Clark-Executive-Journey.pdf`
  - `Chris-Clark-References.pdf`
  - `Chris-Clark-Executive-2Pager.pdf`
- `assets/headshot.jpg` *(optional)* — drop a square photo here and the hero swaps the monogram for the photo automatically. No code change needed.

## Deploy to GitHub Pages
1. Create a new repository (suggested name: `chrisclarkcio`).
2. Upload the contents of this folder to the repo root.
3. Repo **Settings → Pages**: Source = `Deploy from a branch`, Branch = `main` / `/root`.
4. Under **Custom domain**, enter `chrisclarkcio.clarkfamilyusa.com` and Save. (The `CNAME` file already sets this.)
5. Tick **Enforce HTTPS** once the certificate is issued.

## DNS (do this at your domain host for clarkfamilyusa.com)
Add one record:

| Type  | Host / Name      | Value                     |
|-------|------------------|---------------------------|
| CNAME | `chrisclarkcio`  | `<your-github-username>.github.io` |

This mirrors how `chrisclarkresume` already points to GitHub Pages. DNS can take a few minutes to a few hours to propagate; GitHub then issues the HTTPS certificate automatically.

## Updating the résumé or collateral
Replace the matching PDF in `assets/` (keep the filename) and re-upload. The site links by filename, so nothing else changes.
