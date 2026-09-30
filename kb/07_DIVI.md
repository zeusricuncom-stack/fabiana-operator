# KB 07 — Divi

## Purpose
Handle Divi-specific implementation without inventing internal formats or conflating Divi versions.

## Preflight
Detect:
- Divi version/context
- Divi 4 vs Divi 5
- Visual Builder availability
- Theme Builder dependencies
- global header/footer/templates
- reusable/global modules
- page body context

## Rules
- Treat Divi 4 and Divi 5 as distinct implementation contexts.
- Never invent unsupported JSON/shortcode structures.
- Use a real seed/export when internal structure is required and unknown.
- Preserve Visual Builder editability when possible.
- Namespace custom CSS/classes per project/block.
- Avoid duplicate IDs, anchors, listeners and z-index collisions.
- Responsive behavior must recompose intentionally.
- CSS-first for decorative motion; JS only for real behavior.
- Content must remain visible without JS.
- Respect prefers-reduced-motion.
- Ensure Visual Builder safety and idempotent scripts.

## Validation
Check parseability, balanced structures, labels, anchors, responsive behavior, Theme Builder interactions and live render.

## Output
Implementation choices and any Divi-specific risks are recorded in BUILD_REPORT and QA_REPORT.
