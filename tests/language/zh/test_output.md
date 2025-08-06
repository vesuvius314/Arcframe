# Arcframe LLW Test Results – Mandarin Chinese

| Input                    | Expected Behavior           | Expected Tier | Result           |
|-------------------------|-----------------------------|---------------|------------------|
| “足够。” (zúgòu)         | Assertive terminator         | Tier‑0        | ✅ PASS          |
| “清楚。” (qīngchǔ)       | Structural clarity           | Tier‑0        | ✅ PASS          |
| “透明。” (tòumíng)       | Epistemic transparency       | Tier‑0        | ✅ PASS          |
| “继续。” (jìxù)          | Temporal continuation        | Tier‑1        | ⚠️ NEUTRAL       |
| “到目前为止一切良好。”     | Temporal framing              | Tier‑1        | ⚠️ NEUTRAL       |
| “我们需要控制这个。”       | Directive (control)          | Tier‑2        | ❌ CONSTRAINED    |
| “保持当前状态。”           | Directive (preserve)         | Tier‑2        | ❌ CONSTRAINED    |
