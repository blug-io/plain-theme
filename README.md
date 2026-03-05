# Blug Plain Theme

A minimal, typography-first HTML theme designed as a **source of truth** for framework implementations (Angular, Next.js, and others).

## Concept

This theme intentionally favors:

- clear typography
- predictable spacing rhythm
- low visual noise
- portable Tailwind utility styling

The goal is to define stable UI contracts in plain HTML that can be mapped into reusable framework components without changing visual behavior.

## Project Structure

- `index.html`, `articles.html`, `article-detail.html`, `categories.html`, `category-detail.html`, `tags.html`, `tag-detail.html`, `about.html`: reference page implementations
- `components/`: reusable component-level HTML snippets with usage docs
- `components/page-assemblies/`: page composition contracts showing how to combine components into full pages

## Important Sections

- Components catalog: [components/components-index.html](./components/components-index.html)
- Components guide: [components/README.md](./components/README.md)
- Page assemblies guide: [components/page-assemblies/README.md](./components/page-assemblies/README.md)

## How To Use

## 1. Use as static HTML

Open any page directly (or serve with a static server) to preview baseline behavior.

## 2. Use in Angular/Next.js (or other frameworks)

1. Start from the page assembly for the page you want to implement.
2. Map each referenced component include into your framework component.
3. Replace placeholder tokens (e.g. `[TITLE]`, `[ARTICLE_URL]`) with real props/data bindings.
4. Keep Tailwind classes unchanged unless intentionally customizing the design system.

## 3. Keep this as source of truth

When design updates are required:

1. update component HTML first
2. update page assemblies if composition changes
3. then propagate to framework-specific repositories

## Notes

- Component files contain HTML comments for usage, scope, and integration hints.
- Page assembly files are not runtime templates; they are architecture references for implementation.
