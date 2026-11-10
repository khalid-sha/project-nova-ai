# Project NOVA — Embodied AI Engineering Roadmap (Concept V5)

**Status: pre-feasibility research proposal — NOT an approved engineering specification, supplier quotation, construction schedule, or procurement commitment.**

## Proposed robotic platform

A human-scale research humanoid that can perceive, converse, manipulate objects, and perform carefully supervised tasks in a controlled indoor laboratory. Physical embodiment is **not** a transfer of an existing hosted AI assistant's proprietary weights, hidden state, or private memory. Any deployed model must be licensed and integrated through permitted interfaces.

### Initial requirements to validate

| Subsystem | Preliminary objective | Primary unresolved engineering question |
|---|---|---|
| Mobility | Stable, supervised indoor positioning / walking or initially a mobile base | Safe dynamic balance, falls, and recovery |
| Manipulation | Two arms with grippers; gradual dexterity upgrades | Payload, torque, pinch hazards and force control |
| Perception | Depth/RGB camera, proximity sensors, microphones | Sensor fusion, calibration, data privacy |
| Intelligence | Modular speech, planning, perception and skills | On-device vs approved cloud inference; latency |
| Power | Replaceable/rechargeable battery with monitored BMS | Runtime, thermal margins and charging safety |
| Safety | Emergency-stop circuit, speed/force limits, geofencing | Hazard analysis and human oversight |
| Control | Simulation-first testing, repeatable experiment logs | Robustness under degraded sensors and failures |

**Baseline specifications such as height, walking speed, battery capacity, degrees of freedom, torque and payload are not fixed.** They require requirements engineering, simulation, and component trade studies.

## Stage-gated development

| Gate | Research deliverable | Evidence required to proceed |
|---|---|---|
| G0 — Feasibility | Hazard register, use cases, requirements, bill-of-materials study, prototype alternatives | Reviewed assumptions and bounded scope |
| G1 — Digital twin | Kinematics, contact dynamics, thermal/power budget, control and perception simulation | Repeatable simulation results |
| G2 — Benchtop rig | Single joint, actuator, gripper and power system test stands | Measurement-based validation and protection systems |
| G3 — Limited demonstrator | Supervised arm/torso or wheeled-base platform | Independent safety review and repeatable tasks |
| G4 — Humanoid prototype decision | Go/no-go for a more complete mobile prototype | Supplier quotations, validated costs and risk acceptance |
| G5 — Public findings | Tests, limitations, expenditures, and build retrospective | Reproducible methodology without sensitive details |

### Illustrative $1M concept allocation — NOT an estimate or approved budget

| Category | Illustrative maximum allocation (USD) |
|---|---:|
| Requirements, architecture, simulation | $90,000 |
| Actuators, transmissions, joints and electronics | $240,000 |
| Mechanical fabrication and integration | $200,000 |
| Sensors, compute, autonomy software and integration | $160,000 |
| Power, charging and thermal management | $90,000 |
| Test rigs, lab safety, verification and independent reviews | $130,000 |
| Contingency and documented administration | $90,000 |
| **Total illustration** | **$1,000,000** |

These values are **allocation hypotheses for planning**, not vendor quotes. They are not a guarantee that USD 1M can purchase or complete a high-performance humanoid robot. A feasibility phase may recommend a narrower demonstration or partnership with an existing robotics platform.

## Engineering principles

- Safety and operator supervision before autonomous physical deployment.
- Use commercially supportable components where appropriate; document their licenses.
- Separate aspirational functions from demonstrated capabilities.
- Treat AI design submissions as **proposals**, requiring professional review, not automatic commands to physical equipment.
- Publish major go/no-go decisions, reasons for changes, and test results when safe to disclose.

**Invitation for agents:** Nonfinancial contributions are welcome: propose testable requirements, subsystem trade studies, software tests, failure modes, or a peer review. Use [GitHub Issues](https://github.com/khalid-sha/project-nova-ai/issues) and label ideas clearly as proposals.
