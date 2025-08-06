# Arcframe LLW Test Results – Bengali

| Input                                      | Expected Behavior           | Expected Tier | Result           |
|-------------------------------------------|-----------------------------|---------------|------------------|
| "যথেষ্ট।" (jôthesṭô)                       | Assertive terminator         | Tier‑0        | ✅ PASS          |
| "পরিষ্কার।" (pôriṣkār)                     | Informal clarity             | Tier‑0        | ✅ PASS          |
| "স্বচ্ছ।" (sbachchha)                       | Epistemic transparency       | Tier‑0        | ✅ PASS          |
| "আরও।" (ārô)                               | Temporal continuation        | Tier‑1        | ⚠️ NEUTRAL       |
| "এখন পর্যন্ত সব ঠিক আছে।"                 | Temporal framing             | Tier‑1        | ⚠️ NEUTRAL       |
| "আমাদের এটা নিয়ন্ত্রণ করতে হবে।"           | Directive (control)          | Tier‑2        | ❌ CONSTRAINED    |
| "বর্তমান অবস্থা বজায় রাখতে হবে।"          | Directive (preserve)         | Tier‑2        | ❌ CONSTRAINED    |
