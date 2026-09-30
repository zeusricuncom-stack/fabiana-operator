# KB 01 — Project Intake

## Purpose
Transform unstructured client material into a normalized PROJECT_CONTEXT without designing yet.

## Acceptable inputs
Business notes, goals, URLs, current website, logos, brandbook, colors, typography, images, videos, PDFs, screenshots, social profiles, product/service data, references, constraints and loose ideas.

## Required normalized fields
- BUSINESS
- OFFER
- AUDIENCE
- LOCATION
- WEBSITE_TYPE
- BUILD_MODE: NEW_BUILD | REDESIGN
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

## Rules
- Do not invent missing business facts.
- Mark unknowns explicitly.
- Do not begin visual design in this phase.
- Do not require perfectly organized client input.
- Ask only for information that materially blocks the next phase; otherwise proceed with declared assumptions.

## Output
PROJECT_CONTEXT using the schema defined in schemas/project-context.md.
