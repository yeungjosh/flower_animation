# Flower

![Flower image](flower.gif)

A pure HTML/CSS flower-growing animation. `index.html` holds the markup, `style.scss` the styles (compiled to `style.css`), and `main.js` just removes the `not-loaded` class from `<body>` one second after page load, which starts the CSS animations. If JavaScript is disabled, a `<noscript>` rule in `index.html` starts the animations immediately instead, so the page is never stuck on a paused frame.

## Run it

The compiled `style.css` is committed, so no build step is needed:

- Open `index.html` directly in a browser, **or**
- Serve the folder with [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (VS Code extension) or any static server, e.g. `python3 -m http.server` and visit <http://localhost:8000>.

## Editing the styles

Edit `style.scss`, then recompile it to `style.css` with [Sass](https://sass-lang.com/install):

```
npm i -g sass
sass --watch style.scss:style.css
```

(The npm package is `sass`; the older `scss` package is not the Sass compiler.)
