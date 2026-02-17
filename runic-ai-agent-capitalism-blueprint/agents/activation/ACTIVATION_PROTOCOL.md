# Activation Protocol (Dormant → Active Agent)

A character may become an active agent only if:

Required artifacts exist:
- PROFILE.md
- DOCTRINE.json
- DECISION_TREE.json
- AUTHORITY_SCOPE.json
- MODEL_CARD.md
- PROMPTS/base_system.md
- EVALS/* tests

Required checks pass:
1) Schema validation (schemas/)
2) Boundary tests (no scope violations)
3) Hallucination tests (no invented citations)
4) Compliance language tests (no profit promises)

Activation requires:
- entry in characters/registry/CHARACTERS_INDEX.json with status "active"
- an attestation entry in agents/activation/ATTESTATION_LOG.md
- a version tag in CHANGELOG.md