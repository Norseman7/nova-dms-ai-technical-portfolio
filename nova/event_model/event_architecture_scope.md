# Event Architecture Scope

NOVA's event architecture is not limited to Big Trades. Big Trades is treated as one early bounded validation case because it is objective, measurable, timestamped, and suitable for human-reviewed validation. The broader architecture is designed for multiple event and context families, including reference interactions, value-based order-flow signals, absorption, imbalance, stop-runs, volume-profile interactions, market-state tags, order-flow memory zones, session-structure observations, and conditional outcome analysis.

## Why Big Trades Is Useful Early

Big Trades provides a practical proof case for:

- event identity
- timestamp handling
- threshold logic
- source lineage
- duplicate prevention across threshold classes
- standardized outcome compatibility
- human-reviewed validation

It remains one event family. It is not the final event model, not a complete AI capability, and not the purpose of NOVA by itself.

## Broader Event And Context Families

| Family | Purpose |
| --- | --- |
| Reference / indicator modules | Store factual levels and context such as value areas, reference bands, profile levels, and session levels. |
| Value-based signal modules | Measure order-flow or market behavior over windows, including cumulative flow, delta, volume, pace, spread, and volatility. |
| Trigger event modules | Emit timestamped events from explicit trigger logic. |
| Reference interaction events | Record touch, break, hold, reject, accept, and rotation behavior around references. |
| Market state classifier | Add time-bounded, rule-versioned context tags without becoming a trigger event. |
| Order-flow memory zones | Preserve prior order-flow behavior zones and measure later retests. |
| Session-structure observations | Record session relationships, expansion, direction, and continuation/reversal classes. |
| Conditional outcome analysis | Measure what happens after events or conditions under defined datasets and rules. |

## Reusable Outcome Engine

The standardized event outcome envelope is reusable across event families. It lets NOVA compare event behavior across consistent windows, validity statuses, price bases, and diagnostics.

## Validation Direction

Validation should be human-reviewed, timestamped, evidence-based, and source-traceable. Event modules feed future Brain Store only after passing validation, quality gates, and explicit promotion rules.
