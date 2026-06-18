# Whollar

Landing page for **Whollar** — wholesale buying power on home internet. Hundreds of households join one sealed bidding round; providers compete to serve the whole group.

A single self-contained `whollar-landing.html` (inline CSS + vanilla JS, no build step) plus optimized media assets.

## Run it

Open `whollar-landing.html` directly in a browser, or serve the folder:

```bash
python -m http.server 8000
# then visit http://localhost:8000/whollar-landing.html
```

## Structure

- `whollar-landing.html` — the entire page (markup, styles, scripts)
- `images/` — optimized photos (JPG + WebP, served via `<picture>`)
- `can_you_make_this_darker_pleas.mp4` — hero background video
- `whollar-hero-poster.jpg` — hero video poster / fallback

## Notes

- Responsive, with a mobile hamburger nav below 880px.
- Respects `prefers-reduced-motion` (background video and animations pause).
- Brand tokens, type scale, and elevation system are defined as CSS variables in `:root`.
