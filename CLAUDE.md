# zettaai.github.io

Static single-page site (GitHub Pages) for Zetta AI. Everything lives in `index.html`;
`CNAME` sets the custom domain and `img/` holds assets. There is no build step — edits to
`index.html` go live on push to `main`.

## Featured work (publication list)

Most edits are to the "Featured work" section (`<h2 id="research">`). Each paper is one block:

```html
<p class="paper">
  <a href="LINK">Title</a>.
  Author One, <u>Zetta Author</u>, Author Three. Venue. Month Year.
</p>
```

Conventions:
- **Zetta-affiliated authors** are wrapped in `<u>...</u>`. Preserve these exactly when
  copying an author list; getting them right is its own recurring fixup.
- **Published** papers link via the DOI: `https://doi.org/10.1038/...`. **Preprints** link
  via the bioRxiv URL. When a preprint becomes published, swap the link to the DOI and update
  the trailing `Venue. Month Year.` (e.g. `bioRxiv. August 2025.` → `Nature. June 2026.`).
- Entries are ordered newest-first (reverse-chronological). New papers go at the top of the list.
