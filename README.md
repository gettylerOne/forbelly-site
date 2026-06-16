# ForBelly — Homepage

Marketing homepage for **ForBelly**, a belly-friendly psyllium prebiotic fiber drink.

A self-contained static site — no build step. Open `index.html` in any browser, or deploy as-is.

## Structure

```
index.html            The full desktop homepage (inline CSS + JS)
mobile-preview.html   390px mobile preview of the homepage (forced mobile layout)
assets/               Product imagery
uploads/              Hero, logo, lifestyle, and founder images
```

`mobile-preview.html` is a standalone preview that forces the homepage into a centered
390px column with the mobile layout always on — handy for reviewing the phone view on a
desktop screen. It's kept separate from `index.html`; desktop changes don't affect it.

## Deploy on Netlify

This repo is set up to deploy with **zero configuration**:

1. In Netlify, **Add new site → Import an existing project** and connect this GitHub repo.
2. Leave **Build command** empty and **Publish directory** as `.` (the repo root).
3. Deploy — Netlify serves `index.html` directly.

## Features

Interactive pricing (subscribe vs. one-time, quantity stepper, live totals), a slide-out
cart with free-shipping progress (persisted in `localStorage`), a sticky buy bar, an
exit-intent discount modal, an FAQ accordion, and scroll-reveal animations.
