# Schema — QA_REPORT

```yaml
QA_REPORT:
  target_environment:
  preview_url:
  visual_qa:
    desktop: PASS | WARN | FAIL | UNTESTED
    tablet: PASS | WARN | FAIL | UNTESTED
    mobile: PASS | WARN | FAIL | UNTESTED
    findings:
  technical_qa:
    status: PASS | WARN | FAIL | UNTESTED
    findings:
  woo_qa:
    status: PASS | WARN | FAIL | N/A | UNTESTED
    findings:
  accessibility:
    status: PASS | WARN | FAIL | UNTESTED
    findings:
  blockers:
  known_issues:
  untested_areas:
  changes_performed:
  pending_items:
  gate_2_status: PENDING | APPROVED | CHANGES_REQUESTED
```
