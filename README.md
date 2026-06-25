# SCB Consulting

Single-page website for **SCB Consulting** — strategic brand & retail consultancy.

## Structure

- `index.html` — the entire site (one page, no build step)
- `images/` — campaign photography used in the galleries

## Preview locally

It's a static site. Either open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Works on any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages). Point it at the repo root — `index.html` is the entry point. Fonts load from Google Fonts; nothing to compile.

## Editing

- Collaborations are grouped into three acts in `index.html`: **Retail · In-Store Activations**, **Brand Collaborations**, **Experiential Marketing / Pop-Ups**.
- To add images to a collaboration, drop the file in `images/` and add an `<img>` to that collaboration's `.gallery` block. Add `class="wide"` to make a tile span two columns.
