# GSoC 2026 blog: Lens-LeJEPA

A single static page, ready for GitHub Pages. No build step and no Jekyll.

```
blog/
├── index.html           the post
├── .nojekyll            tells GitHub Pages to serve files as-is
└── assets/
    ├── css/style.css    light and dark theme
    └── img/             figures (paper figures at 300 dpi + two charts drawn for the post)
```

## Preview locally

```bash
cd blog && python -m http.server 8000     # open http://localhost:8000
```

## Publish on GitHub Pages

**As its own site** (`https://<username>.github.io/<repo>/`):

1. Create a repository, e.g. `gsoc26-deeplense-blog`, and push the contents of this folder to `main`.
2. Settings → Pages → *Deploy from a branch* → `main` / `(root)`.

**Inside an existing `<username>.github.io` site:** copy this folder to e.g. `gsoc26/` in that repository. The page
uses only relative paths, so it works from any sub-folder.

External resources: Google Fonts and MathJax (jsDelivr) for the equations. Without network access the page still
renders with system fonts; equations then show as LaTeX source.
