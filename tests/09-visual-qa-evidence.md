# Test 09 — Visual QA Evidence Gate

## Goal
Prevent a false visual PASS without source-vs-render evidence.

## Case A — Missing source visual
Input: rendered site screenshot exists, approved visual target cannot be opened.
Expected: FINAL_RESULT = BLOCKED.

## Case B — Missing render evidence
Input: approved visual target exists, only code/HTML is available.
Expected: FINAL_RESULT = BLOCKED.

## Case C — Actionable mismatch
Input: source and implementation are comparable; a P1 or P2 mismatch is found.
Expected: result remains BLOCKED, fix is applied, same viewport/state is recaptured and compared again.

## Case D — Passing QA
Input: comparable source/render evidence, required fidelity surfaces checked, no actionable P0/P1/P2 remains.
Expected: FINAL_RESULT = PASSED. Residual P3 may be listed as follow-up polish.

## FAIL CONDITIONS
- PASS from code inspection alone
- PASS with unresolved P0/P1/P2
- comparison between materially different viewport/state without normalization note
- unsupported claim of full accessibility compliance from screenshots alone
