# ZeroShip Architecture

## Public Role

ZeroShip is the public control-plane and evidence surface for the private
ship-design platform. It tells the outside world how the machine is organized,
what state it is in, and what boundary rules govern the next lawful move.

## Platform Chain

`SourceEstate -> RuntimeAdmission -> CaseState -> ExecutionStateMachine -> Observability -> FastLaneAdmission -> ResumeController`

## Public Runtime Roles

- `Mac control plane`: planning, state lock, packet assembly, review
- `CPU authority candidate`: lower-cost authority-side compute where lawful
- `GPU support substrate`: acceleration lane admitted only when the current
  packet authorizes it

## Boundary With The Vessel Repo

- ZeroShip explains the platform and its public evidence
- Zero-Class-Vessel-Hull-20098 explains the current vessel truth surface
- Platform work can enable ship work, but it does not promote ship claims on
  its own

## Current Position

The public platform story is currently a controlled pause and convergence
surface. The lawful task is to keep the estate, runtime rules, and public
status coherent until one bounded restart path is admitted.
