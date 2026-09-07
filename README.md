# edeninfiniteart.com

Static promotional site for **Eden Infinite Art**. Nothing is sold here — the site
showcases the catalogue and sends buyers to Gumroad (printable downloads),
Redbubble (prints and gifts) and, later, Etsy.

Same pattern as `echofayyz-site`: hand-written HTML/CSS, no build step,
served by GitHub Pages with a `CNAME`.

## Animated artwork
Each gallery card has `data-loop="<id>"`. Drop a silent 2-second loop at
`loops/<id>.mp4` and that card animates on hover (and on scroll-into-view on
touch devices). Cards with no loop file stay as stills. No code change needed.

Loops are ambient only — drifting cloud, water shimmer, candle flicker. Motion
that travels across the frame will show its loop seam.

## Local preview
    python3 -m http.server 8790 --directory .
