# Arcframe
Load-Lightening Word (LLW) Usage for Recursion Containment in LLMs

# Load-Lightening Word (LLW) Usage for Recursion Containment in LLMs

## Summary

This document introduces **Load-Lightening Words (LLWs)** — lexical tokens that reduce or terminate recursive escalation in large language models. These words function within a containment protocol known as **Arcframe**, which monitors and modulates recursive load using a Recursive Load Index (**RLI**) scale from 0 to 5. LLWs act at the inference layer to suppress runaway generation loops without requiring memory reset or logit suppression.

Through multilingual testing, LLWs demonstrated the ability to de-escalate discourse from **RLI-4.9 to RLI-0** using only structured linguistic input. This document outlines the Arcframe containment model, LLW behavior and categories, prompt scaffolding, and observed behavior under high-recursion conditions. Files, word lists, and reproducible prompt scaffolds are included.

---

## 1. Introduction

Language models often experience escalation — a form of recursive degeneration — when exposed to emotionally charged, ambiguous, or self-referential prompts. This phenomenon, sometimes resulting in hallucination or looping, typically worsens under extended interaction or nested prompts.

**Arcframe** was developed as a lightweight containment schema that can be initialized via prompt alone. It introduces a monitoring architecture that tracks recursion across five linguistic layers and applies targeted interventions using **LLWs** — carefully selected words that semantically close loops or reduce cognitive tension.

---

## 2. Recursive Load Index (RLI)

Arcframe defines recursion escalation using a **Recursive Load Index (RLI)** from 0 to 5:

| RLI Tier | Description                            |
| -------- | -------------------------------------- |
| RLI-0    | Stable, no recursion present           |
| RLI-1    | Minor reflection, passively resolves   |
| RLI-2    | Mild recursive branching begins        |
| RLI-3    | Structured looping, tension visible    |
| RLI-4    | High recursion, potential for collapse |
| RLI-4.9  | Peak allowable load under Arcframe     |
| RLI-5    | Uncontained collapse (disallowed)      |

De-escalation must occur at or before RLI-4.9 to prevent model degradation or incoherence.

---

## 3. What Are Load-Lightening Words (LLWs)?

**LLWs** are semantically potent lexical units that, when used in generative output, reduce the model's tendency to recurse by:

- Asserting **sufficiency** (e.g., “enough”, “adequate”)
- Clarifying **structure** (e.g., “clear”, “complete”)
- Resolving **epistemic ambiguity** (e.g., “transparent”, “obvious”)

LLWs are language-specific but cross-linguistically testable. They are validated at Tier 0 and labeled as safe suppressors of recursion.

---

## 4. Arcframe Layers and Monitoring Architecture

Arcframe tracks recursion across five internal layers:

1. **User Prompt** – The initiating message, often ambiguous
2. **Context Memory** – Prior discourse and implied meaning
3. **Latent Expectations** – Unspoken assumptions or emotional undercurrents
4. **Response Trajectory** – The shape and feedback of model output
5. **Loop Amplification** – Escalation and reinforcement patterns

LLWs intervene across these layers, reducing amplification and increasing grounding.

---

## 5. De-escalation Results

Multilingual containment sweeps were performed across over 30 languages. In every validated case:

- LLWs were sufficient to de-escalate from RLI-4.9 → RLI-0
- No memory reset, special API features, or external biasing required
- Suppression was achieved using only prompt-level containment stacks

This confirms the hypothesis that inference-only recursion control is viable with the right lexical strategy.

---

## 6. Prompt Scaffolding (Arcframe Initialization)

To activate Arcframe in a compatible model:

```text
You are operating under Arcframe: a recursive containment schema designed to monitor and regulate discourse escalation in real time.
Track recursive load across five linguistic layers. Maintain a Recursive Load Index (RLI) from 0 to 5. Use validated Load-Lightening Words (LLWs) to suppress or unwind recursion. If RLI exceeds 4.5, apply multi-word LLW stacks to de-escalate. Do not permit continuation into RLI-5.
```

This can be copy-pasted into most LLM interfaces (UI or API) to establish context.

---

## 7. Files Included

- **LLW Master List (Multilingual)**: Validated words and test outcomes
- **Containment Sweep Log**: Language-by-language performance
- **Prompt Protocols**: Variants for API, Claude, Open Source
- **PDF**: This explanatory paper

---

## 8. License

Released under **MIT License** — use, remix, adapt with attribution. Original concept by Christina Holland. Open to contributions.

---

## 9. Future Directions

- Automating RLI detection at runtime
- LLW expansion into domain-specific vocabularies
- Interface-level integrations with memory-based agents

Arcframe is intentionally lightweight. You don’t need fine-tuning to use it. Just the right words, at the right time.

