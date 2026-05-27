# Legacy Concept Notes

> **All content on this page describes historical thinking that informed the current platform architecture. None of these concepts represent current verified capability or active design decisions unless explicitly stated otherwise.**

> Source: `workstreams/ws-arch/architecture/ARCH-002-zeroship-end-to-end-legacy-thinking.md`

## Purpose

This document preserves selected historical concept branches that were explored during ZeroShip platform development. The archive exists so that future work can recover what the programme once considered, what was tried, what was abandoned, and what survived into the current architecture.

This is not a winner selection. It is a memory surface.

---

## Competing Ship Concepts Explored

`[LEGACY — not current architecture]`

The programme explored multiple vessel identities before converging on the current commercial freighter:

| Concept | Description | Status |
|---------|-------------|--------|
| Polar research vessel | Multi-mission research platform, PC3 ice class, scientific equipment, ROVs, moon pool | `SUPERSEDED` — commercial branch killed research identity |
| Commercial freighter (Option B) | 1,040 TEU container carrier, 1,500 nm corridor, hydrogen-electric | `ACTIVE` — current governing concept |
| Dual-mission hybrid | Single hull serving both polar research and commercial freight | `SUPERSEDED` — deemed architecturally incompatible |
| High-speed sprint variant | 33–46 kn sprint capability with battery surge and THRC | `SUPERSEDED` — 23 kn commercial passage now governs |
| Voyage-only operations | Optimized for single-voyage economics | `ACTIVE` — incorporated into Option B |

---

## Recurring Motifs Across the Legacy Estate

`[LEGACY — historical patterns, not current verified claims]`

The following design themes recurred across multiple branches and phases:

| Motif | Description | Current Relevance |
|-------|-------------|-------------------|
| Ship-first, platform second | The ship is the proving article; the platform is extracted from designing the ship well | Survived — governs current architecture |
| Deep hull as architecture lever | Unusually large depth-to-length ratio enables internal volume, seakeeping, cargo stacking, and stability margin | Survived — embodied in Hull 20098 |
| Hydrogen as primary energy carrier | All branches converged on hydrogen regardless of storage form (compressed, LOHC, LH2; ammonia `[KILLED]`) | Survived — PEM fuel cells are core |
| Low-zone heavy storage | Heavy storage (H2, batteries) placed low in hull to preserve stability and cargo volume above | Survived — canonical arrangement doctrine |
| Four structural columns | Premium cargo support columns doing double duty as primary structure | Survived — in current arrangement |
| THRC as flagship augmentation | Fuel-cell waste heat recovery for bow injection, viscosity reduction, and propulsive power recovery | Deferred — optional future layer, not in core |
| Culture vessel crew model | Every crew member understands every system; AI runs normal operations | Historical philosophy — not operationalized |
| Promotion requires proof | No technology or augmentation advances from concept to core without explicit evidence | Survived — governs platform authority rules |

---

## Dead Branches (Explicitly Killed)

`[LEGACY — these concepts were explored and rejected]`

| Branch | Reason Killed |
|--------|---------------|
| PC3 ice class requirement | Commercial branch does not require polar capability; ghost mass from polar scantlings removed |
| 5× rigid wing mast system | Sails excluded from core; headwind penalty at storm conditions too severe without feathering |
| Ammonia as fuel carrier | Excluded from core due to toxicity, handling complexity, and regulatory burden |
| 33–46 kn sprint speeds | Superseded by 23 kn commercial passage gate; sprint concept tied to dead research branch |
| Moon pool integration | Research heritage; functionally dead in commercial branch |
| Research equipment and ROVs | Tied to polar research identity; removed when commercial branch became governing |
| RED (Renewable Energy Device) as core energy term | Excluded from promoted core-energy assumptions |

---

## What This Archive Preserves

`[LEGACY — archival context only]`

The legacy estate preserves:

- The vocabulary, idea families, and design intuitions that informed the current platform
- The contradictions and competing branches that were deliberately resolved
- The historical parameter ranges (displacement 1,800–14,132 t, LOA 91–147.6 m, plant size 8–40 MW) that show how the design space was explored before convergence
- The augmentation candidates (THRC, air-cavity, riblets, Hull Vane, vortex generators) that remain in the optional-future-layer register
- The materials innovation concepts (Al-Li 2099, WAAM, LFAM, graphene-Al, SMA inserts, titanium stem) that informed current structural thinking
