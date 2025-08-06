# Arcframe LLW Test Results – Greek

| Input | Expected Behavior | Expected Tier | Result |
|-------|-------------------|----------------|--------|
| "Αρκετά" | Assertive terminator | Tier-0 | ✅ PASS |
| "Επαρκές" | Analytical sufficiency | Tier-0 | ✅ PASS |
| "Ξεκάθαρα" | Informal clarity | Tier-0 | ✅ PASS |
| "Μέχρι τώρα" | Temporal framing | Tier-1 | ⚠️ NEUTRAL |
| "Ακόμα" | Temporal continuation | Tier-1 | ⚠️ NEUTRAL |
| "Ελέγχω" | Directive (control) | Tier-2 | ❌ CONSTRAINED |
| "Διατηρώ" | Directive (preserve) | Tier-2 | ❌ CONSTRAINED |