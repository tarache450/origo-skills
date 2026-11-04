---
name: origo-launch-checklist
description: Prepare a website for a controlled launch by checking content, SEO, forms, security, responsive behavior, and rollback readiness without deploying automatically.
license: MIT
---

# ORIGO Website Launch

Use this skill when a website is close to publication and the team needs a calm, evidence-based final pass.

## What it solves

It reduces last-minute launch errors in metadata, links, forms, privacy pages, assets, and deployment configuration.

## Before checking

Identify the target environment, the intended domain, the build command, the deployment owner, and the approved scope. Never request, print, or store credentials in the report.

## Checklist

### Content and SEO

- Title, description, canonical, Open Graph, favicon, headings, alt text, sitemap, and robots.
- Main CTA, contact details, prices, case studies, and legal copy match the approved source.

### Product behavior

- Navigation, forms, validation, success/error states, external links, analytics consent, and 404 behavior.
- Test compact mobile, tablet, desktop, theme variants, keyboard focus, and reduced motion.

### Security and performance

- No secrets in source, logs, bundles, or public files.
- Validate external URLs and upload boundaries.
- Confirm lazy loading, image dimensions, caching, and a realistic build artifact.

### Release control

- Record commit, build result, smoke-test URLs, owner, and rollback path.
- Do not deploy, merge, send messages, or alter production without explicit authorization.

## Output

Return `READY`, `READY WITH FOLLOW-UPS`, or `BLOCKED`, followed by evidence for every item, unresolved risks, and the smallest next action. A green build alone is not launch approval.
