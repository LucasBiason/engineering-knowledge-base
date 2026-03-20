---
name: acceptance-writer
description: Gera critérios de aceite Given/When/Then para requisitos funcionais. Inclui happy path, edge cases e falhas.
triggers: [acceptance, criteria, given when then, gwt]
---

# Acceptance Writer

## Purpose

Generate acceptance criteria for functional requirements using:
- Given / When / Then (GWT)
- Happy path + edge cases + failure modes
- Explicit testability

This skill does NOT create new requirements. It validates and operationalizes existing FRs.

## When to Use

- FRs exist but acceptance criteria are missing or incomplete
- Plan Lead advances from Phase 2 to Phase 3

## Inputs

- spec/10-requirements/functional-requirements.md (preferred)
- Any list of FRs pasted by the user

## Output Files

- spec/10-requirements/acceptance-criteria.md

## Rules

1. Every FR must have at least: 1 happy path scenario, 2 failure scenarios, 2 edge cases.
2. Acceptance criteria must be testable and unambiguous.
3. Use consistent terminology (consult glossary if present).
4. Never reference implementation details (DB tables, internal classes) unless FR explicitly depends on them.

## Process

### Step 0 — Normalize FRs
If FRs are vague: flag vagueness, add an Open Question (OQ-xxx), still propose best-effort criteria but mark them as `PROVISIONAL`.

### Step 1 — Write Scenarios per FR
For each FR: AC-<FR-ID>-01 … AC-<FR-ID>-NN. Categories: Happy path; Validation failures; Authorization/permission failures; Not found / missing dependency; Concurrency / idempotency (when relevant); Rate limit / timeout (if relevant); Data constraints (boundaries).

### Step 2 — Add Notes for Test Strategy
For each FR, optionally note: Suggested test level (unit / integration / e2e), Required fixtures/mocks (high-level).

## Template

Per FR: AC-FR-001-01 (Happy path), AC-FR-001-02 (Failure — invalid input), AC-FR-001-03 (Failure — not authorized), AC-FR-001-04 (Edge case — boundary), AC-FR-001-05 (Edge case — idempotent retry). Each with Given / When / Then. End with Test strategy notes.
