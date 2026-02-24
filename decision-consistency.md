# Decision Consistency

Definition
----------
Decision consistency: given identical inputs and the same policy version, the system must produce the same operational outcome.

Why it matters
--------------
- Reduces coordination overhead
- Enables removal of repetitive arbitration
- Makes automation trustable (not merely advisory)

Minimal desiderata
------------------
1. Deterministic mapping from canonicalized input → outcome
2. Policy versioning tied to the mapping (explicit binding)
3. Replayability: ability to re-run previous inputs against a recorded mapping and get identical results
4. Audit trail: who changed binding and why

Short note on human role
------------------------
Humans should be the reviewer and change-author for mappings, not the runtime deciders.
