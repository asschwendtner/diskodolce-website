# disko dolce — website

Static one-page website for the disko dolce music collective.

## File structure

```
/
├── index.html                        # Main site — everything lives here
├── diskodolce_logo_white_trans.png   # Logo (white, used in nav + hero)
├── diskodolce_logo_red_trans.png     # Logo (red, alternative)
├── Cloud_Dancer.otf                  # Custom display font
├── Cloud_Dancer.ttf                  # Custom display font (fallback)
├── 20250912_Arche_FINALE_VERSION.png # Event photo — Arche Ahoi
├── Copy_of_20260320_-_Hive.png       # Event photo — HIVE Club
├── Schneiderei_Final.png             # Event photo — Schneiderei
└── README.md                         # This file
```

## How to edit

All content lives in `index.html`. Key sections to update:

- **Artist photos** — find each `<div class="tile-bg">` inside `.artist-tile` and replace with:
  ```html
  <div class="tile-photo">
    <img src="your-photo.jpg" alt="Artist Name">
  </div>
  ```
- **Artist social links** — search for each artist name block and update the `href` values on `.tile-link` and `.hover-link` anchors
- **Gigs** — find `<div id="gigs">` and add/remove `.gig-item` blocks
- **Contact info** — find `<div id="contact">` and update email / handles

## How to publish (GitHub Pages)

1. Create a new repo on github.com (e.g. `diskodolce-website`)
2. Upload all files in this folder to the repo root
3. Go to **Settings → Pages → Source** → select `main` branch, `/ (root)`
4. Site goes live at `https://yourusername.github.io/diskodolce-website`

For a custom domain (e.g. `diskodolce.com`):
- Add a `CNAME` file to the repo containing just your domain name
- Point your domain's DNS to GitHub Pages (see GitHub docs)

## Local preview

Just open `index.html` in a browser — no build step needed.
