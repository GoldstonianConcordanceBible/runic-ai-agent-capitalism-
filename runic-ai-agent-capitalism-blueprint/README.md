# The Runic Consulting Guide to AI Agent Capitalism — Blueprint Repo

This repository is the production template that turns:
**Book chapters → Blackbook canon → Character specs → Deployable agents**

Primary goals:
1) Readers ship an AI agent MVP using canon + provenance + evals.
2) Goldston can reuse this blueprint across 120+ books so any character can become an agent at any time.

Core pattern:
**Canon → Index → Schemas → Provenance → Prompts → Releases → Agents**

## What’s Inside
- `/manuscript/` : book writing workspace
- `/blackbook/`  : roadmap + workflow to turn chapters into system artifacts
- `/canon/`      : canonical truth layer (agent-safe)
- `/schemas/`    : JSON schemas to keep everything consistent
- `/characters/` : “Character → Agent” conversion standard (CCACS)
- `/agents/`     : agent runbooks, model cards, activation protocol
- `/governance/` : contribution-only DAO governance + communication rules

## Production-Ready Principles
- Agents must cite canon and never invent.
- Changes are versioned (tags + changelog).
- Every character/agent has authority boundaries and tests.

See: blackbook/BLACKBOOK_WORKFLOW.md