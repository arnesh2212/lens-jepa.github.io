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
