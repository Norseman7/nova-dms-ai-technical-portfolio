# NOVA Roadmap

## Purpose

NOVA is a phased modular AI-enabled decision-support platform for high-volume futures-market data. The roadmap emphasizes traceability, validation before AI trust, modular architecture, human approval, auditability, and production-readiness thinking.

## Current baseline

NOVA has a documented architecture direction covering source acquisition, raw authority, DATABASE dataset definitions, derived indexes, ANALYSIS planning, event modules, standardized outcomes, Brain Store boundaries, and AI reasoning safeguards. The system is not presented as finished production deployment.

## Phase 1: Data foundation and session-aware acquisition

Goals:

- acquire source data through session-aware workflows
- preserve source provenance and acquisition diagnostics
- separate acquisition completion from analysis conclusions
- keep raw data immutable and reusable
- avoid UI-owned acquisition logic

Maturity signal: Paul defined acquisition as a controlled source-authority layer rather than a direct trading-signal layer.

## Phase 2: Database/indexing and derived datasets

Goals:

- make DATABASE the dataset input authority
- store dataset definitions as metadata references
- build derived session indexes with rule versions and diagnostics
- preserve session scope and source lineage
- support immutable analysis snapshots

Maturity signal: NOVA favors derived operating views over repeated raw-data scans.

## Phase 3: Event detection modules, not limited to Big Trades

Goals:

- define a module registry and module contracts
- support trigger events, reference interactions, value-based signals, market-state tags, memory zones, and session-structure observations
- use Big Trades as one objective early validation case
- require deterministic event identity and rule versions
- reuse standardized event outcome envelopes across event families

Maturity signal: the event architecture is extensible and validation-driven.

## Phase 4: Analysis workspace and visual review

Goals:

- run ANALYSIS only from DATABASE-approved snapshots
- produce event records, reference interactions, outcomes, and correlations
- support visual review without making visuals the source authority
- keep human-reviewed validation central
- distinguish facts, interpretations, and opinions

Maturity signal: the analysis workspace is an evidence workflow, not a recommendation engine.

## Phase 5: AI reasoning support with human-in-the-loop safeguards

Goals:

- use AI to query, explain, compare, and summarize structured evidence
- preserve AI reasoning as downstream of validated data
- require human review for acceptance and operational use
- avoid unsupported opinion storage as facts
- keep ChatGPT and Codex under controlled development governance

Maturity signal: AI is helpful but not trusted without traceable evidence.

## Phase 6: Validation, scoring, and accumulated learning layer

Goals:

- promote only validated facts, outcomes, correlations, and aggregates into Brain Store
- separate reliability, confidence, sample size, and observed performance
- quarantine experimental/live-learning records before trust
- support supersession and rebuildable aggregates
- track event confidence and scoring without claiming guaranteed performance

Maturity signal: learning is evidence accumulation, not unreviewed automation.

## Phase 7: Production-readiness hardening

Goals:

- strengthen diagnostics, fail-closed behavior, lifecycle states, and audit reports
- protect source data, datasets, logs, and generated outputs from accidental mutation
- formalize module contracts and compatibility checks
- improve reviewability and operational support
- validate performance and data-access patterns before scaling usage

Maturity signal: production readiness is treated as a discipline, not a label.

## Long-term direction

NOVA should evolve into a controlled decision-support environment where raw data can be preserved once and reinterpreted many times through versioned modules, standardized outcomes, accumulated evidence, and human-reviewed AI reasoning.

## Explicit non-goals

NOVA does not claim:

- autonomous trading
- guaranteed performance
- finished commercial deployment
- AI-only decision authority
- replacement of human validation
- dependency on a named third-party validation platform
