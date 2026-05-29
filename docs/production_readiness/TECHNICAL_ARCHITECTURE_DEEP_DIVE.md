# Technical Architecture Deep Dive

## System View

The portfolio combines three layers:

| Layer | Purpose |
| --- | --- |
| NOVA | Modular AI-enabled market decision-support architecture. |
| DMS | Governance and development-control layer for long-running AI-assisted work. |
| Figma workflow | Supporting UI/design quality-control layer for controlled implementation alignment. |

## NOVA Architecture

NOVA is organized as a layered evidence system:

```text
Acquisition
-> raw data authority
-> DATABASE dataset definitions and derived indexes
-> ANALYSIS structured measurement
-> standardized outcome records
-> Brain Store evidence accumulation
-> AI reasoning / explanation
-> human-reviewed decision support
```

Core design decisions:

- raw market records remain source authority and are not overwritten by derived outputs
- DATABASE is the input authority for analysis-ready datasets
- derived indexes and compact read models form the normal operating layer
- ANALYSIS consumes immutable dataset snapshots and approved derived inputs
- event modules emit standardized outcome envelopes
- Brain Store accumulates facts, observations, measured outcomes, correlations, and rebuildable aggregates
- AI operates over structured evidence and does not become the primary calculator

## Event Architecture

NOVA's event architecture supports multiple event and context families:

- trigger event modules such as Big Trades, absorption, imbalance, stop-runs, breakouts, and rejections
- reference and indicator modules such as value areas, profile levels, and session levels
- reference interaction events such as touch, break, hold, reject, accept, and rotation
- value-based signal modules such as cumulative flow, delta, pace, spread, volatility, and volume measures
- market state classifier tags such as trend, rotational, balanced, high-volatility, and value-acceptance states
- order-flow memory zones and retests
- session-structure observations
- conditional outcomes and correlation aggregates

Big Trades is positioned only as an early bounded validation case because it is objective, timestamped, measurable, and easy to review against human-observed evidence. The standard outcome model is reusable across future event families.

## Traceability Model

Each analysis path is expected to preserve:

- dataset definition identity
- immutable analysis snapshot identity
- included and excluded session references
- session scope
- event/module version
- rule version
- timestamp authority
- source lineage
- diagnostics
- outcome validity status

This makes later interpretation auditable even when dataset definitions, module thresholds, or derived indexes evolve.

## DMS Governance Layer

DMS supports:

- project-scoped document access
- handover continuity
- audit template discipline
- report generation
- task and time tracking
- agent/governance prompt control
- evidence-based review gates

DMS is important because NOVA is a long-running, high-complexity project. The governance layer reduces context loss, architecture drift, and uncontrolled AI-assisted development.

## Figma Workflow Layer

The Figma workflow is a supporting toolchain for UI/design discipline. It helps:

- export selected design scope for review
- validate naming and settings changes
- preview change sets before mutation
- keep edits within selected scope
- treat AI-generated UI changes as proposals until validated
- support Figma-to-Codex implementation alignment

It is not presented as equal to NOVA. It is a workflow-control layer that improves UI quality, naming consistency, and implementation discipline.
