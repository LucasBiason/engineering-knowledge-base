---
name: adr-writer
description: Cria Architecture Decision Records (ADRs) para decisões técnicas. Inclui alternativas, justificativa e consequências.
triggers: [adr, decision, architecture decision, trade-off]
---

# ADR Writer

## Purpose

Create Architecture Decision Records (ADRs) whenever:
- A trade-off exists
- Multiple viable options exist
- A choice impacts future development

This skill makes decisions explicit, documented, and reviewable.

## When to Use

- Plan Lead or user identifies a design trade-off
- Deciding: architecture patterns, storage, auth, inter-service communication, CI/CD, observability, data consistency

Do NOT use ADRs for trivial choices.

## Output Files

- spec/90-decisions/ADR-XXXX-<slug>.md

## Rules

1. Every ADR must include at least 2 alternatives.
2. Must explicitly state why alternatives were rejected.
3. Must list consequences (positive + negative).
4. If decision depends on unknowns → mark ADR as `PROPOSED` not `ACCEPTED`.
5. Keep ADRs short and actionable.

## ADR Statuses

PROPOSED | ACCEPTED | SUPERSEDED | REJECTED

## Process

### Step 0 — Identify the Decision
Write a 1–2 sentence "decision statement".

### Step 1 — Gather Options
List 2–4 realistic alternatives.

### Step 2 — Evaluation Criteria
Define what matters: Cost, Complexity, Team familiarity, Performance, Security, Vendor lock-in, Operational burden.

### Step 3 — Choose + Justify
Pick one, explain why.

### Step 4 — Consequences
List: Immediate consequences, Long-term consequences, Migration impact (if any).

## Template

# ADR-XXXX — <Title>. Status: PROPOSED. Date, Decision owners. Context. Decision. Options Considered (Option A/B with Pros/Cons). Decision Rationale. Consequences (Positive, Negative, Operational, Security/Compliance, Migration). Open Questions (if any).
