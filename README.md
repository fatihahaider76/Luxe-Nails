# Luxe Nails Website

A single-page static site for Luxe Nails, a private home nail studio in South Whitby, ON.

## What's in this repo

- `index.html` — the entire site (HTML, CSS, and JS in one file)
- `luxe_logo.png`, `luxe_logo_256.png` — the circular Luxe Nails logo (nav, footer, favicon)
- `*.jpg` — client nail photos used in the hero, about, and gallery sections

No build step, no dependencies. It's plain HTML/CSS/JS plus Google Fonts loaded from a CDN.

## Push to GitHub

```bash
git init
git add .
git commit -m "Luxe Nails website"
git branch -M main
git remote add origin <your-empty-github-repo-url>
git push -u origin main
```

## Deploy on Netlify

1. In Netlify, click **Add new site → Import an existing project** and connect this GitHub repo.
2. Build settings: leave the build command empty and set the **publish directory** to `/` (repo root) — there's nothing to build.
3. Deploy. Then go to **Domain settings** and attach your custom domain.

## Things to double check before going live

- The booking form (`#contact`) opens a pre-filled email to `luxenailsq.co@gmail.com` — confirm that's the right inbox.
- Testimonials in the "What Clients Say" section are placeholders — swap in real reviews when ready.
- Pricing is pulled from the price menu photo provided; update directly in the `Services & Pricing` section of `index.html` if it changes.
