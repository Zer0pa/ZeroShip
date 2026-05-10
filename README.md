# ZeroShip

## What This Is

ZeroShip is the public ship-design platform surface for Zer0paShip: architecture, status, evidence, and boundaries without internal code or runtime access.

This repo shows how the design machine is structured and where the current public boundary sits. Ship truth promotion still happens only through the governed private vessel lane and is surfaced separately in the sibling Hull 20098 repo.

## Information Architecture

This repo is one of three distinct surfaces in the Zer0paShip program. Promotion does not flow between them implicitly; each surface owns a bounded scope.

| Surface | Owns | Does not promote |
|---|---|---|
| `Zer0pa/ZeroShip` (this repo) | Public ship-design platform: 15 dimensions, 6 cross-cutting services, 7 public candidate cases, V_01..V_04 audit. | Vessel authority. Class approval. Yard package. Manufacturing release. 23 kn commercial closure. |
| `Zer0pa/Zero-Class-Vessel-Hull-20098` (public sibling) | Public vessel authority packet for Hull 20098: 14.36 MW @ 23 kn baseline, 10,955 t loaded displacement, 14.35 MW hydro anchor, V_01..V_04 PASS. | Class approval. Yard package. Manufacturing release. Lawful one-unit-out 23 kn commercial closure. |
| Private working repo (authority-gated) | Implementation, runtime, CAD, raw CFD, OEM/vendor/partner data, premium relaunch authorization. | Anything in the private repo remains gated outside both public surfaces and is not promoted from platform work alone. |

Platform work in this repo can enable ship work, but does not promote ship truth by itself. Ship truth promotion happens only through the governed private working repo and is surfaced separately in the Hull 20098 sibling.

## Ship Mechanics

| Field | Value |
|-------|-------|
| Profile | ship_platform |
| Architecture | SHIP_SYSTEM_STREAM |
| Encoding | PUBLIC_EVIDENCE_SURFACE_V1 |
| Public chain | SourceEstate -> RuntimeAdmission -> CaseState -> ExecutionStateMachine -> Observability -> FastLaneAdmission -> ResumeController |
| Truth surfaces | ShipTruth -> PlatformTruth -> RuntimeTruth -> SalvageTruth -> NextRunAuthority |
| Boundary | Platform work can enable ship work, but does not promote ship truth by itself. |

## Key Metrics

| Metric | Value | Baseline |
|--------|-------|----------|
| PLATFORM_DIMENSIONS | 15 | public scope markers |
| CROSS_CUTTING_SERVICES | 6 | service groups |
| PUBLIC_CANDIDATE_CASES | 7 | public registry |
| RUNTIME_ROLES | 3 | public substrates |

> Source: `proofs/artifacts/2026-05-03-ship-mechanics-refresh/platform_snapshot.json`

## Repo Identity

| Field | Value |
|-------|-------|
| Identifier | ZEROSHIP_PUBLIC_PLATFORM_SURFACE |
| Repository | https://github.com/Zer0pa/ZeroShip |
| Portfolio / domain | Zer0paShip / ship-design platform |
| Visibility | PUBLIC |
| Default branch | main |
| Authority source | `proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md` |
| License | No open-source license in this repo; public materials remain rights-reserved unless explicitly stated otherwise. |
| Last verified | 2026-05-03 |

## Readiness

| Field | Value |
|-------|-------|
| Verdict | ACTIVE |
| Public position | Controlled pause and convergence |
| Ship truth changed here | No |
| Relaunch authorized here | No |
| Current gate | Internal readiness surfaces must be reconciled before a refreshed current packet is final. |
| Source | `proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md` |

### Honest Blocker

Premium runtime relaunch and ship-truth promotion remain blocked until the private working repo reconciles the current readiness boundary and authorizes one bounded restart route.

## What We Prove

- ZeroShip exposes a stable public architecture chain for the ship-design platform.
- Platform work is separated from ship truth by explicit public boundary rules.
- The public state is controlled pause and convergence, not abandonment.
- Public updates can move platform status without leaking private code, runtime credentials, CAD, raw CFD estates, or partner data.
- The public story is a falsification-governed design machine, not a source-code release.

## What We Don't Claim

- No public source-code release for the private implementation.
- No ship-truth promotion from platform work alone.
- No public CAD, raw CFD estate, OEM data, vendor data, or partner data.
- No hosted SaaS, operator runtime access, runtime credentials, or premium relaunch authorization.
- No class, construction, vessel, or Hull 20098 commercial claim from this repo.

## Verification Status

| Code | Check | Verdict |
|------|-------|---------|
| V_01 | README uses the Ship Mechanics first-ten-zone spine | PASS |
| V_02 | Displayed proof anchors resolve inside this repo | PASS |
| V_03 | Public status preserves controlled pause and convergence without ship-truth promotion | PASS |
| V_04 | Public packet excludes private paths, secrets, runtime access, CAD, raw CFD, and partner data | PASS |

## Proof Anchors

| Path | State |
|------|-------|
| `proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md` | VERIFIED |
| `proofs/artifacts/2026-05-03-ship-mechanics-refresh/platform_snapshot.json` | VERIFIED |
| `proofs/artifacts/2026-05-03-ship-mechanics-refresh/public_boundary.md` | VERIFIED |
| `validation/results/public_surface_status.json` | VERIFIED |
| `docs/ARCHITECTURE.md` | PUBLIC-BOUNDARY |
| `docs/LEGAL_BOUNDARIES.md` | PUBLIC-BOUNDARY |

## Repo Shape

| Field | Value |
|-------|-------|
| Proof Anchors | 6 display anchors |
| Major directories | `docs/`; `proofs/`; `validation/`; `diagrams/`; `legacy-concepts/` |
| Validation result | `validation/results/public_surface_status.json` |
| Sibling surface | `Zero-Class-Vessel-Hull-20098` |
| Authority source | `proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md` |
| Support sections | Quick Start; development status; architecture; rights and exclusions |

## Quick Start

```bash
git clone https://github.com/Zer0pa/ZeroShip.git
cd ZeroShip
sed -n '1,220p' README.md
sed -n '1,240p' DEVELOPMENT-STATUS.md
find proofs -maxdepth 3 -type f | sort
```
