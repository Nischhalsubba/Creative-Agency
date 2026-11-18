<div align="center">

# Creative Agency

**A responsive creative-agency website project for presenting services, work, brand personality, and clear contact paths.**

![Top language](https://img.shields.io/github/languages/top/Nischhalsubba/Creative-Agency?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/Nischhalsubba/Creative-Agency?style=flat-square)
![Repo size](https://img.shields.io/github/repo-size/Nischhalsubba/Creative-Agency?style=flat-square)

[Open homepage](./index.html) · [Browse site pages](./) · [Issues](https://github.com/Nischhalsubba/Creative-Agency/issues)

</div>

## Overview

**Creative Agency** is documented as a public-facing website experience: help visitors understand the agency, scan services and work, build confidence, and reach a useful next action without fighting the interface.

| Audience | Focus |
|---|---|
| Visitors / clients | Services, work, credibility and contact |
| Developers | Page structure, interactions, assets and delivery |
| Designers | Brand expression, hierarchy, responsive behavior and motion |
| Content teams | Clear positioning, case-study copy, metadata and calls to action |

<details open>
<summary><strong>🏗️ Interactive website architecture</strong></summary>

```mermaid
flowchart LR
    VISITOR["Prospective client"] --> UI["Responsive website"]
    UI --> HERO["Positioning / hero"]
    UI --> SERVICES["Services"]
    UI --> WORK["Projects / proof"]
    UI --> ABOUT["Agency story"]
    UI --> CONTACT["Contact / CTA"]
    STYLE["Visual system & media"] --> UI
    SCRIPT["Interactions"] --> UI
```

</details>

## Visitor flow

```mermaid
flowchart TD
    LAND["Land on site"] --> VALUE["Understand what the agency does"]
    VALUE --> EXPLORE["Review services / work"]
    EXPLORE --> TRUST["Build confidence"]
    TRUST --> CTA["Choose a next action"]
    CTA --> CONTACT["Contact / enquire / continue"]
```

## Repository map

```text
Creative-Agency/
├── .github/   # automation
├── index.html, about.html, services.html, work.html, blog.html, contact.html
├── assets/    # local styles, scripts, vendor files, and imagery
├── docs/      # project guidance and archival material
└── README.md  # project overview
```

## Getting started

```bash
git clone https://github.com/Nischhalsubba/Creative-Agency.git
cd Creative-Agency
```

Run `python3 -m http.server 8000` from the repository root, then open `http://localhost:8000/`. This static page collection does not require a package-manager build step.

## Design & accessibility

Keep brand expression subordinate to comprehension. Preserve readable typography, useful spacing, visible focus, keyboard access, responsive layouts, reduced-motion behavior when motion exists, meaningful image alternatives, and clear CTA hierarchy.

## SEO & discoverability

For a public agency site, prioritize accurate **creative agency, design services, digital services, portfolio, case study, and contact** language only where it reflects real content. Use unique titles/descriptions, semantic headings, descriptive internal links, Open Graph metadata, canonical URLs, accessible images, and structured organization/project data where appropriate.

## Contribution flow

```mermaid
flowchart LR
    BRIEF["Content / design change"] --> BUILD["Implement"]
    BUILD --> RESPONSIVE["Responsive review"]
    RESPONSIVE --> ACCESS["Accessibility review"]
    ACCESS --> SEO["Metadata / content check"]
    SEO --> PR["Pull request"]
```

## Maintainer review guide

See [define agency navigation, content and enquiry QA](./docs/AGENCY_PAGE_AND_ENQUIRY_QA.md) for scoped review procedures, release evidence and risk controls specific to this repository.
