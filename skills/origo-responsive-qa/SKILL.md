---
name: origo-responsive-qa
description: Review a website experience across mobile, tablet, and desktop, reporting observable responsive, accessibility, and perceived-performance issues without claiming checks that were not performed.
license: MIT
---

# ORIGO Responsive QA

Use this skill before launch or after a visual change when a website must work cleanly across devices.

## What it solves

It turns vague feedback such as “it feels broken on mobile” into a prioritized report with reproducible viewport-specific findings.

## Evidence rule

Only report what you can observe from the supplied URL, screenshots, code, or test output. If browser automation, network inspection, or a real device was not available, label that check as unverified.

## Review matrix

Check at least:

- Compact mobile: 320–390 px wide.
- Large mobile or tablet: 768 px wide.
- Desktop: 1280–1440 px wide.
- Landscape when the layout has horizontal interactions.

## Check

1. Horizontal overflow and clipped content.
2. Header, navigation, dialogs, and sticky elements.
3. Tap targets, focus states, labels, and keyboard access.
4. Text scale, line length, contrast, and theme variants.
5. Images, canvas, video, and animation fallbacks.
6. Loading order, large requests, and visible layout shifts.
7. Forms, error states, links, and external navigation.
8. Reduced-motion and low-power behavior.

## Output

Return a table with viewport, severity, evidence, affected component, recommended fix, and verification status. Prioritize blockers that prevent reading, navigation, contact, or checkout. Finish with a short retest checklist.

Never claim “responsive everywhere” from one viewport or from a build that was not run.
