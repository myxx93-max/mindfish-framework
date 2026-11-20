# Core Model

## Purpose

Mindfish is an abstract observation and routing aid for hotspot work. It helps decide which direction deserves the next unit of attention:

- **OBSERVE** — collect more time-bounded observations.
- **SUPPLEMENT** — find missing context, actors, history, or source material.
- **VERIFY** — test a claim, contradiction, or apparent pattern against independent evidence.
- **ACT** — take a bounded next step when evidence and authorization permit.

The model concerns changing states around a topic or event. It is not a model of a person's enduring identity.

## The unit: a Mindfish hypothesis

A Mindfish is a compact, falsifiable hypothesis with:
- a defined topic or event;
- a bounded observation window;
- an explicit cognitive tension or unresolved question;
- observable traces and their sources;
- confidence and uncertainty;
- counterevidence sought or found;
- an expiry or review condition;
- a recommended next observation direction.

A fish should be small enough to be disproved, split, or discarded.

## Separate the layers

| Layer | Question | Do not confuse it with |
|---|---|---|
| Reality | What happened? | What people say happened |
| Attention | Where is attention moving? | Why it moved |
| Expression | What is being said or shown? | What every participant believes |
| Cognitive-state hypothesis | What tension, gap, stake, or intention may be present? | A verified psychological fact |
| Evidence | What supports or contradicts the hypothesis? | Popularity or repetition |
| Navigation | What should be checked next? | Permission to publish or act |

## Proposed minimal record

```yaml
fish_id: string
topic_id: string
window:
  start: timestamp
  end: timestamp
hypothesis: string
route_candidates: [GAP, FOLLOW, VERIFY, STAKE, ACTION, EXPRESS]
observations:
  - source_ref: string
    observed_at: timestamp
    trace_type: string
counterevidence: []
confidence: UNKNOWN
next_direction: OBSERVE
expires_at: timestamp
status: HYPOTHESIS
```

This is a proposed research schema, not a finalized standard. Do not store personal identifiers or infer sensitive traits. `UNKNOWN` is a valid result.

## Non-claims

Mindfish does not currently establish a universal theory of cognition, causal explanations for attention movement, accurate inference of private mental states, reliable prediction of future behavior, business lift, or production readiness.
