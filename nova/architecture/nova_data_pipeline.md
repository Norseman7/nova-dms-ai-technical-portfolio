# NOVA Data Pipeline

## Pipeline Model

```text
Session-aware acquisition
-> immutable raw source authority
-> processing / normalization
-> derived session indexes
-> DATABASE dataset definitions
-> immutable ANALYSIS snapshots
-> event modules and reference modules
-> standardized outcome records
-> correlations and quality gates
-> Brain Store evidence accumulation
```

## Pipeline Responsibilities

| Stage | Responsibility |
| --- | --- |
| Acquisition | Create or resolve source data with provenance and diagnostics. |
| Raw authority | Preserve replayable market memory without mutation by downstream layers. |
| Processing | Normalize records into internal structures for bounded backend workflows. |
| Derived indexes | Produce compact session facts and readiness states with source lineage. |
| DATABASE | Define analysis input datasets and session membership. |
| ANALYSIS | Run structured evaluation from immutable snapshots. |
| Event modules | Detect timestamped events or context observations through versioned rules. |
| Outcome engine | Measure consistent outcome windows and validity status. |
| Brain Store | Accumulate validated evidence and rebuildable aggregates. |

## Safety Rules

- Page load should not trigger broad raw-data scans.
- Derived outputs should not become sole source truth.
- Dataset definitions should reference source sessions, not copy raw records.
- Analysis should fail closed when input authority is missing or ambiguous.
- AI reasoning should operate after evidence is structured and validated.
