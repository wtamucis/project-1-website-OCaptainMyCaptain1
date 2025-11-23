## Brief project overview

- This repository is a small static website for a class project (plain HTML/CSS, no build system).
- Primary pages: `index.html`, `proracquets.html`, `racquetgallery.html`. Styles in `styles.css`. Static assets live in `images/`.
- No package.json, no server code, and no tests — edits are simple file changes and should be previewed in a browser (see "Previewing" below).

## What you (the AI agent) should do first

1. Read `README.md` and `index.html` to understand the content and the preview workflow.
2. Keep all changes local and small: add or edit HTML/CSS files, create new pages in the repo root, and place images under `images/`.
3. When modifying or adding images, follow the project convention: lowercase filenames, no spaces (use `-` or `_`).

## Conventions & examples (do these exactly)

- Images: put images into `images/` and reference with a relative path. Example:

  `<img src="images/my-racquet.jpg" alt="Brand Model" class="some-class">`

- Filenames: lowercase, hyphens or underscores. Example: `golden-retrievers-public-domain.jpg` (see `index.html`).
- Styles: global stylesheet is `styles.css`. Use class names, keep rules simple and avoid adding complex build tooling.
- New pages: place new `.html` files at repository root and link them from `index.html` or other pages.

## Previewing and developer workflow

- The README recommends using the VS Code Live Server extension to preview pages: right-click the file and choose "Open with Live Server".
- Git workflow is manual: use `git add -A`, `git commit -m "brief message"`, and `git push` when ready. Keep commits focused and with short messages.

## What not to do

- Do not introduce node/npm tooling, transpilers, or bundlers (there's no manifest like `package.json`).
- Don't move or rename the `images/` folder; keep asset paths relative.

## Helpful examples from this repo

- `index.html` — shows the primary pattern for linking the stylesheet and adding an image with class `golden-img` (see `styles.css`).
- `styles.css` — simple class-based styles; prefer adding small, readable selectors rather than global resets.

## Commit & PR guidance for the human maintainer

- When you edit files, update `README.md` if you add a new recommended preview step or page.
- Use small, reviewable PRs when adding new pages or multiple images.

## If something is unclear

- Ask the user if adding a new page is allowed or if a specific HTML structure is required for grading.
- If you need to add automation (tests, build) request permission first — this project is intentionally simple.

---

If you want changes or a different tone (more/less hand-holding), tell me which parts to expand or compress and I will iterate.
