# Analysis And Brain Architecture

## Core Flow

```text
DATABASE
-> ANALYSIS
-> Brain Store
-> AI reasoning / explanation
-> human review
```

## DATABASE

DATABASE owns the selected evidence population:

- dataset definition identity
- lifecycle state
- instrument or market identifier
- session scope
- included/excluded session references
- derived index readiness
- source lineage
- read models and diagnostics

DATABASE is not the interpretation layer. It provides controlled input authority for ANALYSIS.

## ANALYSIS

ANALYSIS measures behavior inside an approved dataset snapshot. It produces:

- analysis run records
- baseline dataset statistics
- reference/indicator observations
- value-based signal snapshots
- trigger event records
- reference interaction events
- standardized outcome records
- context tags and market-state tags
- order-flow memory zones and retests
- conditional outcomes
- correlation aggregates

ANALYSIS must fail closed when dataset identity, scope, lineage, or required derived inputs are missing or ambiguous.

## Brain Store

Brain Store is the future accumulation layer for:

- facts
- observations
- standardized outcomes
- context tags
- market-state tags
- value-based signal observations
- memory zones and retests
- correlations
- rebuildable aggregate pattern summaries

Brain Store must not store unsupported recommendations, hidden model conclusions, or unversioned opinions as facts.

## Fact / Interpretation / Opinion Separation

| Category | Meaning | Example |
| --- | --- | --- |
| Fact | Directly measured or deterministically derived value. | event time, event price, range, measured return |
| Interpretation | Rule-based explanation/classification of facts. | reference rejection, value acceptance, trend context |
| Opinion | Generated decision-support output. | setup preference or operational hypothesis |

Opinions must remain generated outputs with evidence references and review status, not trusted Brain Store facts.

## AI Role

AI can help query, compare, explain, and summarize structured evidence. It should not be required to recalculate raw facts or bypass the validation workflow.
