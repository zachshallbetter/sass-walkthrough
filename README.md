# sass-walkthrough

A small Sass walkthrough: SCSS partials for variables, layout and a button component, compiled to CSS for a static demo page.

## Quick start

```sh
npm install
npm run dev     # sass --watch src:public
npm run build   # compressed CSS, no source map, into public/
```

Then open `public/index.html`, which links the compiled `public/main.css`.

## Repository map

- `src/main.scss`: entry point; imports the partials below.
- `src/_variables.scss`, `src/_layout.scss`, `src/_button.scss`: the partials.
- `public/index.html`: the demo page. `public/main.css` is generated and git-ignored.
- `vercel.json`: Vercel deploys `main` only.

## Verification

`npm run build` is the only check: it fails if the SCSS does not compile. There are no tests. Sass currently prints `@import` deprecation warnings during the build, because `src/main.scss` uses `@import` rather than `@use`.

## Status and limitations

A learning project, not a library. It has one dev dependency (`sass`).

## License

`package.json` declares ISC, but the repository contains no `LICENSE` file.
