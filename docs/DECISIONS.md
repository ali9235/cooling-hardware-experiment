# VOLTRA Thermal Lab: engineering decisions

These explain the **current inspectable design/documentation**, not why the owner originally bought components. Original selection history and personal debugging experiences have not been supplied.

| Decision | Current-file rationale | Alternative / trade-off | Constraint |
| --- | --- | --- | --- |
| Observe before naming the mechanism | Document real parts without guessing Peltier/liquid topology. | An inferred schematic could look complete but lack evidence. | Heat path and part models remain unknown. |
| Do not invent controller software | No sketch is attributed to a visible board without a matching file. | Generic new code would not explain this assembly. | A driver must follow verified interfaces. |
| Measure before comparison | Define ambient/load/probe/power conditions. | A single display reading lacks context. | No capacity, efficiency or cooling improvement established. |

## Challenges: distinguish observed from suggested

Unknown parts and absent firmware are documentation blockers, not solved control-engineering incidents.

No matching firmware, powered demonstration, thermal results, flow rate or efficiency measurement is available.

Troubleshooting suggestions are hypotheses, not incidents already solved. Add a case study only with the observed symptom, reproducible conditions, evidence for the cause, exact change, before/after test and remaining uncertainty. Do not turn design intentions into measured improvements.

[Architecture](ARCHITECTURE.md) · [Validation record](VALIDATION.md)
