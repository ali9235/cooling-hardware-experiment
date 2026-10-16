# VOLTRA Thermal Lab: testing and validation

## Scope and actual results

[Machine-readable software-check record](../tests/evidence/2026-10-16-software-checks.json) · This record contains actual software checks and explicit exclusions, not fabricated sensor data.

Evidence inspection/documentation checks only. No application firmware to compile and no performed thermal bench test.

No powered thermal test was performed; matching application firmware was not found.

## Reproduce software checks

```powershell
python tools/check_docs.py
# Documentation checks only; no matching firmware to build.
```

The documentation check needs only Python's standard library. See the [real demonstration plan](DEMO_TEST_PLAN.md) for evidence-collection prerequisites.

## Error behavior to inspect

An unknown component is not a verified sensor and missing measurement is not zero cooling. Record failures without inventing a control diagnosis.

## Hardware acceptance

No matching firmware, powered demonstration, thermal results, flow rate or efficiency measurement is available.

The [demo plan](DEMO_TEST_PLAN.md) defines proposed observations. [hardware-observations.csv](../tests/hardware-observations.csv) contains **not_run** rows, not measurements. Add raw values and genuine evidence only after testing.

## Continuous integration

The proposed workflow runs documentation checks. It does not flash hardware, assess photo truth or establish safety. A workflow file is not a passing run; inspect Actions after an authorized push. No success badge is prefilled.

[Security](../SECURITY.md) · [Roadmap](ROADMAP.md)
