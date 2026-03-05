# Page Assemblies

This folder defines **page composition contracts** for the plain theme.

Each `*.assembly.html` file documents:

- component include order
- expected props/placeholders
- page-specific sections that are not generic components

These files are intended for framework implementers and should be treated as blueprint docs, not runtime templates.

## Assembly Files

- `index.assembly.html`
- `articles.assembly.html`
- `article-detail.assembly.html`
- `categories.assembly.html`
- `category-detail.assembly.html`
- `tags.assembly.html`
- `tag-detail.assembly.html`
- `about.assembly.html`

## How To Use

1. Pick the page assembly matching the page you are implementing.
2. Translate each include comment (`../component-name.html`) into framework component usage.
3. Wire dynamic values into placeholders.
4. Keep structure and spacing consistent with the assembly definition.

## Related Docs

- Root theme guide: [../../README.md](../../README.md)
- Components guide: [../README.md](../README.md)
- Components catalog: [../components-index.html](../components-index.html)
