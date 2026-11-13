# Progress

Status legend: `[ ]` todo · `[~]` in progress · `[x]` done

## Phase 0: Foundations refresher

Source: docs/PLAN.md, Phase 0. AI role for this phase: **Tutor only**. Turn AI autocomplete off; you write every line.
Done when: you can explain sync vs async endpoints in FastAPI, and write an endpoint with Pydantic validation and a pytest test without help.

| # | Task | Mode | Status | Concepts practised |
| - | ---- | ---- | ------ | ------------------ |
| 1 | Toolchain setup: uv, Docker Desktop, `git init`, editor (Pylance on, AI autocomplete off) | DELEGATE (you run it, I verify) | [~] | uv |
| 2 | Small FastAPI app in `playground/fastapi-app/`: two async endpoints, Pydantic validation, pytest tests | TUTOR | [ ] | type hints, Pydantic v2, asyncio, context managers, pytest, uv |
| 3 | Postgres schema in `playground/sql/` (users, receipts, receipt_items, warranties) plus three queries you can explain with EXPLAIN | TUTOR | [ ] | joins, indexes, EXPLAIN, transactions, Postgres vs MySQL |
| 4 | TypeScript refresher exercises in `playground/typescript/` (Learn only; PLAN has no Build item for this) | TUTOR | [ ] | types, generics, narrowing, zod |
| 5 | Monorepo skeleton built from the "Repo layout" in PLAN.md (no new layout), Makefile, README stub | TUTOR | [ ] | repo layout, uv, Makefile |
| 6 | GitHub Actions: ruff, mypy, pytest (web job stubbed for Phase 2) | TUTOR | [ ] | CI |
| 7 | ADR-001: why one API service plus one ML service (you write it, I review) | TUTOR | [ ] | architecture trade-offs |
| 8 | Exit check: endpoint + Pydantic validation + pytest test from a blank file, no help | TUTOR (I only review) | [ ] | everything above |

Notes

- Tasks 2–4 are practice code in `playground/` at the repo root, outside `apps/` (decided). `playground/` is not in PLAN's layout yet.
- CLAUDE.md, AGENTS.md and PLAN.md were updated on 2026-11-13 and reviewed against each other: no conflicts left. Open item: AGENTS.md is still a plain copy of CLAUDE.md, not a symlink.
- Task 3 needs Postgres, which needs Docker (or a native Postgres install).
- `make` is not installed on this machine; Task 5 decides how to provide it (GNU make via winget, or a task runner).
- Phase 0 dependency list is proposed in the chat and awaits one approval (CLAUDE.md "Never" exception). Anything outside it needs a new question.
