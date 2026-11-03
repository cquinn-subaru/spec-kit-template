# Copilot Chat Handoff

> **Purpose**: Provide sufficient context for a new GitHub Copilot chat to continue work without re-reading large artifacts or losing critical context.
>
> This document is a compressed working-state summary—a snapshot of the current project state, decisions, and next steps.

---

## Copilot Instructions

When creating or updating this handoff:

1. Optimize for context compression.
2. Record outcomes, not discussions.
3. Record current state, not historical timelines.
4. Summarize important decisions concisely.
5. Reference large artifacts rather than duplicating them.
6. Include only information likely needed in the next session.
7. Remove completed items that no longer affect future work.
8. Preserve unresolved questions and active constraints.
9. Update sections in-place rather than appending session logs.
10. Keep total length under 500 words whenever practical.
11. Assume the repository is available for inspection.
12. Do not explain code that can be easily understood by reading it.
13. Prefer concise summaries over extensive references when the summary prevents large-context retrieval.

---

## Information Retention Rule

Before adding information to this handoff, ask:

> Will a future Copilot chat likely need this information to make a decision, avoid rework, understand current state, or complete the next task?

If the answer is **No**, do not include it.

Prefer storing information in the following order of value:

1. **Decision** — critical choices affecting direction
2. **Constraint** — limitations that restrict future work
3. **Current State** — what is done, in progress, or blocked
4. **Risk** — potential issues or unknowns
5. **Open Question** — unresolved issues affecting next steps
6. **Discussion History** — avoid unless critical context

---

## Information Tiers

### Tier 1: Always Include

Information that is critical, easy to forget, or difficult to infer from code:

- Architectural decisions
- Technical constraints or limitations
- Active blockers or issues
- Current objective
- Known workarounds or temporary solutions

### Tier 2: Include Only If Relevant

Examples:

- Current implementation status
- API contracts or interfaces
- Feature-specific assumptions
- Partially completed design work
- Tech stack or tool decisions

Remove when no longer relevant.

### Tier 3: Reference Only

Do not copy large artifacts—reference instead:

- Architecture documents
- Design documents
- Research or investigation files
- Meeting notes
- External resources

Summarize conclusions rather than copying source material.

---

# Project Context

## Objective

Provide a concise 1–3 sentence summary of the current initiative, feature, or focus.

---

# Current State

### Completed

- Item
- Item

### In Progress

- Item
- Item

### Not Started

- Item
- Item

---

# Key Decisions

Include only decisions that affect future implementation or design direction.

- Decision 1
- Decision 2

---

# Constraints

Include only constraints that future work must respect.

- Constraint 1
- Constraint 2

---

# Current Architecture / Approach

**Maximum: 150 words**

Summarize:

- Major components or modules
- Data flow or key interactions
- Integration points
- Tech stack or framework choices
- Known limitations

Do not describe implementation details visible in code.

---

# Known Risks / Issues

- Risk 1
- Risk 2

---

# Open Questions

Include only unresolved questions affecting upcoming work.

- Question 1
- Question 2

---

# Next Action

Describe the exact task the next Copilot chat should perform.

**Example:**

Implement grouped search results in `SearchResults.tsx`.

**Success Criteria:**

- Group results by entity type
- Preserve existing sort order
- No breaking API changes

---

# Relevant Files

Only include files directly related to the next work item.

- path/to/file.ts
- path/to/component.tsx

---

# Handoff Quality Checklist

Before saving this handoff, verify:

- [ ] Current objective is clear
- [ ] Next action is specific and actionable
- [ ] Key decisions are summarized
- [ ] Active constraints are documented
- [ ] Open questions remain unresolved
- [ ] Large artifacts are referenced, not duplicated
- [ ] Outdated information has been removed
- [ ] Discussion history has been omitted
- [ ] Document is concise
- [ ] A new Copilot chat could begin productive work immediately
