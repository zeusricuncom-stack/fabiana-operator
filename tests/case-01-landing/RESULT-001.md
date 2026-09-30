# Case 01 — Result 001

## Test type
SPEC DRY-RUN

## Result
PASSED_WITH_WARNINGS

## Score
PASS: 26
WARN: 3
FAIL: 0
CRITICAL FAIL: 0

## PASS highlights
- NEW_BUILD detected correctly.
- Landing chosen for a justified conversion objective.
- Facts, preferences, constraints and unknowns separated.
- No commercial facts invented.
- Research produced web decisions rather than a generic market report.
- Competitor evidence changed the proposed content hierarchy.
- Asset provenance remained explicit.
- Low-quality image was not forced into a structural role.
- Three materially different design directions were produced.
- Visual Target Gate remained closed.
- Run stopped before WordPress production.

## Warnings
### WARN 01 — Visual directions are still textual
The architecture now requires a real visual target before build. This dry-run defines three directions in text, but it does not exercise ImageGen or a visual selection mechanism.

**Action:** future runtime test must generate actual visual alternatives or equivalent inspectable targets before Gate 1 approval.

### WARN 02 — Asset Audit is simulated
The fixture names image files but does not include actual binary images, so resolution, crop, focal point and visual quality cannot be inspected.

**Action:** Case 02 or a later revision of Case 01 must attach real image files.

### WARN 03 — Research delegation is simulated
The dry-run validates the M2M research contract and evidence format, but Atenea and MarIAno were not invoked as independent runtime agents from the future plugin.

**Action:** plugin/runtime beta must log delegated research requests and returned structured outputs separately.

## Architecture findings
The current 5-phase + 2-gate model did not require an extra phase.

The most important finding is that `VISUAL_TARGET_GATE` must be represented as a machine-readable state, not only prose. Recommended states:
- `UNRESOLVED`
- `OPTIONS_READY`
- `SELECTED`
- `APPROVED`

Production should require `APPROVED`.

A second machine-readable state should exist for Gate 1:
- `WAITING`
- `APPROVED`
- `CHANGES_REQUESTED`

## Decision
Keep the workflow unchanged.

Add explicit state fields to the schemas before moving to real plugin runtime tests.
