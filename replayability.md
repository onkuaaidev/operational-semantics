# Replayability

Short notes on replayability as a property:

- Replayable systems can take a prior input snapshot and re-produce the exact same treatment and outcome.
- Key building blocks:
  - Canonical input representation
  - Deterministic hashing / IDs for inputs and policy versions
  - Immutable mapping store (policy_version -> decision_mapping)
  - Runtime that resolves input via mapping with strict fallbacks (insufficient evidence)

Possible small experiments are in ../minimal-experiments.
