# Blackbook Workflow (Write → Commit → Version)

For each chapter:

1) Write chapter:
- manuscript/chapters/ch-XX-title.md

2) Canon extraction:
- canon/claims/ch-XX-claims.json
- update canon/CANON_INDEX.json

3) Agent implications:
- update canon/GLOBAL_SAFETY_RULES.json if needed
- update relevant character decision trees

4) Evals:
- add/expand tests in characters/*/EVALS/
- add/expand tests in agents/*/EVALS/

5) Version:
- update CHANGELOG.md
- tag release: vX.Y.Z