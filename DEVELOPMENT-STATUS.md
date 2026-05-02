# Development Status

| Field | Value |
|-------|-------|
| Last Updated | 2026-05-03 |
| Current Position | Controlled pause and convergence under Ship Mechanics profile |
| Ship Truth Changed Here | No |
| Relaunch Authorized Here | No |
| Sibling Vessel Surface | Zero-Class-Vessel-Hull-20098 |

## What Changed This Week

- The public platform surface was migrated to the `Ship Mechanics` Lab Front Door spine.
- The public evidence tree now includes a 2026-05-03 ship-mechanics refresh packet.
- The pause boundary still says plainly that premium runtime relaunch is blocked until the next lawful route is authorized.
- The public architecture story now separates platform truth from ship truth explicitly.

## What Did Not Change

- Ship truth did not move here.
- The vessel baseline remains governed by the ship-facing corridor, not by platform work.
- Phase 14 remains deferred.
- Expensive runtime spend remains blocked until the private working repo reconciles the current readiness boundary and authorizes one bounded route.

## Current Public Metrics

| Metric | Value |
|--------|-------|
| Dimensions | 15 |
| Cross-cutting services | 6 |
| Candidate cases in active public registry | 7 |
| Runtime roles surfaced publicly | 3 |

## Current Public Boundary

- The public platform chain is `SourceEstate -> RuntimeAdmission -> CaseState -> ExecutionStateMachine -> Observability -> FastLaneAdmission -> ResumeController`.
- The governing truth chain is `ShipTruth -> PlatformTruth -> RuntimeTruth -> SalvageTruth -> NextRunAuthority`.
- ZeroShip is the public control-plane and evidence surface, not the ship-claim surface.
- Code, weights, prompts, runtime credentials, CAD, raw CFD estates, and partner data stay private.
- The next lawful move is readiness-boundary reconciliation, then one bounded restart path.

## Next Lawful Move

Finish the readiness-boundary reconciliation, keep the public packet current,
and only reopen an expensive runtime lane after the private repo authorizes one
bounded route.
