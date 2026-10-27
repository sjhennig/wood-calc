# Wood Calc

A one-page calculator for the shop. Type a measurement in **mm, cm, m, inches or feet** and it shows the
nearest **1/16"** or **1/32"** as a tape-measure fraction (e.g. `127 mm → 5"`, `19 mm → 3/4"`).

It also shows:
- feet-and-inches for anything 12" or longer
- the exact decimal value, and how far the rounded mark is over or under it
- a one-inch strip of tape with the mark highlighted

The app is a single `index.html` with no build step and no dependencies; the only other files are its icons. It has its own number pad, so the phone keyboard never covers the answer, and it fits on one iPhone screen for one-handed use. Your last value, unit and precision are remembered on your device.

## Live site

**https://wood-calc.com**: hosted on Cloudflare Pages, which redeploys automatically whenever `main` changes.

Cloudflare Pages settings, in case the project ever needs recreating:
- **Production branch:** `main`
- **Framework preset:** None
- **Build command:** blank
- **Build output directory:** blank (the repo root)

To put it on an iPhone, open https://wood-calc.com in Safari, then **Share → Add to Home Screen**.

## Icons

The ½ key icon matches the app's orange Copy key and uses the app's Barlow Condensed font,
converted to outlines so it doesn't depend on any font being loaded.
- `favicon.svg` is the browser-tab icon for modern browsers.
- `favicon.ico` is the fallback for older browsers and tools.
- `apple-touch-icon.png` (180×180) is the iPhone Home Screen icon. It has square corners on purpose, because iOS rounds them itself.

## Rounding rules

- 1 inch = 25.4 mm exactly.
- Values round to the nearest mark; a value exactly halfway between two marks rounds up.
