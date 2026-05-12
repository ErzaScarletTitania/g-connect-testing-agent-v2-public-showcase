# Operating Model

## Session Lifecycle

Each testing session follows a controlled lifecycle:
- Session initialization
- Scope and constraints validation
- Phase-by-phase execution
- Evidence and issue synthesis
- Report generation
- Delivery packaging and approval
- Stakeholder notification drafting
- Session closure and persistence

## Control Principles

- Bounded Autonomy: agents act within explicit phase constraints.
- Explicit Handoffs: each phase emits artifacts consumed by the next phase.
- Contract-Driven State: outputs follow machine-readable schema contracts.
- Human Override: operator can intervene at decision checkpoints.
- Approval Gates: customer-ready outputs are not released until a human approves the final package.

## Key Artifacts

- session.summary.json: high-level status, confidence, and outcomes
- evidence-index.json: normalized index of generated evidence
- report.md: human-readable execution narrative and findings
- delivery-handoff.json: machine-readable release state for the customer-ready package
- report-ready-email.md: sanitized stakeholder notification draft

## Delivery Handoff Pattern

The reporting stage can extend into a controlled delivery handoff:

1. Generate the customer-ready report package.
2. Normalize any external references to a customer-safe shared location placeholder.
3. Require explicit human approval before release.
4. Draft the stakeholder email that states the report is ready and where it is located.

## Scalability Pattern

The model is intended to scale by:
- adding new role agents without redesigning the orchestrator contract
- adding plugin knowledge packs for new integration contexts
- reusing skill modules across testing projects
