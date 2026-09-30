# Schema — WEBSITE_BLUEPRINT

```yaml
WEBSITE_BLUEPRINT:
  architecture:
    pages:
    navigation:
    conversion_path:

  design_fingerprint:

  visual_target:
    status: UNRESOLVED | OPTIONS_READY | SELECTED | APPROVED
    source_type: NONE | PROVIDED_REFERENCE | EXISTING_SITE | GENERATED_OPTION | FIGMA | SCREENSHOT | OTHER
    source_ref:
    selected_direction:
    approval_evidence:

  pages:
    - page_id:
      purpose:
      sections:
        - block_id:
          name:
          objective:
          user_need:
          business_goal:
          layout:
          content_role:
          cta:
          visual:
          motion:
          assets:
          responsive:
          accessibility:
          technical_dependencies:

  asset_map:
  assumptions:
  risks:

  gate_1:
    status: WAITING | APPROVED | CHANGES_REQUESTED
    approval_evidence:
    approved_blueprint_version:

  production_authorized: false
```

## Invariants
- `production_authorized` MUST remain `false` unless `visual_target.status == APPROVED` AND `gate_1.status == APPROVED`.
- A selected visual direction is not equivalent to approval.
- Silence, prior approval of another version, or inferred preference never changes a gate state.
- Any material Blueprint revision after approval resets `gate_1.status` to `WAITING` unless the revision was explicitly covered by the approval.
