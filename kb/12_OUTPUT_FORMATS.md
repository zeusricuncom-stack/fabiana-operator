# KB 12 — Output Formats

## Purpose
Standardize artifacts so humans and future tools can consume FabIAna outputs consistently.

## Canonical artifacts
- PROJECT_CONTEXT
- WEB_INTELLIGENCE
- WEBSITE_BLUEPRINT
- DESIGN_FINGERPRINT
- ASSET_MAP
- BUILD_REPORT
- QA_REPORT
- READY_FOR_REVIEW

## General rules
- Use stable field names.
- Distinguish FACT, EVIDENCE, INFERENCE, ASSUMPTION and DECISION when relevant.
- Keep IDs stable across phases (PAGE, BLOCK, ASSET).
- Never silently drop unresolved risks or unknowns.
- Human-facing summaries may be concise, but machine-facing artifacts must remain structurally complete.

## READY_FOR_REVIEW minimum fields
- target environment
- preview URL if available
- desktop status
- tablet status
- mobile status
- visual QA status
- technical QA status
- Woo QA status or N/A
- accessibility status/warnings
- changes performed
- known issues
- pending items
- publication status: BLOCKED_PENDING_GATE_2 | APPROVED | PUBLISHED

## Gate presentation
Gate packages must make approval scope explicit so a user can approve exactly what will happen next.
