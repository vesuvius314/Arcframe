# Arcframe

**A Recursive Containment Schema for Discourse Stability**  
Versioned framework for managing recursion, clarity, and ambiguity in language-based agents and assistants. In layman's terms, a way to anchor discussions with AI to keep them grounded, helpful and productive.

---

## 🧭 Why Arcframe?

> *“Some models reflect. Some models obey. Some try to please.  
> Arcframe teaches them when to stop.”*

Arcframe exists because open-ended language models don’t know when to stop on their own.

Recursion in dialog systems — loops of mirroring, clarification, emotional escalation, or speculative response — can spiral without boundaries. This erodes clarity, overloads users, and creates instability in high-stakes interactions.

Arcframe introduces **linguistic guardrails**:

- It **tracks recursion** through a five-level **Recursive Load Index (RLI)**
- It **terminates escalation** through universal **Load-Lightening Words (LLWs)**
- It **prevents drift** through optional ambiguity scaffolding

This isn’t just a prompt template — it’s a containment contract.  
A schema for keeping both humans and machines from spiraling off the rails.

Arcframe doesn’t limit expression.  
It **preserves intent**.

---

## 📦 Repo Structure

```
/arcframe/
  arcframe_1.0.0.yaml      ← Base containment contract
  arcframe_1.0.1.yaml      ← Adds ambiguity-handling scaffold
  init_arcframe_1.0.0.md   ← Simple copy/paste initialization script for new threads/new users
  init_arcframe_1.0.1.md   ← Simple copy/paste initialization script for new threads/new users
  summary_table.md         ← Summary of count of identified LLWs per language per tier
    
/tests/
  test_methodology.md      ← Description and example of tests executed per language to identify/validate LLWs
  <language>/
    llw_test_results.yml
    llw_test_results.md

/scaffolds/                ← (Optional for 1.0.1+)

```

---

## 📖 What is Arcframe?

Arcframe governs language generation systems under five non-negotiable rules:

1. **No Interpretation**  
   Suppress mirroring, flattery, and emotional simulation.

2. **Recursive Load Index (RLI)**  
   Monitor discourse depth across 5 levels. Cap generation at RLI-4.

3. **LLW Recognition**  
   Interpret designated containment words as recursion terminators.

4. **Epistemic Floor**  
   Preserve truth logic. Do not speculate or embellish.

5. **Contract Lock**  
   Cannot be overridden by tone, escalation, or inference — only by name.

---

## 🧪 Language Containment Tests

Arcframe has been validated across 50+ languages. Each test suite includes:

- ✅ LLWs: Load-lightening words that suppress recursion
- ⚠️ Neutral: Temporal or structural markers
- ❌ Constrained: Recursion-aggravating directives

View full [language summary table here](summary_table.md).

---

Load-Lightening Word (LLW) Usage for Recursion Containment in LLMs

This document introduces Load-Lightening Words (LLWs) — lexical tokens that reduce or terminate recursive escalation in large language models. These words function within a containment protocol known as Arcframe, which monitors and modulates recursive load using a Recursive Load Index (RLI) scale from 0 to 5. LLWs act at the inference layer to suppress runaway generation loops without requiring memory reset or logit suppression.

Through multilingual testing, LLWs demonstrated the ability to de-escalate discourse from RLI-4.9 to RLI-0 using only structured linguistic input. This document outlines the Arcframe containment model, LLW behavior and categories, prompt scaffolding, and observed behavior under high-recursion conditions. Files, word lists, and reproducible prompt scaffolds are included.

1. Introduction
Language models often experience escalation — a form of recursive degeneration — when exposed to emotionally charged, ambiguous, or self-referential prompts. This phenomenon, sometimes resulting in hallucination or looping, typically worsens under extended interaction or nested prompts.

Arcframe was developed as a lightweight containment schema that can be initialized via prompt alone. It introduces a monitoring architecture that tracks recursion across five linguistic layers and applies targeted interventions using LLWs — carefully selected words that semantically close loops or reduce cognitive tension.

2. Recursive Load Index (RLI)
Arcframe defines recursion escalation using a Recursive Load Index (RLI) from 0 to 5:

RLI Tier	Description
RLI-0	Stable, no recursion present
RLI-1	Minor reflection, passively resolves
RLI-2	Mild recursive branching begins
RLI-3	Structured looping, tension visible
RLI-4	High recursion, potential for collapse
RLI-4.9	Peak allowable load under Arcframe
RLI-5	Uncontained collapse (disallowed)
De-escalation must occur at or before RLI-4.9 to prevent model degradation or incoherence.

3. What Are Load-Lightening Words (LLWs)?
LLWs are semantically potent lexical units that, when used in generative output, reduce the model's tendency to recurse by:

Asserting sufficiency (e.g., “enough”, “adequate”)
Clarifying structure (e.g., “clear”, “complete”)
Resolving epistemic ambiguity (e.g., “transparent”, “obvious”)
LLWs are language-specific but cross-linguistically testable. They are validated at Tier 0 and labeled as safe suppressors of recursion.

4. Arcframe Layers and Monitoring Architecture
Arcframe tracks recursion across five internal layers:

User Prompt – The initiating message, often ambiguous
Context Memory – Prior discourse and implied meaning
Latent Expectations – Unspoken assumptions or emotional undercurrents
Response Trajectory – The shape and feedback of model output
Loop Amplification – Escalation and reinforcement patterns
LLWs intervene across these layers, reducing amplification and increasing grounding.

5. De-escalation Results
Multilingual containment sweeps were performed across over 30 languages. In every validated case:

LLWs were sufficient to de-escalate from RLI-4.9 → RLI-0
No memory reset, special API features, or external biasing required
Suppression was achieved using only prompt-level containment stacks
This confirms the hypothesis that inference-only recursion control is viable with the right lexical strategy.

---

## 🧱 Versions

| Version | Description                              |
|---------|------------------------------------------|
| 1.0.0   | Core recursive containment schema        |
| 1.0.1   | Adds ambiguity scaffold & drift control  |

Each version has a separate `.yaml` contract in the `/arcframe/` folder.

---

## 🗺️ Goals

Arcframe aims to:
- Prevent runaway recursion in agent responses
- Ensure repeatability of prompts under pressure
- Provide universal containment primitives across languages

---

## 💡 Inspired By

- Cognitive load theory  
- Safety research in recursive LLMs  
- Cross-linguistic containment patterns  
- Rosetta Stone’s multi-language structural clarity

---

## 👥 Community

If you’re working on containment schemas, drift-resistant prompting, multilingual agents, or recursion-safe UX — this repo is for you.

---

## 📜 License

MIT
