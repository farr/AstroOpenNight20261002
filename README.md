# Astronomy Open Night 2026-10-02

This is the talk I gave at the [Stony Brook Astronomy Open
Night](https://www.astro.sunysb.edu/opennight/) on 2026-10-02. You can browse
the slides at

https://farr.github.io/AstroOpenNight20261002/

To run locally (required for embedded YouTube playback), serve the slides over
HTTP instead of opening `index.html` directly:

```sh
npm install
npm start
```

## Offline KaTeX for local-only use

The checked-in `index.html` uses CDN-hosted KaTeX so GitHub Pages works.
If you want local rendering with no internet connectivity, edit the
`Reveal.initialize(...)` config in `index.html` and change:

```js
katex: {
  version: "0.19.0"
}
```

to:

```js
katex: {
  local: "node_modules/katex"
}
```

Then run:

```sh
npm install
npm start
```
