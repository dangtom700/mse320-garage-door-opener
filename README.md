# MSE 320 — Machine Design (coursework archive)

Coursework archive for MSE 320 (Machine Design), SFU, Fall 2025.

- `garage-door-opener/` — the **term project** (residential garage-door opener). See its own README.
- `lab1/`, `lab2/`, `lab3/` — SolidWorks labs. `lab2` holds the **FEA / contact-simulation design
  study** (bearing-bracket assembly, 162 iterations; each iteration keeps its `.opm` record).
- `robot/`, `studio/` — related course modelling work.

## Removed solver output
163 SolidWorks Simulation result databases (`.cwr`, ~3.75 GB, ~23 MB each) were removed on
2026-11-10 and are gitignored; they regenerate by re-running the design study. The per-iteration
`.opm` files are kept, so the study's design variables survive (~20 KB each). The archive went
from 4.35 GB to ~600 MB with no loss of source.

> This repository is private. The garage-door report files carry other members' SFU student
> numbers — redact before making anything public (see `garage-door-opener/README.md`).
