# Thermal Lab: turn an assembly into measured evidence

**Status: planned, not performed.** Do not energize unknown hardware simply to create a demonstration.

## Identification gate

Use [WIRING_AND_SOURCE.md](../WIRING_AND_SOURCE.md). Identify the actual thermal element, fan/pump ratings, supply/protection, controller role, fluid route if any, and instrument placement. Disconnect power before tracing or adjusting wiring. Keep liquids and condensation away from exposed electronics. Do not infer all load ratings from the fan label or operate an unidentified pump dry.

## Record 60–90 seconds only after safe commissioning

1. Show the real assembly and readable part markings. Identify known and unknown components.
2. Show actual measurement locations, ambient conditions and instruments, with units visible.
3. Show the declared configuration/load and an honest time-based observation. For a long run, disclose editing/time compression and preserve the raw record.
4. Explain one result and one limitation. If the mechanism is still unidentified or no thermal run was safe, show the identification work instead of claiming cooling.

## Measurement cases

| ID | Case | Keep | Acceptance basis |
| --- | --- | --- | --- |
| T1 | Identification | Markings, ratings, traced unpowered connections | Unknowns remain unknown; no assumed cooling technology |
| T2 | Instrument baseline | Ambient and unpowered measurement locations, instrument details | State placement, units and instrument limitations |
| T3 | Supervised time series | Configuration/load, elapsed time and actual temperatures | Preselect duration/criteria; compare like-for-like conditions |
| T4 | Pump/flow path, if verified | Identified route and suitable actual flow observation | Assess the real pump specification; not inferred from visible tubing |

Record [hardware-observations.csv](../tests/hardware-observations.csv). Every row is `not_run`. Add repeated rows for a time series and record the instrument/reference—not guessed temperatures. Preserve the raw failed or inconclusive result.

No below-ambient result, heat-load capacity, efficiency, closed-loop stability or cooling-performance claim is justified until its corresponding evidence exists.
