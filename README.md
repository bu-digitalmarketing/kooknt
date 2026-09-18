# kooknt

Personal website for **Kanatouch Wongga** (คณธัช วงศ์กา) — Bangkok, Thailand.

A single-file site: `index.html` contains all markup, styles and scripts. The only
external dependencies are Google Fonts and Three.js, both loaded from CDNs.

## Running it

No build step. Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

## Publishing with GitHub Pages

Settings → Pages → Source: *Deploy from a branch* → `main` / `root`.
The site then goes live at `https://bu-digitalmarketing.github.io/kooknt/`.

## What's in the page

- A fixed WebGL scene (Three.js r128) with one 3D object anchored to each section —
  icosphere, gyroscope rings, cube cluster, double helix, orbit rings, dodecahedron.
- A second WebGL context for the rotating gem in the portrait tile.
- Scroll-driven 3D tilt on every section, plus hover tilt on cards, chips and links.
- Hand-drawn SVG artwork: three project thumbnails and a Bangkok skyline
  (Wat Arun, MahaNakhon, Baiyoke Tower).
- Everything degrades to a static frame under `prefers-reduced-motion`, and falls
  back to a monogram tile if WebGL is unavailable.

## Content still to replace

The following is **placeholder content** and should be swapped for real details:

- Major, faculty and the year ranges in the Education section
- Both paragraphs in the About section
- All three projects in Selected work
- The Focus chips
- The "Languages" and "Open to" line in the masthead

Confirmed and correct: name, Thai name, `kanatouch.wong@gmail.com`,
Instagram `@kookooknt`, Facebook, Bangkok University, Assumption College Thonburi.

To use a photo instead of the 3D gem, replace `<canvas id="gem">` inside
`<div class="portrait">` with an `<img>` tag.
