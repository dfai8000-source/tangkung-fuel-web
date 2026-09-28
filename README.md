# ตังคุง Daily — Fuel Meter web
Static page for the ตังคุง fuel-price meter. Every evening the backend
pipeline (`evening_post.sh`) regenerates `latest/` and pushes; Vercel
redeploys automatically.

- `index.html` — mobile-first page: post image + caption + copy button
- `latest/post.png` — today's 1080x1080 post image
- `latest/caption.txt` — today's caption (Thai)
- `latest/meta.json` — scenario, prices, signal values
- `assets/coiny.png` — ตังคุง mascot

No build step. Deploy: import this repo in Vercel as a static site.
