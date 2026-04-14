# Platform Dimensions Reference

> Source: `workstreams/ws-arch/architecture/ARCH-001-zeroship-end-to-end-architecture.md`

Technical reference for the fifteen ZeroShip platform dimensions. Each dimension lists platform surfaces, upstream inputs, outputs produced, and downstream consumers.

---

## D0 — Authority, Basis, Chronology

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Basis registry, frozen specimen manifest, challenger registry, dead-prior register, lane rules, authority stack |
| **Inputs** | External requirements, programme authority, owner instruction |
| **Outputs** | Lawful basis hash, consistent source hierarchy |
| **Downstream** | All dimensions (D1–D14) consume the basis hash |

## D1 — Hull And Hydrodynamic Specimen

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Hull truth surface, hydrodynamic anchor pack, modifier registry, geometry reopen gate, hull residual ledger |
| **Inputs** | D0 basis hash, hull parametric search results |
| **Outputs** | Frozen specimen, controlled modifier register |
| **Downstream** | D8 (propulsor efficiency chain), D9 (arrangement), D10 (mass/wetted area), D12 (seakeeping) |

## D2 — Mission And Operating Doctrine

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Mission basis, operating-profile set, speed doctrine, route-family set, port/standby assumptions |
| **Inputs** | D0 basis hash, owner requirements |
| **Outputs** | Machine-readable mission model |
| **Downstream** | D3 (reserve doctrine), D4 (service loads), D5 (storage endurance), D13 (route/economics) |

## D3 — Reserve And Redundancy Doctrine

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Reserve doctrine, casualty requirement matrix, common-mode policy, black-start philosophy, degraded-speed targets |
| **Inputs** | D2 mission model |
| **Outputs** | Reserve rules for plant sizing, ESS role, electrical segmentation |
| **Downstream** | D6 (plant sizing), D7 (electrical segmentation), D8 (casualty speed) |

## D4 — Service-Load Model

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Itemized service-load book, underway/port/emergency load cases, transient factors, load-shedding hierarchy |
| **Inputs** | D2 mission model, D3 reserve doctrine |
| **Outputs** | Itemized service-load model |
| **Downstream** | D6 (plant sizing), D7 (electrical demand), D13 (range/endurance) |

## D5 — Fuel And Storage Basis

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Storage basis, tankage cases, usable-energy cases, storage mass/volume breakdowns, grouping logic, storage residuals |
| **Inputs** | D2 mission model, D3 reserve doctrine |
| **Outputs** | Explicit storage basis |
| **Downstream** | D6 (plant architecture), D9 (arrangement/tankage), D10 (mass book), D13 (range) |

## D6 — Prime Power, ESS Role, And Module Zoning

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Plant architecture, module count/zoning, ESS role contract, ESS size band, cooling architecture, vendor-position rows |
| **Inputs** | D3 reserve doctrine, D4 service loads, D5 storage basis |
| **Outputs** | Machinery architecture (plant, ESS, cooling) |
| **Downstream** | D7 (electrical input), D8 (delivered power), D9 (arrangement), D10 (mass) |

## D7 — Electrical Architecture And Control

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Single-line diagram, bus family, segmentation rules, converter architecture, black-start path, protection logic, load-shedding policy |
| **Inputs** | D6 plant architecture, D3 reserve doctrine |
| **Outputs** | Electrical architecture |
| **Downstream** | D8 (delivered power mapping), D9 (arrangement), D11 (class-facing), Cross-cutting services |

## D8 — Propulsor Topology, Delivered Power, And Casualty Transmission

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Propulsor trade matrix, delivered-power map, efficiency chain, manoeuvring assumptions, casualty-speed matrix |
| **Inputs** | D1 hull specimen, D6 plant, D7 electrical |
| **Outputs** | Same-basis propulsor architecture |
| **Downstream** | D9 (arrangement), D10 (mass), D12 (motion/seakeeping), D13 (range) |

## D9 — Machinery Integration, General Arrangement, Routing, And Hazard

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Arrangement integration map, GA results, routing continuity, hazard interface map, maintenance matrix, removal paths |
| **Inputs** | D5 storage, D6 plant, D7 electrical, D8 propulsor |
| **Outputs** | Physical integration surface |
| **Downstream** | D10 (mass/centres), D11 (structure/stability) |

## D10 — Mass Build-Up, Centres, Loading, And Tankage

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Mass book, centres book, loading-case set, tank fill matrix, ballast logic, cargo distributions |
| **Inputs** | D1 hull, D5 storage, D6 plant, D8 propulsor, D9 arrangement |
| **Outputs** | Controlled weight and centre states |
| **Downstream** | D11 (stability), D12 (motion), D13 (economics) |

## D11 — Structure, Stability, Damage, And Class-Facing Package

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Structure package, intact/damage stability, compartmentation logic, class gap register, yard release boundary |
| **Inputs** | D9 arrangement, D10 mass/centres |
| **Outputs** | Class-facing posture |
| **Downstream** | D12 (motion constraints), D13 (economics), D14 (verdict) |

## D12 — Motion, Seakeeping, And Augmentation Verification

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Motion case matrix, seakeeping results, augmentation promotion report, route-weather interface, runtime gap register |
| **Inputs** | D1 hull, D10 mass/loading, D11 stability |
| **Outputs** | Dynamic-behaviour envelope, modifier promotion/hold/kill |
| **Downstream** | D13 (route operability), D14 (verdict) |

## D13 — Range, Route, Endurance, And Economics

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Range matrix, route-sensitivity set, economic-speed report, cargo-range trade matrix, weather-duty factors, endurance cases |
| **Inputs** | D2 mission, D5 storage, D8 delivered power, D10 mass, D12 weather duty |
| **Outputs** | Operational picture (range, speed, economics) |
| **Downstream** | D14 (verdict) |

## D14 — Synthesis, Promotion, And Residual Closure

| Field | Detail |
|-------|--------|
| **Platform surfaces** | Same-basis comparison engine, promotion log, residual ledger, cycle decision brief, challenger status |
| **Inputs** | All dimensions (D0–D13) |
| **Outputs** | Branch verdict, residual ledger, next-route manifest |
| **Downstream** | Feeds back to D0 for next spiral iteration |

---

## Dependency Summary

```
D0 ──→ D1 ──→ D2 ──→ D3 ──→ D4
                      │       │
                      ├── D5 ←┘
                      │
               D6 ←── D5
               │
        D7 ←── D6
        │
 D8 ←── D7 + D1
 │
 D9 ←── D5 + D6 + D7 + D8
 │
 D10 ←─ D1 + D5 + D6 + D8 + D9
 │
 D11 ←─ D9 + D10
 │
 D12 ←─ D1 + D10 + D11
 │
 D13 ←─ D2 + D5 + D8 + D10 + D12
 │
 D14 ←─ ALL (D0–D13)
 │
 └──→ D0 (next iteration)
```
