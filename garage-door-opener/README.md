# Residential Garage-Door Opener — Machine Design (MSE 320)

Full machine design of a residential garage-door opener: a three-stage spur-gear
reduction driving a slider along a linear track, with belt-drive dynamics validated
in SolidWorks Motion and a complete manufacturing drawing package.

**Course:** MSE 320 (Machine Design), Simon Fraser University
**Term:** Fall 2025 (report due 2025-11-30) · **Team project — Group 2, five members**

## My contribution
- Produced the manufacturing drawing package — part and assembly drawings with GD&T and
  tolerancing.
- Derived the control-side electro-mechanical plant model for slider position/velocity
  control and validated belt-drive dynamics in SolidWorks Motion under dynamic loading.
- Sourced standard components (McMaster-Carr — the part numbers are preserved in the
  bearing / coupling / pulley / framing filenames and `.STEP` files) and optimised designs
  against tolerance charts to minimise manufacturing complexity.

The overall mechanism concept was the team's; I am not claiming the full assembly design.

## Layout
| Path | What it is |
|---|---|
| `report/` | Final report (PDF) + progress report (DOCX) — design rationale, alternatives, calculations, BOM |
| `gearbox_3stage_spurGear/` | The delivered drive — gears, shafts 1-4, housing, drum, belt pulley, end plates, plus McMaster `.STEP` parts |
| `project/` | Track/slider, operator, brackets; its `drawings/`, plus superseded `version1/` and `version2/` iterations |
| `drawings-pdf/` | **Exported PDF drawings — the shareable proof of work** (export from SolidWorks into here) |
| `archive/` | `gearbox_rough/` (earlier gearbox iteration) and quarantined SolidWorks `~$` lock files |

## Publishing / proof of work
SolidWorks `.SLDDRW`, `.SLDPRT`, `.SLDASM` do **not** render on GitHub. To share the drawings
as proof, export each drawing to PDF (File -> Save As -> PDF, or Task Scheduler -> Export Files
-> PDF) into `drawings-pdf/` and optionally merge into one package. `.STEP` files open in most
CAD viewers.

## Privacy — redact before going public
> This repository is private and must stay that way until redacted.

The two report files carry the **names and SFU student numbers of five members**, four of whom
are not me. Before making this repo public, or sharing its link beyond someone who needs it,
**redact the student numbers from both documents**, or gitignore the two report files. Those
identifiers are not mine to publish. For applications, link the repo and grant access on request,
or share a redacted extract.

## FEA is a separate item
This term project's bracket and spring sizing was done by analytical hand-calculation (see the
report). The SolidWorks **FEA / contact-simulation design study** is a separate MSE 320 lab and
lives under `../lab2` (bearing-bracket assembly; 162-iteration design study, each iteration
keeping its `.opm` parameter record). Keep the two distinct on a resume.
