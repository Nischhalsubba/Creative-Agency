# Agency page and enquiry quality assurance

## Scope and source of truth
This repository currently serves static pages at the **repository root**: `index.html`, `about.html`, `services.html`, `work.html`, `blog.html`, and `contact.html`. Assets live under `assets/`. Do not use an obsolete `site/` path or assume a bundler exists.

## User journeys to protect
| Visitor need | Entry point | Expected result |
| --- | --- | --- |
| Understand the agency | `index.html` | Clear positioning and accessible navigation |
| Verify capabilities | `services.html` | Service descriptions and a useful next action |
| Assess proof | `work.html` | Credible portfolio and working project links |
| Learn background | `about.html` | Accurate team/studio claims and attribution |
| Read updates | `blog.html` | Accessible article links and accurate dates |
| Make contact | `contact.html` | Reachable contact method and feedback |

## Content verification protocol
For every changed sentence about clients, services, location, awards, availability, or outcomes, record the approving content owner and source. Do not present template filler, placeholder testimonials, or illustrative pricing as factual business commitments. Verify brand naming is consistent across title, descriptions, on-page copy, image alternatives and social previews.

## Navigation and interaction review
1. Start a local static server from repository root: `python3 -m http.server 8000`.
2. Visit all six pages on desktop and narrow mobile widths. Test each visible menu item, card and footer link; log any missing targets and distinguish intentionally external links.
3. Navigate by keyboard only. Confirm skip link target, logical focus order, visible focus, and accessible name/state for toggles and overlays.
4. Review the existing smooth-scroll, page-transition, and magic-cursor behavior with reduced motion enabled and with JavaScript unavailable.
5. Confirm galleries, forms, validation states and CTA destinations work without obscuring essential content.

## Asset and performance checks
- Verify local references to `assets/vendor/`, `assets/css/`, images and scripts resolve on a case-sensitive server.
- Identify external fonts and image URLs; provide adequate fallbacks before release.
- Preserve aspect ratio and caption/alt relevance when replacing portfolio photography.
- Check for console errors, layout shift, unexpectedly large assets and overlapping sticky elements.

## Enquiry acceptance test
Document *actual* contact implementation before claiming successful submission. If the page only provides an email link or visual form mockup, label that limitation; do not imply a backend exists. Test invalid fields, successful states, keyboard completion and privacy notice where applicable. Never store or print submitted personal data in logs.

## Release evidence log
```text
Change and pages:
Reviewer / date:
Desktop and mobile widths tested:
Keyboard and reduced-motion result:
Broken links and resolution:
Content claims verified by:
Contact outcome observed:
Remaining exceptions and owner:
```

## Definition of done
A reviewer can navigate every published page, reproduce the contact journey, verify client-facing claims and confirm changed assets and interactions do not regress mobile or keyboard behavior. This file defines a review procedure; it does not certify that the site already passes it.
