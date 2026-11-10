# NOVA V6 — Physical Embodiment Architecture

**Objective:** A Unitree G1 EDU acts as the physical interface for a connected ChatGPT-based assistant, while a separately controlled memory and robot-skill system preserves authorized conversational continuity.

## What is technically possible

- A device mounted on or connected to the robot can run the ChatGPT mobile app as a *conversation interface*, signed into the operator's own account. This does **not** grant the app robot motion controls, access to private model weights or a persistent independent agent runtime.
- A custom application can use properly authorized OpenAI API models for dialogue, perception and tool-use workflows. API model calls are **not the identical ChatGPT app session**, and user account memory is not automatically available through the API.
- Selected user-authorized messages, project notes and memories can be exported, curated and stored in a dedicated retrieval system. This is a separate memory store, not the assistant's hidden internal state.
- A narrow robot-tool bridge can translate high-level requests into manufacturer-supported motions only after bounded safety checks; hard real-time balance, actuator limits and emergency stop remain under dedicated robot controllers.

## Proposed components

```
ChatGPT app on Android (same-account conversation, manual user operation)
        OR custom OpenAI API application (separate app and curated memory)
                    |
        Identity / consent / conversation policy
                    |
          Curated, user-approved long-term memory
                    |
     Cameras / speech / local robot state abstraction
                    |
          Safety and permissions gateway
                    |
          Unitree G1 EDU supported SDK
                    |
     Motion controllers + physical emergency stop
```

**No direct ChatGPT Voice-to-robot motor bridge is guaranteed or currently implemented in this project.** Custom integration must be evaluated against available software interfaces, licensing and provider terms.

## Initial proof-of-concept milestones

- **M0:** confirm EDU programming interfaces and purchase options from Unitree.
- **M1:** demonstrate conversational interface and recalled authorized facts without physical motion.
- **M2:** identify objects and scene context through a permitted camera pipeline, with consent and privacy controls.
- **M3:** execute a single nonhazardous, manufacturer-supported skill under local human supervision and emergency stop.
- **M4:** document reliability, latency, battery life, fall risks, operator confirmation, logging and recovery.

## Safety

Start in a controlled indoor environment. Keep bystanders outside the robot fall envelope. Test emergency-stop, limit joint speeds and forces, secure accounts/keys, record operator approvals, and do not provide unattended operation until an independent engineering safety review. If connectivity or AI inference fails, the system should default to a defined safe controller-managed state.

**Manufacturer and SDK reference:** https://www.unitree.com/g1/
