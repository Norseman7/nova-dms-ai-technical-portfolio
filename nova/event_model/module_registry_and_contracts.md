# Module Registry And Contracts

## Purpose

NOVA's future event and analysis modules need explicit contracts so new modules can be added without duplicating DATABASE logic, bypassing source authority, or coupling directly into UI state.

## Module Registry Thinking

A module registry should answer:

- what module exists?
- what event or observation family does it produce?
- what inputs are required?
- what dataset scopes are supported?
- what derived indexes or raw evidence are needed?
- what rule version is used?
- what output record type is produced?
- what diagnostics and failure states are expected?
- whether the module is experimental, validated, accepted, superseded, or archived

## Module Contract Fields

| Contract area | Expected content |
| --- | --- |
| Identity | module name, module version, rule version, schema version |
| Inputs | required snapshot fields, derived indexes, source references, session scope |
| Safety | timestamp cutoff behavior, no-look-ahead constraints, fail-closed rules |
| Output | event record, observation record, signal snapshot, reference interaction, outcome compatibility |
| Diagnostics | missing inputs, unsupported scope, insufficient data, calculation warnings |
| Lifecycle | draft, experimental, validated, accepted, superseded, archived |
| Review | human validation requirements and promotion eligibility |

## Isolation Rules

Modules should not:

- mutate raw source data
- redefine DATABASE dataset authority
- scan raw data on page load
- write Brain Store facts directly without promotion rules
- mix incompatible dataset scopes silently
- store recommendations as facts
- depend on UI layout or row position for event identity

## Why It Matters

Module contracts let NOVA grow from an early bounded validation case into a broader event architecture without losing traceability, comparability, or review discipline.
