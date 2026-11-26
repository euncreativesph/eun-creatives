# Eun Creatives — portfolio website

A single page (`index.html`) plus your cut-out portrait (`eunice-cutout.webp`, `eunice-cutout-560.webp`). No build step, no dependencies.

`eunice-cutout.png` is a full-quality transparent copy of your photo for other uses; the site doesn't need it.

## Put it online (Vercel, same as your current video site)
1. In the GitHub repo behind eunstudio.vercel.app (or a new repo), replace the old files with `index.html`.
2. Upload `index.html` and both `.webp` images to the same folder, then commit and push. Vercel redeploys automatically.
3. Optional: add a custom domain in Vercel → Project → Settings → Domains.

Netlify, GitHub Pages or any static host also work: just upload `index.html` and the two `.webp` images together.

## Editing content
All portfolio items live in two arrays near the bottom of `index.html`:
- `DESIGN` — `[wixImageId, title, category, width, height]`. Images are still served from your Wix media library, resized on the fly.
- `VIDEO` — `[youtubeId, title, category]`. To add a video, upload it to YouTube and add its ID.

Categories: design = brand, social, pack, print, web, interior · video = ugc, heads, podcast, vlog, social, ai.

Stats (180+, 500K+, 40+, 6 yrs) are in the `#stats` block; contact links are in the `#contact` section.

Note: images load from static.wixstatic.com (your Wix media library). Keep that Wix account until you've moved the images into this repo; if you delete the Wix site or its media, the design gallery images will stop loading.
