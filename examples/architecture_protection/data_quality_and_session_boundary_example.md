# Data Quality And Session Boundary Example

## Scenario

A dataset contains sessions with mixed completeness and different session scopes.

## Safe Handling

```text
for each session_reference in dataset_definition:
    verify source lineage
    verify session scope
    verify required derived index exists
    verify completeness and readiness status

    if required evidence is missing:
        mark session as not analysis-ready
        record diagnostic
        exclude from trusted analysis until reviewed
```

## Required Outputs

- session identity
- session scope
- readiness status
- derived index version
- source-lineage reference
- diagnostic reason for exclusion or review
- human review status where needed

## Validation Point

Session boundaries and completeness are not cosmetic labels. They affect whether analysis is valid and whether AI explanations can be trusted.
