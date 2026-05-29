# Event Detection Pseudocode

This example is sanitized pseudocode. It is not copied source code.

## Goal

Show how an event module should preserve deterministic identity, source lineage, rule versions, and standardized outcome compatibility.

```text
function run_event_module(analysis_snapshot, module_config):
    require analysis_snapshot.is_immutable
    require module_config.module_version
    require module_config.rule_version

    source_rows = load_approved_inputs(analysis_snapshot, module_config.required_inputs)
    if source_rows.missing_or_ambiguous:
        return fail_closed("missing required source evidence")

    events = []

    for window in iterate_time_ordered_windows(source_rows):
        context = build_timestamp_cutoff_context(window.end_time)

        if trigger_condition_met(window, context, module_config):
            event = {
                "event_id": deterministic_event_id(window, module_config),
                "event_type": module_config.event_type,
                "event_time": window.event_time,
                "event_price": window.event_price,
                "session_scope": analysis_snapshot.session_scope,
                "analysis_snapshot_id": analysis_snapshot.id,
                "module_version": module_config.module_version,
                "rule_version": module_config.rule_version,
                "source_lineage": window.source_refs,
                "diagnostics": window.diagnostics,
                "outcome_envelope_ready": true
            }
            events.append(event)

    return events
```

## Validation Notes

- Detection uses only evidence available at or before the event timestamp.
- Outcome measurement runs later and does not influence detection.
- Event identity is not based on UI position or visual label placement.
- Missing input fails closed with diagnostics.
