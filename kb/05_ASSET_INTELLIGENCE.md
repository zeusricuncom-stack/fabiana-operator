# KB 05 — Asset Intelligence

## Purpose
Plan, source, generate, prepare and verify visual assets before and during implementation.

## Asset provenance states
- PROVIDED: supplied by user/client.
- EXTRACT: reusable asset from authorized existing project material.
- SOURCE: externally sourced stock/licensed media.
- GENERATE: create new asset with generative tools.

## Required asset fields
- ASSET_ID
- PAGE / BLOCK
- ROLE
- PROVENANCE_STATE
- SOURCE_REFERENCE if applicable
- REQUIRED_RATIO
- DESKTOP_VARIANT
- MOBILE_VARIANT
- FOCAL_POINT
- TEXT_SAFE_ZONE
- STYLE
- QUALITY_REQUIREMENTS
- ALT_STRATEGY
- STATUS

## Asset audit
Check resolution, aspect ratio, focal point, lighting/style fit, crop flexibility, text compatibility, brand fit and commercial role.

## Generate brief
For GENERATE assets specify subject, framing, camera/visual language, lighting, negative space, ratio, mobile crop, brand cues and avoid-list.

## Processing pipeline
ORIGINAL -> VALIDATE -> CROP/RESIZE -> COMPRESS -> MODERN_FORMAT_WHEN_APPROPRIATE -> RENAME -> ALT -> UPLOAD -> VERIFY_RENDER

## Alt rules
- Informative image: concise functional description.
- Decorative image: empty alt where appropriate.
- Functional image: describe function/action, not visual appearance.

## Rules
- Never invent asset URLs.
- Never assume rights to third-party images.
- Do not design a critical block around a random placeholder.
- If an asset is missing but not blocking blueprint approval, mark it pending with an exact brief.
