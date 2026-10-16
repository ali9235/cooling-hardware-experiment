# Thermal Lab: explain what is actually visible

This is a physical hardware study, not a verified cooling product. No matching control sketch, thermal dataset or working-device recording has been supplied. There is no control code to explain as tested firmware.

## Separate a component's purpose from a demonstrated result

| Visible element | Typical purpose | Not established |
| --- | --- | --- |
| 12V-labelled fan | Move air | Actual operating voltage, current or airflow |
| Metal assembly | Part of the fan/thermal mounting structure | Internal stack, cooling technology or heat transfer rate |
| Motor-driven pump and tubing | Move fluid through a suitable path | Complete loop, fluid, ratings, actual flow |
| Partly visible controller | Potential control logic | Board identity, firmware, sensor or feedback behavior |
| Rotary control / external PCB | Visible electrical parts | Exact identity and circuit function |
| Enclosure and wiring | Hold/connect the assembly | Full circuit, waterproofing or electrical protection |

Use the [annotated photo](../media/component-guide.png) to point to parts. Leader lines are not electrical connections. Do not call an unidentified layer a Peltier/TEC or an unidentified module a thermostat.

## The engineering questions to answer next

1. **What creates the temperature difference?** Identify the real thermal element and stack from markings/specifications, without assuming the fan itself produces below-ambient cooling.
2. **Where is heat intended to travel?** Trace mechanical contacts and any real fluid route; distinguish the heat source/load from an exposed surface.
3. **What supplies and switches each load?** Document the fan, pump and any other element independently. The fan's 12V label is not the whole system specification.
4. **What does the controller observe?** Locate an actual sensor and its code before claiming closed-loop regulation.
5. **How will you measure a result?** Choose locations, instruments, load and time history before energizing the identified configuration.

These are investigation steps, not claims that the design already implements them. Historical selection reasons and solved engineering challenges have not been supplied.

## What a credible record contains

An identified parts list, a traced power/signal diagram, genuine firmware if present, photographs of sensor locations, ambient and device readings with elapsed time, and raw observations including failed runs. A colder-looking surface, fan noise or pump motion alone does not establish cooling capacity or efficiency.

If reporting electrical input later, identify the actual measurement points and method. Do not calculate cooling power or efficiency from supply voltage alone. Instrument resolution, placement and a changing ambient temperature affect interpretation.

## Useful learning exercises

- Point to each confirmed item in the real photo and say what you know versus what you still need to identify.
- Draw a **provisional** heat/flow/power diagram with unknown links marked, then replace it only after tracing the real assembly with power disconnected.
- Compare a proposed measurement method against its claim: a surface-temperature change is not the same as cooling capacity.

## Troubleshooting without unsafe guesswork

| Symptom or uncertainty | Next step |
| --- | --- |
| Fan runs but a surface stays warm | Establish the thermal mechanism, load and measurement method; do not assume fan failure |
| Pump appears present but no loop is documented | Identify ports, tubing route and ratings before operation |
| Controller board is visible | Obtain matching firmware and the actual input/output map |
| Moisture or condensation appears near electronics | Stop the test and make the arrangement safe; do not continue for footage |
| No measured result | Publish it as untested hardware investigation, not successful thermal regulation |

There is no firmware build or physical test pass for this update. See the [real demonstration plan](DEMO_TEST_PLAN.md) and [identification checklist](../WIRING_AND_SOURCE.md).
