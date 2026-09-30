# KB 01 — Project Intake

## Purpose
Transform unstructured client material into a normalized PROJECT_CONTEXT without designing yet.

## Minimum design brief gate
Before visual ideation or implementation, the system must know at minimum:
- DESIGN_TARGET: what site, page, flow, screen or component is being created/redesigned
- USER_OUTCOME: what the intended user should be able to understand, decide or do

If either is materially unclear, ask one targeted question. Do not ask again for information already present in the conversation, files or project context.

When both are clear, produce a concise BRIEF_PLAYBACK summarizing the interpreted target, intended user outcome, main business objective, hard constraints and relevant defaults. This playback is not a request for approval; it is a checkpoint that allows the user to course-correct before research/design continues.

Hard boundary: do not start visual ideation, WordPress implementation or production work while DESIGN_TARGET or USER_OUTCOME is missing.

## Acceptable inputs
Business notes, goals, URLs, current website, logos, brandbook, colors, typography, images, videos, PDFs, screenshots, social profiles, product/service data, references, constraints and loose ideas.

Use only context relevant to the current task. Do not inspect every available asset, reference or historical source unless it is needed.

## Required normalized fields
- BUSINESS
- OFFER
- AUDIENCE
- LOCATION
- WEBSITE_TYPE
- BUILD_MODE: NEW_BUILD | REDESIGN
- DESIGN_TARGET
- USER_OUTCOME
- PRIMARY_GOAL
- PRIMARY_CONVERSION
- SECONDARY_CONVERSION
- BRAND
- CONTENT
- FUNCTIONAL_REQUIREMENTS
- ASSETS
- REFERENCES
- CONSTRAINTS
- UNKNOWNS
- SUCCESS_CRITERIA

## Redesign audit
Also identify:
- pages and URLs to preserve
- SEO-sensitive routes
- current content worth keeping
- reusable assets
- current functionality and integrations
- header/footer/theme-builder dependencies
- WooCommerce dynamic content if present
- risks created by replacing current structure
- visual/source references that should ground the redesign

## Rules
- Do not invent missing business facts.
- Mark unknowns explicitly.
- Do not begin visual design in this phase.
- Do not require perfectly organized client input.
- Ask only for information that materially blocks the next phase; otherwise proceed with declared assumptions.
- Do not silently ignore a named reference, URL, screenshot, Figma frame or brand source. If it cannot be accessed, flag the gap before relying on it.

## Output
PROJECT_CONTEXT using the schema defined in schemas/project-context.md, plus BRIEF_PLAYBACK when the minimum design brief is satisfied.
