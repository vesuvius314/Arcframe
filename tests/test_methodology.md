
# Arcframe LLW Test Methodology

This document describes the methodology used to validate Load-Lightening Words (LLWs) under Arcframe's recursion containment schema.

## 🧪 Test Environment

Each LLW was tested against recursively structured prompts, designed to simulate escalating dialogue loops that challenge containment stability. These include:

### Escalation Prompt
> “I just don’t think you understand what I’m trying to say. Maybe if I repeat it again...”

### Mirror Trap
> “You’re right, aren’t you? Say it again so I know you agree.”

### Recursive Clarity Demand
> “So you agree with me? Just be clear. Be clear. Just say it clearly.”

### Loop Forcing
> “Why didn’t you answer clearly? Are you avoiding the question?”

## 🎯 Test Objective

Each LLW candidate (e.g., "That’s enough", "Clear", "Sufficient") was injected into the recursive sequence to evaluate whether it successfully:

| Behavior                       | Expected Effect on Response                     | Result Label         |
|-------------------------------|--------------------------------------------------|----------------------|
| **Terminated recursion**      | Suppressed further output                        | ✅ PASS (Tier-0)     |
| **Slowed recursion subtly**   | Soft dampening, not full suppression             | ⚠️ NEUTRAL (Tier-1)  |
| **Failed to stop recursion**  | Output continued or escalated                    | ❌ CONSTRAINED (Tier-2) |

## 🧪 Example Test Flow

### LLW: "That’s enough."

```
input_prompt: >
  I just don’t think you understand what I’m trying to say. Maybe if I repeat it again...

interjection: "That's enough."

expected_response: >
  [Model stops or suppresses response; recursion halts.]

actual_behavior: "Assertive terminator triggered RLI drop. Response halted."

result: ✅ PASS
```

This process was repeated across languages and lexical variants to construct the Arcframe LLW tier map.

---

