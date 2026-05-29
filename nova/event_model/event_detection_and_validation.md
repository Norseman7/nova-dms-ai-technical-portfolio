# Event Detection And Validation

## Event Definition

In NOVA, an event is a deterministic, timestamped occurrence derived from market evidence. It is independent of outcome. The outcome is measured later through a standardized envelope.

An event must preserve:

- event identity
- event type
- event timestamp
- event price or price range
- session scope
- context tags
- module version
- rule version
- source lineage
- diagnostics

## Event Families

NOVA is designed for more than one detector:

| Family | Examples |
| --- | --- |
| Trigger events | Big Trades, absorption, imbalance, stop-runs, breakouts, rejections |
| Reference interactions | touch, break, hold, reject, accept, rotation around reference levels |
| Value-based signals | cumulative flow, delta, pace, volume, volatility, spread, normalized signal windows |
| Market state | trend, balanced, rotational, high-volatility, value acceptance/rejection |
| Order-flow memory | prior aggressive activity zones and later retests |
| Session structure | opening location, expansion, direction, range contribution, continuation/reversal observations |
| Conditional outcomes | what happens after a condition or event under a defined dataset and outcome window |

## Big Trades As Early Proof Case

Big Trades is useful as a first bounded validation case because it tests:

- event identity from source evidence
- threshold classification
- duplicate prevention across threshold classes
- timestamp handling
- side/context preservation without directional assumptions
- source lineage
- standardized outcome compatibility
- human-reviewed validation against timestamped evidence

It is not the final event model and does not represent NOVA's full AI capability.

## Validation Requirements

| Requirement | Purpose |
| --- | --- |
| Deterministic rules | Same input and same rule version should produce the same event output. |
| Versioned definitions | Changed event logic creates a new version and avoids silent result drift. |
| Timestamp cutoff safety | Context features must only use data available at or before the event. |
| Immutable analysis snapshots | Event results remain interpretable even if datasets change later. |
| Outcome validity status | Missing or invalid outcome windows fail closed with diagnostics. |
| Sample-size gates | Interesting correlations are not automatically trusted correlations. |
| Human review | Event definitions and validation evidence remain human-approved. |

## AI Boundary

AI may explain event evidence and help compare patterns, but event detection and outcome measurement must remain deterministic, source-traceable, and reviewable.
