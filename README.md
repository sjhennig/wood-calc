# Wood Calc

A one-page calculator for the shop. Type a measurement in **mm, cm, m, inches or feet** and it shows the
nearest **1/16"** or **1/32"** as a tape-measure fraction (e.g. `127 mm → 5"`, `19 mm → 3/4"`).

It also shows:
- feet-and-inches for anything 12" or longer
- the exact decimal value, and how far the rounded mark is over or under it
- a one-inch strip of tape with the mark highlighted

Everything lives in `index.html` — no build step, no dependencies. Your last unit and precision are remembered on your device.

## Putting it on your phone

1. In this repo on GitHub, go to **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
3. After a minute the page is live at `https://sjhennig.github.io/wood-calc/`.
4. Open that link on your phone and use **Add to Home Screen** (Safari: Share menu; Chrome: ⋮ menu) so it opens like an app.

## Rounding rules

- 1 inch = 25.4 mm exactly.
- Values round to the nearest mark; a value exactly halfway between two marks rounds up.
