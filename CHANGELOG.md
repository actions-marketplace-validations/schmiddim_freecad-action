# Changelog

All notable changes to this project are documented in this file.

## [v3.0.0](https://github.com/schmiddim/freecad-action/releases/tag/v3.0.0) - 2026-05-28

Major release with improved documentation and project hygiene.

- Add MIT LICENSE file
- Rewrite README: badges, "Why?" section, quickstart first, troubleshooting, corrected demo URL
- Add CONTRIBUTING.md
- Add CHANGELOG.md
- Improve aggregator documentation with link to https://freecad-aggregator.fly.dev/
- Update all schema URLs to v3.0.0
- Move `Agents.md` and `Architecure.md` to `.github/` (fix typo in filename)
- Rename `öpcjeosemsatz.FCStd` to `opcje-oemsatz.FCStd`
- Update project structure documentation (templates in `scripts/templates/`)
- Update version pinning examples to v3

## [v2.8.9](https://github.com/schmiddim/freecad-action/releases/tag/v2.8.9) - 2026-05-26

- Fix: add git to Docker image for commit-date sorting

## [v2.8.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.8.0) - 2026-05-26

- Fix: use existing action versions (checkout@v4, gh-release@v2)
- Add workflow_dispatch trigger

## [v2.7.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.7.0) - 2026-05-17

- Tailwind CSS via PostCSS replacing custom CSS
- Jinja2 template inheritance with partials (base, footer, scripts)
- Consistent layout and typography across all pages
- Node.js/npm integration in GitHub Action and build.sh
- Dark mode with system preference detection

## [v2.6.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.6.0) - 2026-05-17

- Move templates to `scripts/templates/` for better organization
- Extract all CSS to separate `styles.css` file
- Add footer with freecad-action attribution
- Fix GitHub links to point to repository

## [v2.5.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.5.0) - 2026-05-17

- Full UTF-8/Unicode support in filenames (umlauts, accents, CJK, Cyrillic)
- Docker container with full UTF-8 locale configuration
- All file operations UTF-8 aware

## [v2.4.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.4.0) - 2026-05-17

- Unified gallery combining 3D viewer and photos
- Thumbnail navigation between 3D model and images
- Improved visual hierarchy and UX

## [v2.3.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.3.0) - 2026-05-17

- Printables-style image gallery with hero image and thumbnails
- Lightbox/modal for full-size image viewing
- Keyboard navigation support
- Enhanced metadata creation UX with interactive hint box

## [v2.2.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.2.0) - 2026-05-17

- 100x faster thumbnail rendering with OpenSCAD (0.1s vs 10-20s)
- Multiple rendering backends with automatic fallback
- Improved rendering quality

## [v2.1.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.1.0) - 2026-05-16

- Automatic thumbnail generation from STL files using trimesh
- Headless rendering without FreeCADGui or X11 dependencies
- 800x600 PNG thumbnails in CI/CD pipelines

## [v2.0.0](https://github.com/schmiddim/freecad-action/releases/tag/v2.0.0) - 2026-05-16

- Major version bump (Docker-based architecture)

## [v1.5.0](https://github.com/schmiddim/freecad-action/releases/tag/v1.5.0) - 2026-05-15

- Repository renamed from `freecad-actions` to `freecad-action` (singular)
- Docker image: `ghcr.io/schmiddim/freecad-action:latest`

## [v1.4.0](https://github.com/schmiddim/freecad-action/releases/tag/v1.4.0) - 2026-05-15

- Pass `github.action_ref` as `ACTION_REF` env for generator_version in discovery doc

## [v1.3.0](https://github.com/schmiddim/freecad-action/releases/tag/v1.3.0) - 2026-05-15

- Dark/light mode toggle
- GitHub link in navigation
- FCStd download button

## [v1.2.0](https://github.com/schmiddim/freecad-action/releases/tag/v1.2.0) - 2026-05-15

- Configurable gallery title via `cad-gallery.yaml`
- Schema URL support

## [v1.1.0](https://github.com/schmiddim/freecad-action/releases/tag/v1.1.0) - 2026-05-15

- RSS 2.0 and Atom 1.0 feed generation
- Auto-detection of base URL from git remote
- UTF-8 encoding fixes for international filenames

## [v1.0.0](https://github.com/schmiddim/freecad-action/releases/tag/v1.0.0) - 2026-05-15

- Initial release as reusable GitHub Action
- FreeCAD STL export via Docker
- Three.js interactive gallery
- GitHub Pages deployment
