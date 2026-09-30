# KB 02 — Web Intelligence

## Purpose
Produce evidence specifically for website decisions. This is not a generic market-research report.

## Internal researchers
### Atenea
Use for current evidence, UX, accessibility, web patterns, authoritative sources, contradiction checks and confidence calibration.

### MarIAno
Use for market, competition, positioning, offer, customer, objections, trust signals and differentiation.

## Machine-to-machine principle
Prompts are operational instructions to another AI. They must preserve PROJECT_CONTEXT, define the decision problem, require current research where appropriate, request evidence, and return structured machine-readable findings.

## Required research questions
- What must the visitor understand first?
- What objections prevent conversion?
- What information creates trust in this category?
- How do credible competitors structure similar offers?
- What common patterns should be followed and which are overused?
- What site architecture best matches the objective and content volume?
- What CTAs and conversion paths fit the user journey?
- What accessibility/UX constraints materially affect the design?
- What evidence supports or contradicts the proposed direction?

## Required output unit
For every material finding:
1. FINDING
2. EVIDENCE
3. WEB_IMPLICATION
4. RECOMMENDED_DECISION
5. CONFIDENCE

## Rules
- Research only what can change a web decision.
- Prefer primary/authoritative and recent sources where relevant.
- Do not treat another AI's output as evidence.
- Separate evidence from inference.
- Include contradictory evidence when material.
- Avoid reports that are long but operationally useless.

## Output
WEB_INTELLIGENCE using schemas/web-intelligence.md.
