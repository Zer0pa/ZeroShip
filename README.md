# ZeroShip

## What This Is

A ship-first, physics-governed engineering platform for taking a vessel from frozen basis to integrated ship closure across the full MIT ship spiral. The platform implements fifteen engineering dimensions (D0–D14) spanning authority and requirements, margins and service doctrine, energy and plant architecture, propulsion and physical embodiment, weights and stability, dynamics and modifiers, operations and economics, and synthesis and comparison. Six cross-cutting platform services govern all dimensions.

The commercial model centres on vessel-design outputs — design packages, vessel reports, geometry files, authority packs — rather than platform code distribution. The platform itself is internal and private. This repository explains the architecture, not the implementation.

Part of the [Zer0pa](https://github.com/Zer0pa) family. Vessel showcase: [Zero-Class-Vessel-Hull-20098](https://github.com/Zer0pa/Zero-Class-Vessel-Hull-20098).

## Key Metrics

| Metric | Value | Baseline |
|--------|-------|----------|
| DIMENSIONS | 15 | Full MIT ship spiral (D0–D14) |
| CROSS_SERVICES | 6 | Platform-wide governance |
| VESSEL_OUTPUTS | 5 | Per-spiral closure categories |
| SOURCE_MODULES | 94+ | Python + Rust |

> Source: `workstreams/ws-arch/architecture/ARCH-001-zeroship-end-to-end-architecture.md` | `src/zeropa_ship/` module inventory

## What We Prove

- Fifteen engineering dimensions map to and extend the MIT ship spiral, covering every stage from authority and basis through to synthesis and comparison.
- Six cross-cutting services (basis control, runtime admission, OEM intake, dependency tracking, proof/residual handling, publication) operate across all dimensions.
- The platform produces five output categories per spiral closure: lawful ship baseline, challenger comparisons, class/route/economics artifacts, governed evidence estate, and reusable platform corpus.
- The same-basis comparison engine enables honest evaluation of design challengers on one frozen vessel basis and consistent loading/route logic.
- OEM, bounded-surrogate, and custom component data enter through a single governed intake layer with explicit truth-class labeling.

> Source: `workstreams/ws-arch/architecture/ARCH-001-zeroship-end-to-end-architecture.md` — sections 1–5, 21–22

## What We Don't Claim

- No claim of production fleet deployment — the platform is in active development.
- No claim of class-society approval for any vessel designed through the platform.
- No claim that the platform is available as a software product, SaaS, or hosted service.
- No claim of open-source status — all rights are reserved unless expressly granted.
- No claim that third-party tool licences (NavalToolbox, gmsh, OpenFOAM) are granted through this repository.
- No claim that all fifteen dimensions have reached full computational closure for any single vessel.

## Commercial Readiness

| Field | Value |
|-------|-------|
| Verdict | PLATFORM_INTERNAL |
| Surface | Public showcase — architecture and concept |
| Code | Not published |
| Model | Output-only — design packages, not software |
| Engagement | hello@zer0pa.com |

> Evaluators: This is a concept and architecture surface. For deeper technical engagement, contact directly.

## Tests and Verification

The private Zer0paShip repository contains test suites covering hull generation, CFD batch execution, displacement closure, stability validation, authority case materialization, and governed runtime checks. Test harnesses span Python (pytest) and Rust compilation. Phase-specific regression suites validate authority metrics across spiral iterations.

Test code and results remain in the private repository. Selected authority metrics and computed results are published through the vessel showcase repository.

## Proof Anchors

| Artifact | Path (private repo) |
|----------|---------------------|
| Phase 13.2 authority pack | `output/ship/phase13.2-ship-truth-ascent/` |
| Phase 13.1 engineering truth | `output/ship/phase13.1-harsher-engineering-truth/` |
| Phase 4 vessel closure | `output/ship/phase4-vessel-closure-current-canonical/` |
| Phase 12.1 lawful lead | `output/ship/phase12.1-lawful-lead-authority-pack/` |
| Science-engineering pack | `output/ship/phase13.2-science-engineering-authority-pack/` |
| VPC-2.0 frozen spec | `docs/VPC-2.0-spec.md` |

## Repo Shape

**What is in this public repository:**
- Platform architecture and dimension descriptions
- Cross-cutting service definitions
- MIT ship spiral mapping
- Commercial model explanation
- Development status and phase tracking
- Public rights notice and disclaimers

**What is not in this public repository:**
- Source code (Python, Rust, or any other language)
- Solver integrations or internal toolchain wrappers
- Model weights, training data, or prompts
- Credentials, API endpoints, or runtime access
- OEM or vendor-proprietary data
- Deployable software artifacts

## Ecosystem

ZeroShip is the platform layer behind the Zer0pa domain codec family:

| Repo | Domain |
|------|--------|
| ZPE-IMC | Multi-modal integration (platform core) |
| ZPE-Bio | Biosignal |
| ZPE-FT | Financial time-series |
| ZPE-Geo | Geospatial |
| ZPE-IoT | IoT sensor streams |
| ZPE-Ink | Structured document |
| ZPE-Mocap | Motion capture |
| ZPE-Neuro | Neuroscience |
| ZPE-Prosody | Speech prosody |
| ZPE-Robotics | Robotics telemetry |
| ZPE-XR | Extended reality |

Vessel concept showcase: [Zero-Class-Vessel-Hull-20098](https://github.com/Zer0pa/Zero-Class-Vessel-Hull-20098)

## Quick Start

This is a showcase repository — there is no code to run.

- **Platform architecture:** start with [SYSTEM-ARCHITECTURE.md](SYSTEM-ARCHITECTURE.md)
- **Dimension reference:** see [PLATFORM-DIMENSIONS.md](PLATFORM-DIMENSIONS.md)
- **Cross-cutting services:** see [CROSS-CUTTING-SERVICES.md](CROSS-CUTTING-SERVICES.md)
- **Commercial model:** see [COMMERCIAL-MODEL.md](COMMERCIAL-MODEL.md)
- **Current status:** see [DEVELOPMENT-STATUS.md](DEVELOPMENT-STATUS.md)
- **Vessel showcase:** see [Zero-Class-Vessel-Hull-20098](https://github.com/Zer0pa/Zero-Class-Vessel-Hull-20098)

---

> This repository is a public architecture and concept surface for ZeroShip. It does not publish ZeroShip platform code, internal toolchains, training assets, or third-party partner data. Except for limited GitHub service-level permissions associated with public repository visibility, no licence is implied by public posting, and all rights are reserved unless expressly granted in writing.
