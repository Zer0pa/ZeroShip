# ZeroShip

## What This Is

ZeroShip is the public architecture and evidence surface for the ship-design
engineering platform behind the Zer0pa vessel programme. It shows how the
design machine is structured, how public status is reported, and where the
current boundary sits without publishing internal code, partner data, or
runtime access.

This repo is useful now for following platform progress, diligence posture,
and weekly state changes. Ship-truth promotion still happens only through the
governed vessel lane and is surfaced separately in the sibling vessel repo.

| Field | Value |
|-------|-------|
| Architecture | SHIP_SYSTEM_STREAM |
| Encoding | PUBLIC_EVIDENCE_SURFACE_V1 |

## Key Metrics

| Metric | Value | Baseline |
|--------|-------|----------|
| DIMENSIONS | 15 | D0-D14 |
| CROSS_CUTTING | 6 | services |
| CANDIDATE_CASES | 7 | registry |
| RUNTIME_ROLES | 3 | substrates |

> Source: `proofs/artifacts/2026-04-19-showcase-refresh/platform_snapshot.json`

## What We Prove

- ZeroShip exposes one stable public architecture chain: `SourceEstate -> RuntimeAdmission -> CaseState -> ExecutionStateMachine -> Observability -> FastLaneAdmission -> ResumeController`
- Platform work is separated from ship truth by explicit public boundary rules
- The current public state is a controlled pause-and-convergence surface, not an abandonment surface
- Weekly public updates can move the platform surface forward without leaking private code or partner data

## What We Don't Claim

- No public source-code release for the ZeroShip implementation
- No ship-truth promotion from platform work alone
- No public OEM, vendor, or third-party solver data
- No authorized premium-runtime relaunch while the current pause packet keeps that route blocked
- No hosted SaaS or operator runtime access from this repo

## Commercial Readiness

| Field | Value |
|-------|-------|
| Verdict | PARTIAL |
| Commit SHA | aec2256 |
| Confidence | 84% |
| Source | proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md |

## Tests and Verification

| Code | Check | Verdict |
|------|-------|---------|
| V_01 | README contract matches the showcase playbook | PASS |
| V_02 | Proof anchors resolve inside this repo | PASS |
| V_03 | Public status packet reflects the 2026-04-19 pause state | PASS |
| V_04 | Public packet excludes private paths, secrets, and runtime access | PASS |

## Proof Anchors

| Path | State |
|------|-------|
| `proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md` | VERIFIED |
| `proofs/artifacts/2026-04-19-showcase-refresh/platform_snapshot.json` | VERIFIED |
| `proofs/artifacts/2026-04-19-showcase-refresh/pause_and_resume_boundary.md` | VERIFIED |
| `validation/results/public_surface_status.json` | VERIFIED |

## Repo Shape

| Field | Value |
|-------|-------|
| Proof Anchors | 4 |
| Public Packet | 2026-04-19 showcase refresh |
| Sibling Surface | Zero-Class-Vessel-Hull-20098 |
| Authority Source | proofs/manifests/CURRENT_PUBLIC_STATUS_PACKET.md |

## Quick Start

```bash
git clone https://github.com/Zer0pa/ZeroShip.git
cd ZeroShip
sed -n '1,200p' README.md
sed -n '1,240p' DEVELOPMENT-STATUS.md
find proofs -maxdepth 3 -type f | sort
```
