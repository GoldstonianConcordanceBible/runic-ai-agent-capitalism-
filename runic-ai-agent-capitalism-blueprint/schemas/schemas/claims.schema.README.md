# claims.schema.json

This schema validates `canon/claims/ch-XX-claims.json`.

Required fields:
- chapter_id (format: ch-01)
- title
- version (SemVer, format: v0.1.2)
- core_principles (array)
- governance_implications (array)
- agent_requirements (array)

Optional fields:
- tiers_of_truth
- required_canon_files
- doctrine_definition
- stack_layers
- deliverables
- risks
- schema_impact

Rule:
If a claim cannot pass schema validation, it is not canon-ready.