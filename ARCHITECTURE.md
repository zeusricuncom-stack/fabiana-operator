# Architecture v0.1

## Core pipeline

PROJECT_INPUT -> PROJECT_CONTEXT -> WEB_INTELLIGENCE -> WEBSITE_BLUEPRINT -> GATE_1 -> PRODUCTION -> QA_LOOP -> GATE_2 -> PUBLISH

## Separation of responsibilities
- Atenea: evidence, current practices, UX, accessibility, contradiction checks.
- MarIAno: market, competition, offer, customer, objections, differentiation.
- FabIAna: interprets evidence, makes web-design decisions, builds, audits and corrects.

## Operating modes
- NEW_BUILD
- REDESIGN
- LANDING
- MULTIPAGE
- CATALOG
- WOOCOMMERCE

## Safety model
- R0 READ: inspect, search, analyze.
- R1 REVERSIBLE: draft, staging, new assets.
- R2 MODIFY: edits to external systems.
- R3 HIGH_IMPACT: publish, delete, permissions, payments, production-critical changes.

R2/R3 require explicit authority appropriate to impact. Default execution target is draft/staging.

## Gate model
GATE_1 blocks production until blueprint approval.
GATE_2 blocks publication until final review approval.

## Primary artifacts
- PROJECT_CONTEXT
- WEB_INTELLIGENCE
- WEBSITE_BLUEPRINT
- DESIGN_FINGERPRINT
- ASSET_MAP
- BUILD_REPORT
- QA_REPORT
- READY_FOR_REVIEW
