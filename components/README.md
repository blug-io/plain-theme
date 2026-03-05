# Components

This folder contains reusable HTML + Tailwind component primitives for the Blug Plain Theme.

Each component file includes documentation in HTML comments describing:

- where it is used
- how it should be used
- what values/placeholders should be replaced in framework ports

## Component Files

- `site-navigation.html`
- `site-footer.html`
- `page-header.html`
- `article-card.html`
- `article-list-filters.html`
- `category-list.html`
- `tag-list-inline.html`
- `article-detail-header.html`
- `article-content-shell.html`
- `components-index.html` (catalog)

## How To Use

1. Treat each file as a UI contract.
2. Convert each into a framework component (Angular component, React component, etc.).
3. Replace bracket placeholders like `[TITLE]` with props/inputs/state.
4. Preserve Tailwind classes for visual consistency.

## Composition Reference

Use page composition docs here:

- [page-assemblies/README.md](./page-assemblies/README.md)
- [page-assemblies/index.assembly.html](./page-assemblies/index.assembly.html)

## Conventions

- Keep component files focused and component-worthy.
- Avoid putting full pages inside component files.
- Prefer composition via page assemblies instead of duplicating markup.
