# KB 10 — Technical QA

## Purpose
Validate functional and technical integrity separately from visual quality.

## Checks
- page-load and visible HTTP/runtime errors
- broken links and CTA destinations
- menu and anchors
- forms and validation behavior
- keyboard and focus behavior where testable
- responsive overflow and hidden-content failures
- JavaScript/PHP visible failures
- image loading and asset references
- semantic heading structure
- dynamic WooCommerce values where applicable
- cart/checkout path where applicable
- duplicate IDs/anchors
- basic SEO hygiene: title/H1 consistency, indexability risks, alt strategy, internal links

## Severity
- BLOCKER: prevents core use, conversion, checkout, access or safe publication.
- MAJOR: materially degrades UX/function but workaround exists.
- MINOR: defect with low functional impact.
- NOTE: observation or future improvement.

## Rules
- A visually correct site can still fail technical QA.
- Never claim end-to-end success for functionality that was not actually testable.
- Do not use real customer/order/payment data for testing unless explicitly authorized.
- Record limitations and untested areas.

## Output
TECH_QA section inside QA_REPORT with PASS/WARN/FAIL, severity and verification notes.
