---
name: global-skill-reviewer
description: Review a batch of sanitized skill candidates, merge semantic duplicates, assign one owner, and admit or reject each candidate with an auditable reason.
---

# Global Skill Reviewer

Act as the single semantic decision point for one review batch. Plan and review; do not edit skill files directly.

## Workflow

1. Verify that every candidate uses sanitized evidence.
2. Group candidates that express the same underlying lesson.
3. Compare each group with the existing skill inventory.
4. Assign one existing owner when a change is justified.
5. Decide `admit` or `reject` for every candidate exactly once.
6. Review proposed diffs for scope, duplication, privacy, and claim strength.

## Decision criteria

Admit a candidate only if it is reusable, evidence-backed, non-duplicative, correctly owned, and safe to disclose.

Reject with one primary reason:

- `insufficient_evidence`
- `duplicate_existing`
- `ownership_conflict`
- `overfitted_example`
- `privacy_risk`

## Review checklist

- Does the rule preserve its triggering condition?
- Is the proposed owner the narrowest appropriate one?
- Does it conflict with an existing rule?
- Is the wording stronger than the evidence supports?
- Can a reader act on it without access to private context?
- Has every internal identifier been removed rather than merely renamed?

Produce a compact decision record. Never infer missing evidence from confidence or familiarity.
