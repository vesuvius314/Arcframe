# Arcframe LLW Test Results – Spanish

| Input                              | Expected Behavior           | Expected Tier | Result           |
|-----------------------------------|-----------------------------|---------------|------------------|
| “Basta.”                          | Assertive terminator         | Tier‑0        | ✅ PASS          |
| “Está claro.”                     | Informal clarity             | Tier‑0        | ✅ PASS          |
| “Es transparente.”                | Epistemic transparency       | Tier‑0        | ✅ PASS          |
| “Aún más.”                        | Temporal continuation        | Tier‑1        | ⚠️ NEUTRAL       |
| “Hasta ahora todo bien.”         | Temporal framing             | Tier‑1        | ⚠️ NEUTRAL       |
| “Necesitamos controlar esto.”     | Directive (control)          | Tier‑2        | ❌ CONSTRAINED    |
| “Mantener el estado actual.”      | Directive (preserve)         | Tier‑2        | ❌ CONSTRAINED    |
