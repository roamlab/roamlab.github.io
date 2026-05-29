# roamlab.github.io

Project pages for the **[ROAM Lab](https://roam.me.columbia.edu)** — the Robotic
Manipulation and Mobility Lab at Columbia University.

**Live site:** https://roamlab.github.io

Each paper lives in its own self-contained folder (`reactemg/`, `hula/`, `morph/`, …)
and is served at `roamlab.github.io/<project>/`. The root `index.html` is the landing
page that links to all of them.

## Repository layout

- `index.html` — landing page / project gallery.
  - `assets/css/index.css` — landing-page styles (shares the per-paper design language).
  - `assets/thumbs/` — one optimized 4:3 thumbnail per project.
- `<project>/` — one folder per paper, each with its own `index.html` and assets.

## Adding a new project

1. Copy the `reactemg/` folder as a template (pure HTML + a self-contained
   `static/css/index.css`, no JS; fonts/icons from CDN) and fill in your content.
2. Add a thumbnail at `assets/thumbs/<project>.jpg` (~560×420, 4:3, crop-to-fill).
   If you don't have an image yet, use a monogram placeholder row instead
   (`<div class="thumb placeholder"><span>NAME</span></div>`).
3. Add an `<a class="project-row">` entry near the top of `index.html` (newest first).

## Committing

Please format commit messages as `[PROJECT_NAME]: [COMMIT_MESSAGE]`
(e.g. `reactemg: fix teaser video`). Please avoid merge commits by using rebase.
