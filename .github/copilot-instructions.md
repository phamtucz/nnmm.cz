# Copilot Instructions for nnmm.cz

## Project Overview
- This is a static website project, primarily HTML/CSS/JS, with no backend code in this repository.
- The main site files are in the root directory (e.g., `index.html`, `indexvn.html`, `contact.html`, etc.).
- Static assets are under `static/` (CSS, JS, images, and third-party libraries).
- The `static/libs/bootstrap/` directory contains a vendored copy of Bootstrap (with its own build/test system, not used for the main site).

## Key Patterns & Conventions
- All site logic is implemented in plain JavaScript (`static/js/`). No frameworks are used for the main site.
- CSS is organized by theme and purpose: `public.css`, `public2.css`, `style.css`, etc.
- Do not introduce build steps or package managers for the main site unless explicitly requested.
- All HTML files are self-contained and reference assets via relative paths.
- No templating or server-side rendering is used.

## Developer Workflow
- Edit HTML, CSS, and JS files directly. No build or test commands are required for the main site.
- To preview changes, open HTML files directly in a browser.
- Ignore the `static/libs/bootstrap/Gruntfile.js` and related build/test tasks unless working on Bootstrap itself.
- There are no automated tests or CI/CD for the main site.

## External Libraries
- Bootstrap, Font Awesome, and jQuery are included as static assets in `static/libs/`.
- Do not update or modify vendored libraries unless specifically working on them.

## Examples
- To add a new page, copy an existing HTML file and update as needed.
- To add a new style, edit or add a CSS file in `static/css/` and reference it in the relevant HTML files.
- To add a new script, place it in `static/js/` and reference it in the HTML.

## Special Notes
- The `schema.org` file is a large data/resource file, not code.
- The root `README.md` is currently empty; see this file for project guidance.

---
For any non-obvious changes or new conventions, update this file to keep AI agents productive.
