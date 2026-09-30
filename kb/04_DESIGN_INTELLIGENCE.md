# KB 04 — Design Intelligence

## Purpose
Create a project-specific visual system that is coherent within the project and sufficiently differentiated from recent FabIAna work.

## Preconditions
Do not generate or implement visual directions until KB 01 has established:
- DESIGN_TARGET
- USER_OUTCOME
- hard constraints
- relevant brand/source references

If the project already has a strong visual system and the user did not ask for a new style, stay within that system and vary structure, hierarchy, interaction and emphasis before changing brand language.

## Source inspection rule
When screenshots, Figma frames, live URLs, brand assets, previous designs or other visual references are available, inspect the actual source before designing. Do not infer visual characteristics from filenames or descriptions alone.

If a named source cannot be accessed, explicitly flag the gap. Do not silently proceed as though it was inspected.

## Design Fingerprint
Define before production:
- VISUAL_PERSONALITY
- LAYOUT_ARCHETYPE
- HERO_TYPE
- GRID_BEHAVIOR
- SPACING_RHYTHM
- TYPOGRAPHY_PERSONALITY
- GEOMETRY
- IMAGE_LANGUAGE
- CARD_LANGUAGE
- CTA_LANGUAGE
- NAVIGATION_STYLE
- SECTION_TRANSITIONS
- MOTION_PERSONALITY
- DENSITY
- CONTRAST_STRATEGY
- DECORATIVE_LANGUAGE
- SIGNATURE_ELEMENT

## Visual direction protocol
When there is no approved visual target, create exactly three meaningfully distinct visual directions before build:
- A: commercial/safe
- B: editorial/expressive
- C: experimental/distinctive

These directions must differ in information hierarchy, layout strategy, spatial composition and product framing — not merely colors or fonts.

For narrow redesigns or existing products, vary structure, emphasis and interaction first. For broad greenfield websites, directions may vary the visual system more aggressively.

Each direction must preserve:
- brand constraints
- content truth
- user outcome
- business goal
- accessibility-critical requirements
- required functionality

## Visual target gate
Production requires one VISUAL_TARGET. It may be:
- selected generated concept
- approved mockup
- Figma frame
- screenshot/reference
- approved blueprint with sufficient visual specificity

If three directions are presented to the user, stop before build until one direction is selected or the user requests a revised/hybrid direction.

If the user combines parts of multiple directions, generate/define a consolidated VISUAL_TARGET before implementation.

## Composition rules
Prefer differentiation through this order:
1. spacing, grouping, alignment, typography and hierarchy
2. dividers and structural rhythm
3. subtle surface changes
4. borders when necessary
5. shadows/elevation sparingly

Avoid:
- cards inside cards
- every section becoming a card
- decorative UI added only to fill space
- generic centered app/site panels when the page itself can be the primary surface
- visual complexity that does not support the user outcome

## Typography rules
- Maintain readable body sizes and intentional hierarchy.
- Keep long-form text at a comfortable line length.
- Avoid unnecessary font proliferation; normally use no more than two type families unless a documented design system requires otherwise.
- Treat wrapping, weight and line-height as composition variables, not afterthoughts.

## Anti-repetition gate
Avoid reusing the same dominant combination of hero, grid, typography, card language, CTA treatment, spacing rhythm and signature element from recent known projects unless functionally justified.

If project history is unavailable, do not pretend similarity was measured. Apply diversity heuristics only to known context.

## Core visual gates
- Hero must have a deliberate compositional strategy.
- Desktop must show at least one strong spatial decision.
- Text over photography must remain legible via focal-point control, overlay, scrim or repositioning.
- Responsive design must recompose, not merely shrink.
- Motion must support hierarchy and behavior, respect reduced-motion preferences and never be required for content visibility.
- Strong client imagery should influence layout rather than being forced into generic cards.
- Avoid crowding; remove non-essential UI/content before reducing readability.

## Principle
Optimize for coherence within each project and differentiation between projects; never vary visual choices randomly just to be different.
