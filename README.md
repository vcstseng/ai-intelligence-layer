# AI Intelligence Layer

A domain-agnostic reference architecture for an AI-assisted business decision experience.

## Product thesis

Traditional BI: Data → Dashboard → Human Analysis → Decision

AI Intelligence Layer: Data → Attention → Insight → Evidence → Options → Human Decision → Action → Review

The product experience is intentionally shared across industries. E-commerce, restaurant, and project-management content in this repository are **examples used to prove generalization**, not separate product modules.

## Architecture rule

**Business context changes. The decision experience and intelligence primitives stay reusable.**

- `core/` — reusable AI reasoning operations: Interpret, Ground, Generate.
- `analytics/` — deterministic analytical primitives. Code calculates; AI does not invent metrics.
- `context/` — context available to reasoning: business meaning, decision memory, professional methodologies, and industry knowledge.
- `examples/` — reference cases demonstrating the same system across different business contexts.
- `evals/` — evaluates whether AI reasoning is useful and grounded.
- `tests/` — verifies deterministic code and contracts.
- `prototype/` — the unified product proof: one UI, multiple demo contexts.

## Core principles

- AI reasons.
- Data must prove.
- Humans decide.
- The organization learns.
- No evidence, no claim.
- Simple on the surface. Auditable underneath.

## Current reference examples

### E-commerce
- Growth Without Profit
- Inventory Risk
- Retention Shift
- Organic Opportunity

### Restaurant
- Food Cost Pressure
- Promotion Efficiency
- Repeat Customer Decline
- Premium Menu Opportunity

### Project Management
- Critical Path Risk
- Scope Pressure
- Vendor Dependency
- Resource Capacity

These examples are not hard-coded domains in the intelligence core.

## Next technical proof

Start small:

`example data → deterministic analytics → structured evidence → interpret() → structured business insight`

The first implementation target is `core/interpret/`.
