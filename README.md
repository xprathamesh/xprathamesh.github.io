# xprathamesh.github.io

Personal site: [xprathamesh.github.io](https://xprathamesh.github.io/)

Plain HTML + CSS. No framework, no build step, no JavaScript. GitHub Pages serves the repo root.

```
index.html    all page content
style.css     all styling (dark theme; every color is a token at the top of the file)
favicon.svg   "PP" tab icon
```

On screens 1000px and wider, the name, headline and links sit in a left column that stays in place while the sections scroll. Phones get a single column.

## Editing

- **Content:** edit `index.html`. Each section is marked with a `<!-- ===== NAME ===== -->` comment.
- **Preview locally:** open `index.html` in a browser. Everything uses relative paths.
- **Publish:** commit and push to `master`. Pages redeploys in about a minute.
- **Status line:** the "Open to new roles" line at the bottom of the left column. Edit its text, or delete the line to hide it.

## Things that are ready to switch on

Each one is a commented-out line in `index.html`. Uncomment it to turn it on.

| What | How |
|---|---|
| Photo | Add `images/avatar.jpg` (square, ~480px) and uncomment the `<img class="avatar">` line in the hero |
| Resume button | Add `resume.pdf` to the repo root and uncomment the Resume button in the hero |
| Beyond work | Uncomment the `BEYOND WORK` section **and** its nav link in the header |

> Note: HTML comments are visible in the page source, so don't park anything private in them.

## Adding a page (e.g. Investing)

1. Create `investing/index.html` by copying `index.html`, keeping the `<head>`, header and footer, and replacing what's inside `<main>`.
2. In the new file, point assets one level up: `../style.css`, `../favicon.svg`.
3. Link to it from a card in the Beyond work section (`href="investing/"`).

The existing styles (`.label`, `.cards`/`.card`, the `.item` timeline and `.teams` sub-list) work on any page.
