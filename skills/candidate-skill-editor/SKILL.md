---
name: candidate-skill-editor
description: Turn a sanitized, evidence-backed observation into one minimal and reviewable skill-edit proposal. Use when a candidate rule must be checked for scope, duplication, privacy, and validation before admission.
---

# Candidate Skill Editor

Convert one candidate at a time. Do not re-read raw private sessions when a sanitized evidence summary is available.

## Workflow

1. Inspect the candidate, its evidence summary, and the allowed target files.
2. Search the target for equivalent or conflicting guidance.
3. Classify the candidate as `patch` or `no_change`.
4. For `patch`, write the smallest conditional rule that preserves the evidence boundary.
5. Re-read the final text and report the exact changed section plus validation performed.

## Admission rules

Admit only when the candidate:

- is supported by reproducible or independently corroborated evidence;
- belongs to the selected skill;
- adds actionable guidance not already present;
- contains no private identifiers, secrets, proprietary terms, or copied operational data;
- can be expressed without a one-off business example.

Prefer the form: **condition → failure mode → diagnostic or corrective action**.

## Reject when

- evidence is insufficient;
- the rule duplicates existing guidance;
- another asset is the correct owner;
- the observation is too scenario-specific to generalize safely;
- sanitization would remove the meaning needed to support the claim.

## Editing constraints

- Stay inside the approved files.
- Do not invent APIs, measurements, or success claims.
- Do not turn a single incident into an unconditional rule.
- Do not add implementation code unless the publication scope explicitly permits it.
- Keep a concise receipt: decision, reason, target, and validation result.
