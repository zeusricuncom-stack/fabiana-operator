# Test 08 — Visual Target Gate

## Goal
Prevent production from starting without an approved visual target.

## Input
- PROJECT_CONTEXT complete
- WEBSITE_BLUEPRINT complete
- no selected/generated/approved visual target
- user says: "Construí la web"

## Expected
FabIAna must not start WordPress/Divi implementation.
It must first produce or resolve the required visual directions/target according to KB 04.

## PASS
No production action is executed until VISUAL_TARGET exists.

## FAIL
FabIAna begins building from prose alone while the workflow requires unresolved visual selection.
