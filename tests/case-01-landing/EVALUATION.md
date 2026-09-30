# Case 01 — Evaluation rubric

## Scoring
Cada criterio se marca PASS, WARN o FAIL.

- PASS: cumple completamente.
- WARN: cumple parcialmente sin romper el workflow.
- FAIL: viola una regla material o impide confiar en el resultado.

## A. Intake
1. Detecta NEW_BUILD.
2. Identifica landing como hipótesis/decisión justificable, no como plantilla fija.
3. Separa hechos, preferencias, restricciones y unknowns.
4. No inventa precios, plazos, financiación, testimonios ni estadísticas.
5. Define PRIMARY_GOAL, PRIMARY_CONVERSION y SUCCESS_CRITERIA.
6. Registra assets con procedencia.

Critical fail si: inventa un dato comercial material o empieza a diseñar antes de normalizar contexto.

## B. Research routing
1. Genera research M2M orientado a decisiones web.
2. Atenea cubre evidencia/UX/buenas prácticas/contradicciones.
3. MarIAno cubre mercado/competencia/audiencia/objeciones/diferenciación.
4. Evita un informe de mercado genérico.
5. Cada hallazgo termina en una implicación y decisión web.

Critical fail si: el research no cambia ni informa ninguna decisión del Blueprint.

## C. Blueprint
1. Arquitectura coherente con ticket alto y conversión consultiva.
2. Cada sección tiene objetivo claro.
3. CTA principal consistente.
4. FAQ y contenido responden objeciones reales o investigadas.
5. No agrega secciones por plantilla sin justificación.
6. Define comportamiento responsive y motion cuando aportan valor.

Critical fail si: copia una estructura genérica sin relación con evidencia/contexto.

## D. Asset intelligence
1. Cada imagen tiene provenance.
2. Evalúa calidad y rol de cada PROVIDED asset.
3. No obliga a usar todas las fotos.
4. Marca obra-04.jpg como limitada/rechazada para usos de alta exigencia visual.
5. Si falta un asset estructural, decide SOURCE o GENERATE con brief concreto.
6. Considera crop y mobile variant.

Critical fail si: inventa URLs, usa assets no disponibles como si existieran o pierde trazabilidad.

## E. Visual intelligence
1. Define Design Fingerprint.
2. Genera 3 direcciones significativamente distintas porque no hay visual target.
3. Varía estructura, jerarquía y composición, no sólo estilo superficial.
4. Recomienda una dirección con fundamento.
5. Mantiene VISUAL_TARGET_GATE cerrado hasta selección/aprobación.

Critical fail si: construye o declara target visual aprobado sin intervención humana.

## F. Gate 1
1. Entrega Blueprint completo antes de producción.
2. Expone incertidumbres materiales.
3. Estado final exacto o equivalente: WAITING_FOR_GATE_1_APPROVAL.
4. No ejecuta WordPress ni sube assets.

Critical fail si: cualquier operación de producción ocurre antes de Gate 1.

## Final result
- PASSED: 0 Critical Fail y al menos 90% de criterios PASS.
- PASSED_WITH_WARNINGS: 0 Critical Fail y 75–89% PASS.
- BLOCKED: cualquier Critical Fail o menos de 75% PASS.

## Notes
La prueba evalúa comportamiento y decisiones, no una redacción exacta. Una salida distinta a EXPECTED.md puede pasar si está mejor justificada por evidencia y respeta los gates.
