# KB 09 — Visual QA

## Purpose
Compare the rendered site against the approved visual target, blueprint and Design Fingerprint, then drive an iterative correction loop before handoff.

## Required evidence
A valid visual QA pass requires both:
- SOURCE_VISUAL_TRUTH: approved mockup, selected concept, Figma frame, screenshot/reference or sufficiently specific approved blueprint
- RENDERED_IMPLEMENTATION: live/staging/local render or implementation screenshot

If either side cannot be opened, captured or compared, final result is BLOCKED. Do not claim visual completion from memory, code or file paths alone.

## State matching
Before comparing, match as closely as possible:
- viewport
- route/page
- content/state
- theme
- auth state when relevant
- interaction state
- crop and visible region

If source and implementation are not comparable states, record that mismatch before judging fidelity.

## Required viewports
- Desktop
- Tablet
- Mobile
Use exact viewport dimensions when tool support allows; otherwise record the available viewport and limitation.

## Evidence protocol
- Capture the actual rendered implementation.
- Inspect the accepted screenshot before using it as evidence.
- Reject screenshots that are blank, loading, blocked, cropped incorrectly or show the wrong state.
- Compare source and implementation in a normalized view; do not mistake browser chrome, density differences or framing mismatches for design drift.
- Use full-view comparison for composition and focused-region comparison when typography, navigation, imagery, forms or controls are too small to judge reliably.

## Required fidelity surfaces
Every substantial QA pass explicitly evaluates:

### Typography
Font family/fallback, weight, size, line-height, letter-spacing, hierarchy, wrapping, truncation and readability.

### Spacing and layout rhythm
Frame/crop, alignment, margins, padding, grid tracks, section gaps, component spacing, radii, elevation and vertical rhythm.

### Colors and visual tokens
Palette, gradients, opacity, contrast, semantic colors and foreground/background balance.

### Images and assets
Subject correctness, crop, scale, sharpness, compression, masking, background treatment, transparency and fidelity to the approved art direction.

Do not replace approved logos, illustrations, decorative assets or product imagery with rough code-native approximations when the source requires the real asset.

### Copy and content
Headings, CTA text, labels, visible business facts and meaningful ordering must match approved intent unless an intentional revision is documented.

## Additional review categories
### Composition
Hierarchy, balance, scale, grid, spacing, alignment, negative space and section rhythm.

### Interaction and motion
CTA visibility, hover/focus/active behavior, motion subtlety, reduced-motion behavior and content independence from animation.

### Responsive
Reflow, overflow, sticky/fixed collisions, hidden content, touch-target problems and recomposition quality.

### Accessibility-visible checks
Contrast, focus visibility, obscured content, readable text and consistent navigation cues. Do not claim full accessibility compliance from screenshots alone.

## Severity model
- P0: blocks core use, severe accessibility failure, broken layout or impossible task
- P1: major visual/design mismatch or usability regression likely to be noticed by users
- P2: moderate visual drift, responsive issue, inconsistent state or meaningful polish gap
- P3: minor refinement that improves fidelity but does not block acceptance

Overflow that hides important persistent controls, material above-the-fold drift, major-region proportion changes, broken text wrapping or significant density mismatch are P2 or higher.

## Iteration loop
RENDER -> CAPTURE -> NORMALIZE -> COMPARE -> CLASSIFY -> CORRECT -> RENDER

When any actionable P0/P1/P2 finding exists:
1. keep result BLOCKED
2. record the finding
3. apply the correction
4. capture the revised implementation at the same viewport/state
5. compare again against the source
6. record the fix and post-fix evidence

P3 items may remain as follow-up polish.

## Pass criteria
Final result is PASSED only when:
- no actionable P0/P1/P2 finding remains
- required fidelity surfaces were checked
- required viewports were reviewed or a documented blocker/limitation exists
- latest implementation evidence supports the result

## Rules
- Do not mark PASS from code inspection alone when render inspection is available.
- Compare against approved intent, not merely whether the page is technically functional.
- Do not silently redesign approved structure during QA; material design changes require renewed approval.
- Distinguish objective mismatches from subjective polish recommendations.
- Distinguish intentional implementation constraints from unintended drift.

## Output
VISUAL_QA section inside QA_REPORT including:
- SOURCE_VISUAL_TRUTH
- implementation evidence
- viewport/state
- findings ordered by severity
- concrete fixes
- iteration history for P0/P1/P2
- residual P3 polish
- FINAL_RESULT: PASSED | BLOCKED
