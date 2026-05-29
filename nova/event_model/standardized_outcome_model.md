# Standardized Outcome Model

## Purpose

The standardized outcome model ensures that event families can be measured consistently. Event detection and outcome measurement are separated so NOVA can ask what happened after an event without turning the event definition itself into a prediction or recommendation.

## Event Outcome Envelope

Each event module should emit records compatible with a common envelope:

| Field group | Examples |
| --- | --- |
| Event identity | event id, event type, module version, rule version |
| Time and price | event timestamp, display timestamp, event price, price range |
| Dataset context | dataset id, analysis run id, analysis snapshot id, session scope |
| Session context | clock session phase, minutes since phase start, minutes to key boundaries |
| Context tags | market state, reference context, value-signal class, memory-zone context |
| Outcome windows | 1m, 5m, 15m, 30m, 60m, to regular-session close, to selected-session close |
| Validity | valid, not applicable, insufficient data, missing source data, session closed before window, calculation error |
| Diagnostics | source references, rule notes, missing-field notes, calculation warnings |

## Outcome Window Shape

Each outcome window should preserve:

- return in points/ticks where applicable
- direction derived from measured return
- maximum up movement
- maximum down movement
- maximum favorable/adverse movement only when expected direction is explicitly defined
- high/low after event
- time to maximum movement
- price basis
- validity status
- diagnostics

## Direction-Neutral First

Raw event outcomes should first store direction-neutral facts. Directional favorable/adverse interpretation requires an explicit expected direction or hypothesis. This prevents the system from encoding hidden recommendations into factual event records.

## Quality And Comparability

Outcome records are comparable only when dataset scope, event definition, rule version, price basis, and outcome validity are compatible. Missing windows must fail closed with diagnostics instead of fabricated results.
