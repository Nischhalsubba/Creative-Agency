# Creative Agency: content and lead-path quality checklist

The static website is rooted at **index.html**, with main public pages including **about.html**, **services.html**, **work.html**, **blog.html** and **contact.html**. Visual changes and contact-path changes should be reviewed as a complete visitor journey.

## Editorial and trust rules

- Services and capabilities must correspond to work the agency can credibly demonstrate.
- Project imagery must be authentic or clearly labelled conceptual; check attribution and use permissions.
- Do not create invented testimonials, client logos, conversion rates or award claims.
- Keep a clear call to action appropriate to the page, without coercive urgency.
- Maintain valid links to work examples, service details and contact destinations.

## Acceptance matrix

| Route or state | Review outcome |
| --- | --- |
| Homepage | Primary value proposition and first action are readable without motion |
| About | People, roles and credentials are represented accurately |
| Services | Scope is clear; unsupported guarantees and vague pricing claims are removed |
| Work | Case-study images and descriptions correspond to the claimed projects |
| Blog | Article cards and internal links resolve; headings and dates are meaningful |
| Contact | Inputs have visible labels, validation feedback and explicit submission result when forms exist |
| Navigation | Current page is understandable; keyboard and mobile menu behavior are reliable |
| Error/empty states | Failed requests do not falsely claim that a message was sent |

## Manual local preview

From repository root, start a static web server:

~~~bash
python -m http.server 8000
~~~

Open http://localhost:8000/ and check each maintained HTML page. This command previews the current files but does not simulate an external form delivery service, so a real send must only be reported as tested when an approved endpoint is used.

## Accessibility and performance

Test keyboard navigation, readable link names, focus contrast, 200% zoom, reduced-motion preference, mobile menu reachability, and missing image handling. Check titles and descriptions for each public page. Do not remove semantic headings to match a screenshot.

## PR evidence

For each changed page, report its URL/path, before/after purpose, source of claims and imagery, manual browser matrix, link results, and automation results (if applicable). Note any blocked integration, and avoid posting personal contact submissions in issues.

## Incident and rollback

If a contact action becomes unreliable or an unsupported public claim ships, disable the misleading claim/action or revert the focused change promptly. Verify the public experience after rollback; a local file check alone does not prove production status.
