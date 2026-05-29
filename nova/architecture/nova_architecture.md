# NOVA Architecture

## Layered Model

NOVA uses a preservation-first architecture:

```text
Source acquisition
  -> raw market memory
  -> processing / normalization
  -> derived indexes and read models
  -> DATABASE dataset authority
  -> ANALYSIS structured evaluation
  -> event outcomes and correlations
  -> Brain Store evidence accumulation
  -> AI explanation and human review
```

## Authority Boundaries

| Layer | Owns | Must not own |
| --- | --- | --- |
| Acquisition | source data acquisition, completion metadata, provenance, diagnostics | event interpretation, Brain logic, recommendations |
| Raw authority | immutable source records and replayable market memory | derived conclusions as source truth |
| Derived indexes | session characterization, compact operating views, rule versions | raw source mutation |
| DATABASE | dataset definitions, included/excluded session references, session scope, readiness | ANALYSIS execution or event scoring |
| ANALYSIS | analysis runs, immutable snapshots, module execution, standardized outputs | raw acquisition ownership or DATABASE mutation |
| Brain Store | promoted facts, observations, measured outcomes, correlations, rebuildable aggregates | unsupported opinions or direct raw-data ownership |
| AI layer | reasoning, query, explanation, development support | primary calculation authority or autonomous decision authority |
| UI layer | display, selection, and interaction | business logic, raw parsing, source-of-truth lineage |

## Operating Layer Principle

NOVA should not load or present more data than required for the current decision. Raw data is preserved for audit and recalculation, while derived indexes, summaries, manifests, and read models are the normal operating layer.

## Analysis Snapshot Gate

ANALYSIS cannot proceed safely without an immutable dataset snapshot. The snapshot preserves:

- source dataset identity
- dataset version or revision marker
- instrument/session scope
- included and excluded session references
- derived index schema/rule versions
- creation timestamp
- diagnostics

This protects old analysis runs from silently changing meaning when a dataset definition changes later.

## AI Boundary

AI is deliberately downstream. It may help query, explain, compare, and reason over structured evidence. It should not recalculate raw facts on demand, store unsupported opinions as facts, or bypass validation gates.
