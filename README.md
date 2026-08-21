# DANILO — Watch Brand Website

A single-page marketing site for DANILO, an original luxury sports-watch concept. Built as one self-contained `index.html` (no build step, no dependencies) with a scroll-scrubbed disassembly animation as the hero.

## Live preview

Open `index.html` directly in any browser, or serve the folder locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Structure

- **Hero / Mechanism** — a video of the watch coming apart, scrubbed frame-by-frame as you scroll (no autoplay, purely scroll-driven).
- **Atelier** — brand origin story with a supporting image.
- **Collection** — four finishes (Steel, Noir, Marine, Reserve), each with a click-to-expand blurb about the finish.
- **Editorial** — two lifestyle shots (on the wrist, in presentation box).
- **CTA + Footer**.

## Notes

- All imagery and video are AI-generated concept assets for this fictional brand, currently hotlinked from their generation host. For a fully self-hosted deployment, download the assets and point the `<img src>` / `<video><source>` tags at local files (e.g. an `/assets` folder) before publishing.
- Fully responsive: desktop, tablet (iPad portrait/landscape), and phone, including a slide-in mobile nav under 760px.
- No frameworks, no build tools — plain HTML/CSS/JS, safe to deploy as a static site (GitHub Pages, Netlify, Vercel, or any static host).

## Deploy

Any static host works since this is a single HTML file:

- **GitHub Pages**: push this repo, then enable Pages on the `main` branch (root) in repo Settings → Pages.
- **Netlify / Vercel**: drag-and-drop this folder, or connect the repo — no build command needed, output directory is `/`.
