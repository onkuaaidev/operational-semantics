# Behavior vs State

Summary
-------
Systems today reliably store *state* (facts, events, timestamps).
Organizations rely on *behavior* (how facts were treated) — the mapping from state → outcome that
is persistently repeatable under the same conditions.

Observation
-----------
- A database records "refund approved" (state).
- People remember *why* that refund was approved (treatment).
- The record does not encode the treatment as an executable property.

Consequences
------------
- Two identical inputs may lead to different outcomes if the policy interpretation is not encoded.
- Organizations rely on humans to preserve consistent treatment across time.

Open questions
--------------
- How to represent treatment so that "same input → same outcome" is guaranteed unless a controlled policy change occurs?
- How to audit the mapping (input → treatment) so it is reviewable and versionable?
