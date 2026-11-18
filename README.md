# GAME 401 — PICO-8 Portfolio (demo)

A one-page portfolio that plays PICO-8 carts in the browser, hosted on GitHub Pages.

## Folder layout

```
index.html            the portfolio page
games/pet/index.html  the exported cart
games/pet/index.js    the cart data (must sit next to index.html)
games/pet/thumb.png   the card screenshot
```

## How to add your own game

1. Run your cart in PICO-8 and press Ctrl-7 to capture a label. Without a label
   the export fails with "please capture a label first".
2. Type `save mygame.p8`, then `export index.html`. That writes `index.html`
   and `index.js` into your cart folder.
3. Make a folder `games/yourgame/` in the repo and copy both files into it.
   Do not rename `index.js` — the HTML asks for it by that exact name.
4. Add a screenshot as `thumb.png` in the same folder.
5. Copy one `<article class="card">` block in `index.html` and point it at
   your folder.

## Turning on GitHub Pages

Settings -> Pages -> Source: Deploy from a branch -> main -> / (root).
The site appears about a minute later.
