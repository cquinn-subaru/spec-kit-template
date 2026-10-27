# Product Requirements Document: [Product Name]

**PRD ID**: PRD-001
**Owner**: [Accountable product owner]
**Status**: [Draft / In review / Approved / Superseded]
**Revision**: [Version or commit]
**Last updated**: [YYYY-MM-DD]
**Approvers**: [Names or roles]

> This document owns product intent, outcomes, feature boundaries, and shared
> policies. Detailed feature behavior, user stories, edge cases, and test
> scenarios belong in feature specifications. Technical design belongs in plans;
> implementation work belongs in tasks.
>
> Replace example IDs with stable IDs unique within the product. Never renumber
> or reuse retired IDs. Use Markdown links for document and requirement references.
>
> Hierarchy: PRD -> FRD -> Specification -> Plan -> Tasks -> Implementation.
> Each product feature is elaborated in a Functional Requirements Document (FRD),
> which may map to one or more Spec Kit feature specifications. A product feature
> is a coherent business capability; a specification defines a deliverable slice
> of that capability. Features may align to epics in a project management tool,
> but that mapping does not define the requirements hierarchy. Use the
> [FRD template](./frd-template.md) to define that bridge.
> Example links below assume this PRD is saved as docs/prd.md and FRDs live in
> docs/frds/. Replace them with actual document links.

## 1. Business Problem

[Describe the current problem, affected users, business impact, supporting
evidence, and why addressing it matters now. Avoid prescribing a solution.]

## 2. Product Vision

[Describe the desired future experience, product value proposition, and how
this product supports business strategy.]

## 3. Users / Personas

| Persona ID | Name / role | Goals | Pain points | Context / evidence |
|------------|-------------|-------|-------------|--------------------|
| PRD-001-P-001 | [Persona] | [Desired outcome] | [Current difficulty] | [Research link / context] |

## 4. Product Goals

> Goals describe desired business or user outcomes, not a feature backlog.

| Goal ID | Outcome | Personas | Priority | Success metric IDs |
|---------|---------|----------|----------|--------------------|
| PRD-001-G-001 | [Outcome] | [Persona IDs] | [Priority] | PRD-001-M-001 |

## 5. Success Metrics

> Distinguish product outcome measurement from feature acceptance testing.
> Mark unknown baselines or targets as TBD with an owner and resolution date.

| Metric ID | Goal IDs | Measure / definition | Baseline | Target | Measurement window | Data source / method | Owner |
|-----------|----------|----------------------|----------|--------|--------------------|----------------------|-------|
| PRD-001-M-001 | PRD-001-G-001 | [Metric and population] | [Value / date] | [Value] | [Period after launch] | [Source / calculation] | [Owner] |

## 6. Non-Goals

> Identify product-level exclusions and their rationale. Feature-specific exclusions
> belong in the relevant FRD.

| Non-goal ID | Excluded outcome / capability | Rationale |
|-------------|-------------------------------|-----------|
| PRD-001-NG-001 | [Exclusion] | [Reason] |

## 7. Feature Catalog

> A product feature is a coherent business capability or outcome, not automatically
> a single feature specification. Each approved feature is elaborated in an FRD and
> may be delivered through one or more independently testable feature specs.
> Do not put feature acceptance scenarios or detailed requirements in this table.

| Feature ID | Feature / capability | Intended outcome and boundary | Goal IDs | Priority / sequencing | FRD | Status / owner |
|---------|-------------------|-------------------------------|----------|-----------------------|-----|----------------|
| FEAT-001 | [Feature name] | [Outcome; boundary with adjacent features] | PRD-001-G-001 | [Priority / dependencies] | [FRD-001](./frds/FRD-001.md) | [Proposed / owner] |

## 8. Shared Business Rules

> Include only policies that apply across the product or multiple features.
> Feature-wide rules belong in the FRD; specification-local validations and
> behavior belong in the spec. Define the rule here once and reference its ID.

| Rule ID | Policy / rule | Applicability | Business authority / rationale |
|---------|---------------|---------------|--------------------------------|
| PRD-001-BR-001 | [Unambiguous policy] | [All features or named scope] | [Authority / reason] |

## 9. Shared Constraints

> Record genuine, externally imposed boundaries rather than proposed design
> choices. Make measurable constraints explicit where possible. Explain the
> authority for any mandated technology; otherwise leave technical choices to plans.

| Constraint ID | Category | Constraint / measurable limit | Applicability | Source / authority |
|---------------|----------|-------------------------------|---------------|--------------------|
| PRD-001-C-001 | [Business / technical / security / compliance / accessibility / operational] | [Boundary] | [Scope] | [Source] |

## 10. Product-Level Open Questions, Assumptions, and Decisions

> Keep only questions or assumptions affecting product direction, shared policy,
> or feature boundaries. Move detailed feature behavior to the relevant spec.

| ID | Type | Question / assumption / decision | Owner | Resolve by | Status / resolution / affected IDs |
|----|------|---------------------------------|-------|------------|------------------------------------|
| PRD-001-Q-001 | [Question / assumption / decision] | [Description] | [Owner] | [Date] | [Status / links] |

## 11. Traceability and Change Control

- The feature catalog is the product-to-feature index. Each FRD links back to this
  PRD, identifies the reviewed PRD revision, and maps its scope to goal IDs.
- Shared rules and constraints are authoritative here. FRDs and specs reference
  applicable IDs; they do not maintain independently editable copies.
- On a product change, review affected FRDs and their linked specs for impact.
  Record the decision, affected IDs, owner, and required follow-up before
  treating downstream documents as aligned.
- An approved PRD means product direction is agreed, not that every feature is
  specified or implemented. Record unallocated or deferred goals explicitly;
  do not imply coverage solely because a feature is listed.

| Change / decision | Affected IDs | Downstream impact / links | Owner | Review status |
|-------------------|--------------|---------------------------|-------|---------------|
| [Revision / decision reference] | [IDs] | [FRDs to review / action] | [Owner] | [Pending / reviewed] |
