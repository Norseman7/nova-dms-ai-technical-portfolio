# Validation Traceability Example

## Example Record Shape

```text
analysis_run_id: run_2026_05_28_example
analysis_snapshot_id: snapshot_dataset_alpha_v3
source_dataset_definition_id: dataset_alpha
session_scope: regular_session
module_name: example_trigger_module
module_version: v1
rule_version: rules_v1
event_id: deterministic_event_0001
event_time_utc: timestamp from source evidence
event_price: measured source price
source_lineage: source session references and row references
outcome_5m_status: valid
outcome_15m_status: insufficient_data
diagnostics: 15m window unavailable because session boundary was reached
human_review_status: pending_review
```

## What This Demonstrates

- dataset identity is preserved
- analysis snapshot is immutable
- source evidence is referenced
- event logic is versioned
- outcome validity is explicit
- missing data does not produce fabricated conclusions
- human review is tracked separately from measurement
