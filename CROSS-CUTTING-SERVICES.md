# Cross-Cutting Platform Services

> Source: `workstreams/ws-arch/architecture/ARCH-001-zeroship-end-to-end-architecture.md` — section 5

Six services operate across all fifteen dimensions rather than being embedded within individual spiral stages.

---

## 1. Basis And Chronology Control

Maintains one active vessel basis, one challenger set, one dead-prior register, and one source hierarchy. Ensures that every dimension operates against the same frozen vessel state and that changes to the basis propagate consistently.

**Touches:** All dimensions (D0–D14). Primary governance of D0.

## 2. Runtime And Authority Admission

Binds each computational task to an admissible compute surface and preserves custody of results. Fail-closes when runtime, telemetry, or provenance constraints are not met. Prevents results from entering the authority estate without traceable computation.

**Touches:** All dimensions during execution. Primary governance of D7 (electrical) and D14 (synthesis).

## 3. OEM And Bounded-Surrogate Intake

Normalizes external component data — OEM vendor data, bounded surrogates, and custom components — into one embodiment layer. Applies a single intake rule: OEM data first (preferred), bounded surrogates second (with explicit truth class and replaceability), custom components third (promoted as explicit branch, not smuggled).

**Touches:** D6 (plant/vendor positions), D8 (propulsor selection), D9 (arrangement/component placement).

## 4. Dependency And Rerun Planning

Maintains which dimensions feed which others. When an upstream dimension changes (e.g., D5 storage basis is revised), the dependency graph determines which downstream dimensions require rerun versus which can consume cached results.

**Touches:** All dimensions. Governs the directed acyclic graph from D0 through D14.

## 5. Proof, Decision, Debt, Kill, And Residual Handling

Records the outcome status of every engineering decision using a four-way classification:

| Status | Meaning |
|--------|---------|
| **Proven** | Result has been verified through computation and meets acceptance criteria |
| **Decided** | A design choice has been made and recorded with rationale |
| **Residual debt** | An open item that has not been resolved but is tracked with explicit intervention plan |
| **Killed** | An alternative that was evaluated and rejected with recorded reasoning |

**Touches:** All dimensions. Primary governance of D14.

## 6. Fast Lane, Data Capture, Publication, And Federation

Builds authority-subordinate acceleration layers for rapid iteration, captures training data from governed runs, and publishes reproducible artifacts. Maintains truth-class boundaries during publication so that OEM data, surrogate data, and custom data are never mixed or misrepresented.

**Touches:** D0 (publication of basis), D12 (augmentation promotion), D14 (synthesis publication). Governs all external-facing artifact production.
