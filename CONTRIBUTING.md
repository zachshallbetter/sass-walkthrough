# Contributing to sass-walkthrough

Thanks for your interest. This project is maintained by one person, so reviews are best-effort
(see [SUPPORT.md](SUPPORT.md)).

## Setup

```sh
npm install
npm run dev     # sass --watch src:public
npm run build   # sass --no-source-map --style compressed src:public
```

## Conventions

- One partial per concern under `src/` (`_variables.scss`, `_layout.scss`, `_button.scss`),
  imported from `src/main.scss`.
- `public/main.css` is generated; do not commit it.
- Commits follow conventional-commit style, for example `ci(vercel): ...` or `docs: ...`.

## Verifying a change

There are no tests. Before opening a PR, run `npm run build` and open `public/index.html` to check
the styles.

## Pull requests

- Branch off `main`; keep PRs focused.
- Use a conventional-commit title.
- Describe the change and how you verified it. The PR template prompts for this.
