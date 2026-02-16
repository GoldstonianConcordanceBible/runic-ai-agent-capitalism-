# The Blackbook Framework

The Blackbook is the operational constitution for agents.

Every agent requires:

## 1. Canon Layer
- CANON_INDEX.json
- GLOSSARY.md
- DOCTRINE.md
- INTERPRETIVE_RULES.md

## 2. Provenance Layer
- CITATION.cff
- CHANGELOG.md
- Releases + tags
- ATTESTATION_LOG.md

## 3. Agent Layer
- AGENTS/<agent_name>/MODEL_CARD.md
- AGENTS/<agent_name>/PROMPTS/
- AGENTS/<agent_name>/EVALS/
- AGENTS/<agent_name>/RUNBOOK.md

Agents without canon drift.
Agents without provenance hallucinate.
Agents without evals decay.