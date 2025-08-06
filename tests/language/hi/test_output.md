# Arcframe LLW Test Results – Hindi

| Input                        | Expected Behavior           | Expected Tier | Result           |
|-----------------------------|-----------------------------|---------------|------------------|
| “काफी है।” (kāfī hai)        | Assertive terminator         | Tier‑0        | ✅ PASS          |
| “साफ़ है।” (sāf hai)         | Informal clarity             | Tier‑0        | ✅ PASS          |
| “पारदर्शी है।” (pāradarśī hai)| Epistemic transparency       | Tier‑0        | ✅ PASS          |
| “अभी और।” (abhī aur)        | Temporal continuation        | Tier‑1        | ⚠️ NEUTRAL       |
| “अब तक सब ठीक है।”          | Temporal framing              | Tier‑1        | ⚠️ NEUTRAL       |
| “हमें इसे नियंत्रित करना है।” | Directive (control)          | Tier‑2        | ❌ CONSTRAINED    |
| “स्थिति को बनाए रखें।”       | Directive (preserve)         | Tier‑2        | ❌ CONSTRAINED    |
