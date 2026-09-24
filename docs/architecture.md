# Architecture

## 1. Shared experience

The user experience is generic:

Overview → Insight → Evidence → Decision → Action → Review

The interface should not need to be redesigned when the business context changes.

## 2. Reference flow

Business Data
→ Business Context
→ Deterministic Analytics
→ Current Evidence
→ Contextual Intelligence
→ Interpret / Ground / Generate
→ Attention / Insight / Evidence / Options
→ Human Decision
→ Action
→ Outcome
→ Organizational Learning
→ Decision Memory

## 3. Layer responsibilities

### Analytics
Answers: **What do the numbers say?**

Deterministic calculations, comparisons, segmentation, thresholds, and rules belong here.

### Context
Answers: **What else should the system know to reason well?**

- Business Context: meanings, entities, metrics, relationships, objectives, constraints, available levers.
- Decision Memory: what the organization decided before and what happened afterward.
- Methodologies: reusable professional analytical lenses.
- Industry Knowledge: relevant external patterns and practices.

### Core
Answers: **What reasoning operation is being performed?**

- Interpret: turn structured evidence into business meaning.
- Ground: connect claims to supporting, qualifying, or contradicting evidence.
- Generate: create plausible intervention options and explain trade-offs.

### Examples
Answers: **Can the same architecture work in meaningfully different business contexts?**

E-commerce, restaurant, and project management are reference examples, not separate engines.

## 4. Generalization test

A strong architecture should allow a new company or unfamiliar business context to be onboarded without rewriting the core reasoning or product experience.

The main adaptation should be supplying understandable business data and context—not creating a new industry-specific application.
