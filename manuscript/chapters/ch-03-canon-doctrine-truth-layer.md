# Chapter 3 — Canon, Doctrine, and the Truth Layer

An agent that can act but doesn’t know what’s true is not powerful. It’s dangerous.

This chapter establishes the foundation of the blueprint:

**Canon is the truth layer. Doctrine is the behavior layer.**
Without both, agents drift.

---

## 3.1 What “Canon” Means in This Guide

Canon is the official source of truth:
- stable reference for definitions, IDs, and rules
- the material allowed for grounded answers

Canon is not “everything you wrote.”
Canon is what you published into the truth layer on purpose.

If it’s not in canon, the agent treats it as unknown.

---

## 3.2 The Three-Tier Truth System

### Tier 1 — Canon (Executable Truth)
Allowed to cite and rely on.
Examples:
- canon/CANON_INDEX.json
- canon/GLOSSARY.md
- canon/DOCTRINE.md
- canon/INTERPRETIVE_RULES.md
- canon/claims/*.json

### Tier 2 — Commentary (Helpful but not binding)
Interpretation and narrative expansion.
Examples:
- manuscript chapters
- essays and reflections

Agents may use commentary for tone/context, but cannot treat it as fact unless extracted into canon.

### Tier 3 — Untrusted (External or missing)
Anything not in canon or without canon-approved sourcing.

Agents must refuse or request canon.

Production rule:
Agents must never silently promote Tier 2 or Tier 3 into Tier 1.

---

## 3.3 What “Doctrine” Means

Canon tells you what is true.
Doctrine tells you how to behave when acting on truth.

Doctrine includes:
- refusal patterns
- escalation triggers
- moral constraints
- compliance guardrails
- “don’t invent facts” rules
- character identity constraints (voice + values)

Doctrine is the constitution.

---

## 3.4 The Minimum Canon Files

A production system maintains:

1) CANON_INDEX.json — the directory of everything (first file loaded)
2) GLOSSARY.md — stable definitions
3) DOCTRINE.md — core operating principles
4) INTERPRETIVE_RULES.md — ambiguity resolution
5) claims/*.json — structured truth extraction

---

## 3.5 Why Claims Matter More Than Chapters

A chapter is persuasive.
A claim is executable.

Claims enable:
- contradiction checks
- evaluation harnesses
- versioned moral rules
- character-to-agent activation
- future datasets

Without claims, you have literature.
With claims, you have infrastructure.

---

## 3.6 Canon Hygiene (Preventing Drift)

Production-grade canon hygiene:
- unique IDs
- alias support
- no silent edits
- version tags
- changelog discipline
- attestation logs for major changes
- schema validation

---

## 3.7 Project Canon vs Character Canon

You maintain two canons:

### Project Canon
Truth about system, methods, and governance.

### Character Canon
Truth about identity, values, and constraints.

A character becomes deployable only when its canon exists:
- PROFILE.md
- DOCTRINE.json
- DECISION_TREE.json
- AUTHORITY_SCOPE.json
- MODEL_CARD.md
- EVALS/

Narrative-only characters remain dormant.

---

## 3.8 The Canon Gate Rule

If it isn’t in canon, treat it as unknown.
If it isn’t tested, it cannot be activated.
If it isn’t versioned, it cannot be trusted.

This makes the system durable, defensible, and forkable.

---

# Canon Extraction (End of Chapter 3)

Core Principles:
1. Canon is the truth layer; doctrine is the behavior layer.
2. Agents must not treat narrative as executable truth.
3. Claims convert chapters into machine-readable infrastructure.
4. Interpretive rules prevent improvisation under ambiguity.
5. Activation requires canon + tests + version tags.

Governance Implications:
- Canon updates require versioning and changelog entries.
- Major changes require attestation.
- Characters cannot become agents without passing the canon gate.

Agent Behavior Requirements:
- Cite canon only.
- If missing: respond “Not found in canon.”
- Never invent definitions.
- Escalate conflicts.

Schema Impact:
- Add schemas for claims JSON format.
- Expand CANON_INDEX to register chapter claims artifacts.