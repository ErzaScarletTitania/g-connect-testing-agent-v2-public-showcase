# g-connect-testing-agent-v2-public-showcase

Public showcase for the Version 2 architecture of an AI-driven testing framework designed for G-Connect workflows.

## What This Project Demonstrates

This repository presents a production-oriented design for orchestrating autonomous and semi-autonomous testing sessions through a structured multi-agent system.

Core capabilities demonstrated:
- Orchestrator-led decomposition of testing into bounded phases
- Role-specialized AI agents for intake, planning, execution, evidence, triage, feedback, and reporting
- Reusable skills and plugin-specific knowledge packs
- Machine-readable session state and output contracts
- Evidence-first reporting pipeline for reproducibility and auditability
- Approval-gated delivery handoff with stakeholder notification drafting

## Why This Matters

Most AI demos stop at prompt engineering. This project focuses on operational AI architecture:
- repeatable execution
- controlled decision boundaries
- persistent state and traceability
- practical integration with software quality workflows

The goal is to move from ad-hoc test execution to a scalable AI-assisted delivery model.

## Technical Scope

See:
- [Architecture](docs/architecture.md)
- [Operating Model](docs/operating-model.md)
- [Security and Public/Private Boundary](docs/security-and-sharing.md)

## Sample Outputs

A sanitized sample execution package is included in [artifacts/sample-session](artifacts/sample-session):
- session summary JSON
- evidence index JSON
- report markdown
- delivery handoff JSON
- report-ready email draft

These files illustrate how execution state, evidence, and outcomes can be persisted in machine-readable and human-readable forms.

## Public Mirror Strategy

This repo is intentionally sanitized and publication-safe.
The private full repository retains implementation details, internal prompts, connectors, and operational assets.

Sharing model:
- Public mirror: architecture, models, examples, and non-sensitive artifacts
- Private full repo: deep implementation and internal operations
- Candidate/employer deep review: read-only invitation to private repo when needed

Public examples intentionally replace customer-specific locations with generic placeholders such as `<customer-shared-location>`.

## Skills Highlighted

- Applied AI systems design
- Multi-agent orchestration architecture
- Automation and workflow engineering
- Information modeling and schema-driven outputs
- Evidence-based QA process design
- Technical leadership for AI-enabled delivery
