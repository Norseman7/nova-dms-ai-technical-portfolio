# High-Volume Data Challenge

## Problem

High-volume futures-market data creates architectural risks that do not appear in small prototypes:

- repeated raw scans can make UI workflows slow and unreliable
- session scope must be explicit
- raw data, derived data, and analysis outputs can be confused if authority boundaries are weak
- look-ahead leakage can invalidate analysis
- derived values can become untraceable if rule versions and source references are missing
- AI can produce plausible explanations over invalid or incomplete evidence if the data layer is not controlled

## NOVA Response

NOVA separates source authority from operating views:

```text
raw source records
-> immutable raw-session authority
-> backend-derived indexes
-> DATABASE read models
-> immutable ANALYSIS snapshots
-> event outcomes and correlations
```

## Derived Operating Layer

The normal review path should use:

- derived session indexes
- compact metadata
- manifests
- source-lineage references
- dataset definitions
- readiness diagnostics
- bounded analysis outputs

Raw records remain available for audit, recalculation, and explicit backend workflows, but they are not the default UI/page-load path.

## Session Awareness

Session scope is part of identity, not an optional label. NOVA distinguishes full-session and regular-session concepts so analysis does not silently mix incompatible scopes.

Each derived session index should preserve:

- trading day identity
- instrument or market identifier
- session scope
- open/high/low/close style derived facts where valid
- range and net movement
- usable source-record count
- activity/readiness status
- rule version
- source lineage
- diagnostics

## Why This Matters For AI

AI-assisted reasoning is only useful when the evidence layer is trustworthy. NOVA's data architecture supports AI by making the facts structured, traceable, and bounded before explanation or interpretation occurs.
