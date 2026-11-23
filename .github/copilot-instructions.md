# Copilot Instructions for this repository

## Overview
This repository is a static personal portfolio / CV website. The project is intentionally simple and does not use a framework, build tool, or package manager.

- Main entry page: `index.html`
- Styling: `CSS/styles.css`
- Images: `images/`
- Skills/icons: `flaticons/`
- Fonts: `fonts/` and remote Google Fonts in `index.html`
- Purpose: a single-page personal landing site with profile, skills, and contact information

## Build, test, and lint commands
No automated build, test, or lint tooling is configured in this repository.

- No `package.json`, `vite.config.*`, `webpack.*`, `eslint` config, or test runner files were found.
- To preview the site locally:
  ```bash
  cd "D:\Documents\DevProjects\Web\web-portfolio\portfolio"
  python -m http.server 8000
  ```
  Then open `http://localhost:8000/` in a browser.
- There is no single-test command because there are no automated tests in the project.

## High-level architecture
- `index.html` defines the full page structure: top banner, profile section, skills section, contact section, and footer.
- `CSS/styles.css` contains the design system, layout, colors, spacing, typography, and responsive behavior.
- Static asset folders are referenced with relative paths from the site root, so the site is expected to be served directly rather than built into an output directory.
- The project is content-first and presentation-driven; most work involves editing HTML copy and CSS styles rather than application logic.

## Key conventions
- Keep changes small and local to the relevant section of the page.
- Preserve the existing personal-brand styling: centered single-page layout, teal/gray color palette, and the current typography pairing.
- Prefer the existing class names and layout patterns in `CSS/styles.css` over introducing new CSS structure.
- Maintain relative asset paths exactly as they are currently written; this project is not structured around a bundler or asset pipeline.
- If updating fonts or asset references, keep them portable and consistent with how the site is currently served.
- Personal details, social links, and contact information are user-facing content and should stay coherent across the page when edited.

## Working expectations for future changes
- Keep the site static and lightweight; do not add framework or build-tool conventions unless they are clearly needed.
- Favor direct edits to `index.html` and `CSS/styles.css` rather than creating extra abstraction layers.
- Avoid introducing JavaScript or build tooling for tasks that only require content or styling changes.
