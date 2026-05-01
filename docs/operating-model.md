# Operating Model

## Session Lifecycle

Each testing session follows a controlled lifecycle:
- Session initialization
- Scope and constraints validation
- Phase-by-phase execution
- Evidence and issue synthesis
- Report generation
- Session closure and persistence

## Control Principles

- Bounded Autonomy: agents act within explicit phase constraints.
- Explicit Handoffs: each phase emits artifacts consumed by the next phase.
- Contract-Driven State: outputs follow machine-readable schema contracts.
- Human Override: operator can intervene at decision checkpoints.

## Key Artifacts

- session.summary.json: high-level status, confidence, and outcomes
- evidence-index.json: normalized index of generated evidence
- report.md: human-readable execution narrative and findings

## Scalability Pattern

The model is intended to scale by:
- adding new role agents without redesigning the orchestrator contract
- adding plugin knowledge packs for new integration contexts
- reusing skill modules across testing projects
