# Functional Requirements Document: [Feature / Capability Name]

**FRD ID**: FRD-001
**Feature ID**: FEAT-001
**Owner**: [Accountable feature owner]
**Status**: [Draft / In review / Ready for specification / In delivery / Accepted / Superseded]
**Revision**: [Version or commit]
**Last updated**: [YYYY-MM-DD]
**Parent PRD**: [PRD-001](../prd.md)
**Parent PRD revision reviewed**: [Version or commit]
**Product goal IDs**: [PRD-001-G-001]
**Approvers**: [Names or roles]

> This document bridges product intent and feature specifications. It owns
> feature scope, business capabilities, cross-specification outcomes, and decomposition.
> It does not duplicate specification-level behavior or acceptance scenarios,
> technical plans, or implementation tasks.
>
> Hierarchy: PRD -> FRD -> Specification -> Plan -> Tasks -> Implementation.
> Each FRD elaborates one product feature from the PRD and may produce one or more
> Spec Kit feature specifications. The FRD describes the feature's required
> functional capabilities; specs refine them into detailed, independently testable
> delivery slices. A feature may align to an epic in a project management tool,
> but that optional mapping does not change document ownership or traceability.
> Start with the [PRD template](../prd-template.md) for product-level context.
>
> Path examples assume this FRD lives at docs/frds/FRD-001.md and the PRD at
> docs/prd.md in the same project as specs/. Adjust links to the actual layout.
> Keep IDs stable; never renumber or reuse retired IDs.

## 1. Feature Purpose and Business Outcome

[Describe the problem this feature addresses, why it is a coherent unit of value,
and how it contributes to the linked product goals.]

## 2. Personas and Business Journey

- **Personas**: [Links to PRD persona IDs; add feature-specific context only.]
- **Business journey**: [High-level start, outcome, and business handoffs.
  Detailed user stories and interaction flows belong in feature specs.]

## 3. Scope and Boundaries

### In Scope

- [Business capability / outcome included in this feature.]

### Out of Scope

- [Excluded capability and rationale; link to another feature if applicable.]

### Boundary with Adjacent Features

| Related feature | Ownership boundary / handoff | Dependency / coordination owner |
|--------------|------------------------------|---------------------------------|
| [Feature link / ID] | [What each feature owns] | [Dependency / owner] |

## 4. Functional Requirements

> Describe outcome-oriented business capabilities at the product-feature level.
> Each requirement should have verifiable completion evidence and a PRD goal
> reference. Detailed system MUST statements, UI behavior, field validations,
> and specification-local edge cases belong in specs.

| Requirement ID | Business capability / outcome | PRD goal IDs | Priority | Feature acceptance IDs |
|----------------|-------------------------------|--------------|----------|---------------------|
| FRD-001-R-001 | [Required capability / outcome] | PRD-001-G-001 | [Priority] | FRD-001-AC-001 |

## 5. Rules and Constraints

### Inherited Product Policies

> Reference applicable PRD policies without copying their normative text.
> All product-wide policies apply; identify relevant scoped policies and explain
> any non-applicability. Omitting a policy here does not waive it.

| PRD rule / constraint link and ID | Applicability to this feature | Allocation / evidence expected |
|----------------------------------|----------------------------|--------------------------------|
| [PRD-001-BR-001](../prd.md#8-shared-business-rules) | [Scope] | [Spec coverage / feature verification] |
| [PRD-001-C-001](../prd.md#9-shared-constraints) | [Scope] | [Spec coverage / feature verification] |

### Feature-Specific Rules and Constraints

| ID | Type | Rule / constraint | Scope | Source / authority |
|----|------|-------------------|-------|--------------------|
| FRD-001-BR-001 | Business rule | [Feature-wide policy] | [Scope] | [Authority] |
| FRD-001-C-001 | Constraint | [Measurable boundary] | [Scope] | [Authority] |

> Escalate conflicts or exception requests to the authority owning the policy.
> Do not silently override a PRD rule in this FRD or a spec. Link any approved
> exception, its scope, owner, and expiry.

## 6. Feature Dependencies, Risks, and Cross-Specification Exceptions

> Include issues affecting feature viability, dependencies on adjacent features,
> and exceptions spanning specification boundaries. Specification-local failure
> and edge cases remain in the relevant spec.

| ID | Type | Dependency / risk / exception | Impact / affected requirements | Mitigation / required outcome | Owner / status |
|----|------|------------------------------|--------------------------------|-------------------------------|----------------|
| FRD-001-D-001 | [Dependency / risk / cross-specification exception] | [Description] | [IDs / impact] | [Response] | [Owner / status] |

## 7. Feature Specification Catalog

> Split this product feature into one or more coherent, independently testable
> delivery slices, not technical layers. A small feature may need only one spec. Keep
> sequencing dependencies explicit without fragmenting a journey into unusable
> pieces. Use existing Spec Kit feature directory names as spec identifiers.

| Feature slice / spec ID | Spec link or planned status | Slice boundary / delivered value | FRD requirement IDs | Dependencies | Owner / status |
|-------------------|-----------------------------|------------------------------------|----------------------|--------------|----------------|
| 001-feature-name | [Spec](../../specs/001-feature-name/spec.md) | [Slice / value] | FRD-001-R-001 | [None / spec IDs] | [Owner / status] |

> For an uncreated spec, write "Planned - not created" instead of a link.
> Use one primary FRD per spec as a local ownership convention. Reference any
> contributing features and their FRDs explicitly; do not duplicate the spec to claim coverage.

### Spec Kit Handoff

When creating each spec, supply the relevant FRD scope and applicable PRD
policies as input. Preserve the existing Spec Kit sections and add these
traceability fields to the spec header:

```markdown
**Parent PRD**: [PRD ID and link]
**Parent FRD**: [FRD ID and link]
**FRD revision reviewed**: [Version or commit]
**FRD requirement IDs**: [FRD-001-R-001, ...]
**Applicable policy IDs**: [PRD and FRD rule / constraint IDs]
```

In the spec, map each relevant requirement, success criterion, or acceptance
scenario back to its FRD requirement or policy IDs. Update the coverage matrix
below with the resulting spec-local IDs. These are local documentation
conventions; Spec Kit does not automatically create or enforce this hierarchy.

## 8. Requirements Coverage

> This matrix maps feature intent to concrete spec requirements and success
> criteria. Populate exact spec-local IDs after specification; do not invent
> detailed feature requirements here. Qualify IDs with the spec ID because
> FR-001 and SC-001 recur in different specs.

| FRD requirement / policy ID | Spec link | Spec-local requirement / success criterion IDs | Coverage status / gap / deferral rationale |
|------------------------------|-----------|-----------------------------------------------|-------------------------------------------|
| FRD-001-R-001 | [Spec](../../specs/001-feature-name/spec.md) | 001-feature-name:FR-001; 001-feature-name:SC-001 | [Planned / partial / covered / deferred with approval] |

> Include applicable inherited policies and feature-specific rules / constraints.
> A requirement may span several specs; list each contribution. Every requirement
> must have coverage or an explicit disposition. "Covered" means specified,
> not implemented, tested, or accepted.

## 9. Feature Acceptance and Outcome Measurement

> Define evidence that the combined delivery slices achieve the feature outcome,
> including cross-specification business journeys. Do not copy specification-level
> Given/When/Then scenarios. Passing all specification-local tests alone does not
> establish feature acceptance, and delayed product metrics need not block delivery
> acceptance.

### Delivery Acceptance

| Acceptance ID | Required feature-level outcome / measurable threshold | Requirement IDs | Verification method / evidence link | Approver | Result |
|---------------|-----------------------------------------------------|-----------------|-------------------------------------|----------|--------|
| FRD-001-AC-001 | [Observable combined outcome] | FRD-001-R-001 | [End-to-end review / evidence] | [Owner] | [Pending / pass / fail] |

### Outcome Measurement

| PRD metric ID / feature metric ID | Feature contribution / measure | Baseline | Target | Data source / method | Measurement window | Owner |
|-------------------------------|-----------------------------|----------|--------|----------------------|--------------------|-------|
| PRD-001-M-001 | [Contribution, not an automatic claim of product success] | [Value] | [Value] | [Source] | [Period] | [Owner] |

## 10. Open Questions, Assumptions, and Decisions

| ID | Type | Question / assumption / decision | Affected IDs | Owner | Resolve by | Status / resolution |
|----|------|---------------------------------|--------------|-------|------------|---------------------|
| FRD-001-Q-001 | [Question / assumption / decision] | [Description] | [IDs] | [Owner] | [Date] | [Status] |

## 11. Readiness and Change Control

### Ready for Feature Specification

- [ ] Parent PRD revision and linked product goals have been reviewed.
- [ ] Feature scope, ownership, functional requirements, and acceptance outcomes agree.
- [ ] Applicable shared policies, dependencies, and risks are identified.
- [ ] Proposed feature slices and boundaries are recorded.
- [ ] Blocking questions are resolved; non-blocking unknowns have owners and dates.

### Ready for Feature Acceptance

- [ ] Coverage maps each required capability and applicable policy to spec IDs
  or an explicitly approved disposition.
- [ ] Linked specs identify this FRD and its reviewed revision.
- [ ] Delivery evidence satisfies the feature acceptance outcomes.
- [ ] Deferred scope and exceptions have explicit approval.
- [ ] Outcome measurement ownership and follow-up dates are assigned.

### Change Review

On a PRD, FRD, or feature scope change, review affected coverage rows and
downstream specs, plans, and tasks. A reverse link alone does not prove that a
document is current. Resolve conflicting requirements at their authoritative
level and record alignment to the new revision.

| Change / decision | Affected IDs / specs | Impact / required updates | Owner | Review status |
|-------------------|----------------------|---------------------------|-------|---------------|
| [Revision / decision link] | [IDs / links] | [Action] | [Owner] | [Pending / reviewed] |
