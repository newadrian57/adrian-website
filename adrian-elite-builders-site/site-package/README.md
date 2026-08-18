# Adrian Elite Builders Corporation — Website

Static site. No build step, no dependencies — just `index.html` plus the image files sitting next to it.

## Deploy on GitHub + Vercel

1. Create a new GitHub repository (e.g. `adrian-elite-builders`).
2. Upload every file in this folder to the repo root — keep them all in the same top-level folder, don't put `index.html` in a subfolder while the images stay outside it.
3. Go to vercel.com → **Add New Project** → import that GitHub repo.
4. Framework preset: choose **Other** (this is a plain static site, no build command needed).
5. Click **Deploy**. Vercel will give you a live `.vercel.app` URL immediately.
6. To use your own domain later: Vercel project → **Settings → Domains** → add your domain and follow the DNS steps it gives you.

## Updating the site later

Edit `index.html` directly (in GitHub's web editor or locally), commit, and push — Vercel redeploys automatically on every push to the main branch.

## Notes

- The quote form currently submits via `mailto:`, which isn't fully reliable on all devices/browsers. Swap the form's `action` for a Formspree endpoint when you have one — ask Claude to wire it in.
- NJHIC# 13VH14137500 is displayed in the About section and footer, as required for NJ home improvement advertising.
