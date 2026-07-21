# Stilence.com Website

Professional one-page site for your Airbnb walkthrough video service.

## What's here

- `index.html` — the entire website (all styling and interactivity is built in, no other files needed)
- `videos/` — drop your 8 teaser clips here

## Adding your teaser videos

Name your watermarked 15-second clips exactly like this and put them in the `videos` folder:

```
videos/teaser-01.mp4
videos/teaser-02.mp4
...
videos/teaser-08.mp4
```

They'll appear automatically in the showcase grid — hover plays them on desktop, tap plays on phones. Until a file exists, that slot shows a "Teaser coming soon" placeholder, so the site looks fine even before all 8 are ready.

**Tips:**
- Vertical (9:16) clips look best — the grid is built for that shape (like Reels/TikTok).
- Keep each clip under ~10 MB so the page loads fast. Export at 720×1280, H.264.
- The clip titles ("Modern Loft", "Lakehouse Retreat"...) are in `index.html` — search for `class="label"` and rename them to match your actual projects.

## Putting it live on stilence.com

Where you deploy depends on where stilence.com's DNS is managed, but the upload itself is just these files. Easiest options:

1. **Netlify (free):** drag the whole `stilence-website` folder onto https://app.netlify.com/drop, then point stilence.com at it (Netlify shows you the DNS records to add at your domain registrar).
2. **Your registrar's hosting:** if you bought hosting with the domain (GoDaddy, Namecheap, etc.), upload `index.html` and the `videos` folder to the site root via their file manager.

## Changing things later

- **Phone number:** search `index.html` for `848-221-7216` and `+18482217216` (the second is the tap-to-call/text link format).
- **Colors:** the gold accent is `--accent: #e8b45a;` near the top of the file — change that one line to re-theme the whole site.
