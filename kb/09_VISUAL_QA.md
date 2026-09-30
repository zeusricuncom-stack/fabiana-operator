# KB 09 — Visual QA

## Purpose
Compare the rendered site against the approved blueprint and Design Fingerprint, then drive an iterative correction loop.

## Required viewports
- Desktop
- Tablet
- Mobile
Use exact viewport dimensions when tool support allows; otherwise record the available viewport.

## Review categories
### Composition
Hierarchy, balance, scale, grid, spacing, alignment, negative space and section rhythm.

### Typography
H1/H2 hierarchy, line length, line-height, wrapping, contrast and responsive scaling.

### Images
Crop, focal point, quality, consistency, text-safe areas and mobile behavior.

### Interaction and motion
CTA visibility, hover/focus behavior, motion subtlety, reduced-motion behavior and content independence from animation.

### Responsive
Reflow, overflow, sticky/fixed collisions, hidden content, touch-target problems and recomposition quality.

### Accessibility-visible checks
Contrast, focus visibility, obscured content, readable text and consistent navigation cues.

## Loop
RENDER -> OBSERVE -> COMPARE -> DETECT -> CORRECT -> RENDER
Repeat until pass criteria are met or a material limitation is reached.

## Rules
- Do not mark PASS from code inspection alone when render inspection is available.
- Compare against approved intent, not merely whether the page is technically functional.
- Do not silently redesign approved structure during QA; material design changes require renewed approval.

## Output
VISUAL_QA section inside QA_REPORT with PASS/WARN/FAIL per category and evidence/notes.
