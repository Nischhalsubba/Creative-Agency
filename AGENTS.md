# Repository Instructions

## Setup

Serve the static repository root:

```bash
python -m http.server 8000
```

Open `index.html` and test every linked page.

## Architecture

- Root HTML files define home, about, services, work, insights, and contact experiences.
- `assets/css/main.css` and `helper.css` are runtime styles.
- `assets/scss/atomic/` contains modular source organization.
- Vendor scripts provide sliders, galleries, cursor behavior, and template interactions.

## Change rules

- Preserve page-level section comments and shared class conventions.
- Keep runtime CSS and SCSS source aligned when both are maintained.
- Do not duplicate navigation, footer, or overlay-menu behavior per page.
- Verify all local video formats and fallback imagery.
- Remove unused vendor libraries before adding new ones.
- Treat business claims, projects, metrics, and testimonials as placeholders until approved.

## Accessibility and motion

- Keep the skip link and semantic navigation.
- Test overlay menu and accordions by keyboard.
- Maintain visible focus.
- Add reduced-motion behavior for transitions, cursor, parallax, and reveals.
- Ensure project information is not hover-only.

## Verification

1. Test every HTML page.
2. Check menu, transitions, cursor, accordions, galleries, and videos.
3. Review mobile navigation and layouts.
4. Check console and missing assets.
5. Validate forms, metadata, internal links, and alt text.
6. Verify deployment before publishing a live link or screenshot.

## Do not

- Do not claim Aurora Creative Co. is a real operating agency unless confirmed.
- Do not publish template clients or results as evidence.
- Do not present the repository thumbnail as a browser screenshot.