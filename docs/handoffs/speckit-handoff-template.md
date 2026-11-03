# AI Handoff

> Purpose:
>
> Provide sufficient context for a new GitHub Copilot chat to continue work
> without re-reading large artifacts unnecessarily.
>
> This document is a compressed working-state summary, not a PRD,
> FRD, specification, architecture document, research document,
> meeting notes repository, or session transcript.

---

# Copilot Instructions

When creating or updating this handoff:

1. Optimize for context compression.
2. Record outcomes, not discussions.
3. Record current state, not historical timelines.
4. Summarize important decisions instead of linking to discussions.
5. Reference large artifacts rather than duplicating them.
6. Include only information likely needed in the next session.
7. Remove completed items that no longer affect future work.
8. Preserve unresolved questions and active constraints.
9. Update sections in-place rather than appending session logs.
10. Keep total length under 500 words whenever practical.
11. Assume the repository is available for inspection.
12. Do not explain code that can be easily understood by reading it.
13. Prefer concise summaries over extensive references when the summary prevents large-context retrieval.
14. Maintain a single source of truth:
    - Handoff = working state
    - PRD = business intent
    - FRD/Spec = implementation intent

---

# Information Retention Rule

Before adding information to this handoff, ask:

> Will a future Copilot chat likely need this information to make a
> decision, avoid rework, understand current state, or complete the
> next task?

If the answer is **No**, do not include it.

Prefer storing information in the following order of value:

1. Decision
2. Constraint
3. Current State
4. Risk
5. Open Question
6. Discussion History

Discussion history should almost never appear in this document.

---

# Information Tiers

## Tier 1: Always Include

Information that is:

- Critical
- Easy to forget
- Difficult to infer from code

Examples:

- Architectural decisions
- Business rules
- Constraints
- Active blockers
- Current objective

---

## Tier 2: Include Only If Relevant To Upcoming Work

Examples:

- Current implementation status
- API contracts
- Feature-specific assumptions
- Partially completed design work
- Temporary workarounds

Remove when no longer relevant.

---

## Tier 3: Reference Only

Do not copy large artifacts.

Reference instead:

- PRDs
- FRDs
- Specifications
- Architecture documents
- Research documents
- Wireframes
- Meeting notes

Summarize conclusions rather than copying source material.

---

# Project Context

## Objective

Provide a concise 1–3 sentence summary of the feature, initiative, or workstream.

---

# Current State

## Completed

- Item
- Item

## In Progress

- Item
- Item

## Not Started

- Item
- Item

---

# Key Decisions

Include only decisions that affect future implementation or design.

- Decision
- Decision

---

# Constraints

Include only constraints that future work must respect.

- Constraint
- Constraint

---

# Current Architecture

Maximum: 150 words

Summarize:

- Major components
- Data flow
- Integration points
- Ownership boundaries

Do not describe implementation details visible in code.

---

# Known Risks / Issues

- Risk
- Risk

---

# Open Questions

Include only unresolved questions affecting upcoming work.

- Question
- Question

---

# Next Action

Describe the exact task the next Copilot chat should perform.

Example:

Implement grouped search results in SearchResults.tsx.

Success Criteria:

- Group by entity type
- Preserve existing sort order
- No API contract changes

---

# Relevant Artifacts

Authoritative sources.

- PRD:
- FRD:
- Spec:
- Architecture:
- Additional References:

---

# Relevant Files

Only include files directly related to the next work item.

- path/to/file
- path/to/file

---

# Handoff Quality Checklist

Before saving this handoff, verify:

- [ ] Current objective is clear.
- [ ] Next action is specific and actionable.
- [ ] Key decisions are summarized.
- [ ] Active constraints are documented.
- [ ] Open questions remain unresolved.
- [ ] Large artifacts are referenced, not duplicated.
- [ ] Outdated information has been removed.
- [ ] Discussion history has been omitted.
- [ ] Document remains concise.
- [ ] A new Copilot chat could begin productive work immediately after reading this file.