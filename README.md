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
