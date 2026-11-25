# Fictional Machines (working title)

**Project Concept and Classification System v0.6**  
November 24, 2026

> English translation of the Japanese original, [Fictional_Machines.md](Fictional_Machines.md) (v0.6). If the two versions differ, the Japanese original takes precedence.

## 01　Concept and Design Principles

### Purpose

To construct machines that do not exist in reality from both engineering design and fiction, and to realize them in a form that actually works. The scope ranges from machines that could be manufactured with real technology to machines based on fictional components, signals, logic, and physical laws.

### Scope of Subjects

A machine is a system with its own structure and operating principles that produces phenomena in response to inputs, internal state, the passage of time, and so on (provisional definition). Physical existence and practicality are not required. Besides electronic devices, physical mechanisms, computers, software, and games, the components, standards, and laws that make a machine possible are themselves subjects of design.

### Design Principles

**Science-fiction premises are allowed, but the design and behavior built on those premises must meet engineering rigor.**

| Principle | Description |
|---|---|
| Engineering basis | Respect the specifications and characteristics of real technology, and state fictional premises explicitly. |
| Structure and causality | Define the internal structure and operating principles, and derive outputs and behavior from them. |
| Constraints | Define the relevant constraints, such as time, resources, precision, signals, and energy. |
| Execution and verification | Implement at an appropriate level of abstraction, and verify conformance to the specification. |
| Non-ideality and abstraction | Handle failures, noise, and the like where needed, and state which phenomena are omitted and what that omission affects. |

Fiction shapes a machine's purpose, development background, and technological lineage, and the performance and flaws that emerge from implementation can be reflected back into the story. We value letting engineering and fiction develop each other, but a story is not required for every individual work.

<!-- pagebreak -->

## 02　Production Activities and Implementation Methods

Depending on the nature of the machine, combine design, simulation, physical fabrication, and fiction writing.

| Activity | Example methods and deliverables |
|---|---|
| Electronic circuit and board design | KiCad, SPICE, schematics, PCBs, component models |
| Digital logic design | Verilog / SystemVerilog, HDL simulation, FPGA |
| Signal and standard design | DSP, modulation, encoding and decoding, transmission and display formats |
| Software and emulation | C++, Rust, Python, emulators, firmware, SDKs |
| Mechanism and physics simulation | CAD, Isaac Sim, MuJoCo, sensor and mechanism models |
| Virtual environments and games | Unity, Godot, Unreal Engine, world rules, game rules |
| Physical fabrication and measurement | Real circuits, microcontrollers, FPGAs, machining, 3D printing, measurement |
| Fiction writing | Stories, fictional histories of technology, development records, product catalogs, datasheets |

### Separating the Machine Specification from Its Implementations

Manage the machine itself (its structure, components, operating rules, and constraints) as a specification. A single specification can have multiple implementations for different purposes.

| Example implementation | Purpose |
|---|---|
| Fast software emulator | Real-time operation, software development |
| Detailed circuit or physics simulator | Verifying timing, signals, and component characteristics |
| FPGA, real circuits, real mechanisms | Physical operation and measurement |
| Implementation inside a virtual environment | Operation in space, interaction with the environment |

When fidelity differs between implementations, record the differences. Where needed, link heterogeneous simulators together.

### Production Environment

Make use of existing development tools, and accumulate and reuse the component models, standards, tests, and development tools gained from individual works. Collaboration with AI agents is also being considered as a means that spans design, implementation, verification, and documentation.

<!-- pagebreak -->

## 03　Classification A: Fictionality, Era, and Design Origin

The classification is not a ranking. It is a shared vocabulary for describing the nature of each work. Ideas that are out of scope can be classified too, and undecided items and multiple classifications are allowed.

### F — Fictionality

| ID | Category | Definition |
|---|---|---|
| F0 | Real | Reproduction or use of existing machines and specifications. |
| F1 | Unbuilt | A design that could have been built with real technology and components as of a specified date, but never existed. |
| F2 | Unrealized | Could be consistent with real physical laws, but the required components or manufacturing technology have not been realized. |
| F3 | Idealized | Idealizes or removes real constraints, such as perfect precision or infinite capacity. |
| F4 | Virtual-world-specific | Works under its own physical laws, logic, space, and time. |
| F5 | Contradiction / causal deviation | Expresses behavior that departs from ordinary logic and causality through its own consistent execution rules. |

F is not a strict ordering. Describe the reference world and point in time, and what exactly is fictional.

### T — Temporal Constraint

| ID | Definition |
|---|---|
| T0 | No era constraint. |
| T1 | References the technology and style of a specific era. |
| T2 | Limited to components and technology available by a specified date. Example: T2:1985. |
| T3 | Reproduces not only the technology but also the economic, social, and manufacturing conditions of the time. |

Under T2, respect component performance, physical characteristics, and manufacturability at the time, while budget and commercial rationality may be relaxed. The use of modern design and verification tools is kept separate from the technical constraints of the target machine itself.

### D — Design Origin (multiple choices allowed)

| ID | Approach | ID | Approach |
|---|---|---|---|
| D0 | Reproducing an existing machine | D4 | Extending an existing machine |
| D1 | Repurposing | D5 | Combining components and technologies |
| D2 | Reprogramming | D6 | Original architecture or principle |
| D3 | Modifying circuits or structure | D7 | Designing components, signals, or fundamental laws |

Given / Designed: describe which constraints are fixed and which elements are newly designed.

<!-- pagebreak -->

## 04　Classification B: Design Domain and Engineering Integrity

### Scope — Unit of Design (multiple choices allowed)

Principle, Component, Module (functional block), Standard, Machine, System (composite system), Ecosystem (technology ecosystem), World.

### L — Technical Layer (multiple choices allowed)

| ID | Domain | Examples |
|---|---|---|
| L0 | Fundamental laws | Physical laws, time, space, basic rules of computation |
| L1 | Physical structure | Mechanisms, materials, shapes |
| L2 | Components | Electronic components, sensors, actuators |
| L3 | Circuits and logic | Electronic circuits, digital logic |
| L4 | Standards and formats | Video, communication, encoding, transmission |
| L5 | Architecture | CPU, instruction set, memory, bus |
| L6 | System software | OS, firmware, runtime |
| L7 | Applications | Games, UI, applications |
| L8 | World and environment | Game rules, virtual environments, world state |

L is not a strict hierarchy. Distinguish the design target (for example, hardware) from the implementation medium (for example, software).

### E — Engineering Integrity

| ID | Definition |
|---|---|
| E0 | Appearance and setting only. No operating principle. |
| E1 | Reproduces surface-level inputs, outputs, and functions. Internal principles are undefined. |
| E2 | Internal structure and operating principles are defined and can be explained consistently. |
| E3 | Relevant component characteristics, constraints, inputs and outputs, and temporal behavior can be verified. |
| E4 | Systematically handles relevant non-idealities, failures, and the effects of design changes. |

E expresses the consistency of the design and the completeness of its description. It is independent of verification results (V) and simulation fidelity (S). Aim for E2 or higher during production, and roughly E3 or higher on completion.

<!-- pagebreak -->

## 05　Classification C: Implementation Medium, Fidelity, and Verification

### M — Implementation Medium (multiple choices allowed)

| ID | Medium | ID | Medium |
|---|---|---|---|
| M0 | Specifications, schematics, etc. | M4 | FPGA, etc. |
| M1 | Software / emulator | M5 | Real electronic circuits / PCB |
| M2 | Circuit / HDL simulator | M6 | Real mechanisms / physical machines |
| M3 | Virtual environment / physics simulator | M7 | Mix of real and virtual |

### S — Simulation Fidelity

| ID | Aspect | Examples |
|---|---|---|
| S0 | Representation | Appearance, display, presentation |
| S1 | Function | Inputs and outputs, functional behavior |
| S2 | Internal structure | Internal state, memory, relationships among components |
| S3 | Time and timing | Clocks, processing delays, synchronization, cycle accuracy |
| S4 | Signals | Waveforms, voltages, modulation, signal transmission |
| S5 | Components and elements | Behavior of individual components and mechanisms |
| S6 | Physical phenomena | Electromagnetism, materials, mechanics, etc. |

S is not a cumulative level but a per-aspect fidelity profile. For each implementation, record the reference specification, granularity and tolerance, omissions, and non-idealities. The fidelity of a fictional machine is treated as conformance to its defined machine specification, component models, and laws. For example, a fictional game console may emphasize cycle accuracy of the CPU and bus and the video and audio waveforms, while omitting transistor-level reproduction of every element.

### V — Verification: Methods and Status (multiple choices allowed)

| ID | Definition |
|---|---|
| V0 | Unverified. |
| V1 | Verified by theory, equations, or specification. |
| V2 | Verified by test code or simulation. |
| V3 | Verified by comparison between different implementations or independent models. |
| V4 | Measurement and experiments with real components, real circuits, or real machines. |

Record the target of verification, the conditions, the acceptance criteria, and the unverified parts. Distinguish the current status from the goal, and do not require physical measurement across the board.

<!-- pagebreak -->

## 06　Classification D: Fiction and Selection

### N — Narrative Integration

| ID | Definition |
|---|---|
| N0 | No fiction. |
| N1 | Name, purpose, and a simple background. |
| N2 | A story covering the development history, the manufacturer, the social background, and so on. |
| N3 | The story or world setting influences the machine's specification and design. |
| N4 | Behavior arising from the implementation and the fiction develop each other. |

### Selection Criteria

| Decision | Condition |
|---|---|
| Main work | Has new fictionality, and aims at engineering design of its internal structure and operating principles, together with execution and verification. |
| Design candidate / on hold | Fits the intent, but its operating principles or implementation approach are undecided. |
| Side work / basic experiment | Analysis or reimplementation of existing machines, etc. |
| Generally out of scope | Appearance, setting, or output effects only, with no aim at engineering design. |

### Classification Examples (targets on completion; provisional)

| Subject | F / E / T | Main L / Scope | N | Decision |
|---|---|---|---|---|
| Fictional retro game console (with historical constraints) | F1/E4/T2 | L2–7 / Machine | N3 | Main |
| Original video format | F1/E3/T0 | L3, L4 / Standard | N0–3 | Main |
| Machine with its own physical laws | F4/E3/T0 | L0, L1, L8 / Machine | N3 | Candidate |
| Reimplementation of an existing game console | F0/E4/T0 | L3, L5 / Machine | N0 | Basic |
| Appearance-only SF device | F undecided/E0/T0 | L1 / Machine | N2 | Out of scope |

<!-- pagebreak -->

## 07　Describing Individual Projects

### Common Description Format

| Item | Contents |
|---|---|
| Basic information | ID, name, summary, purpose, selection, development status |
| Design boundary | F, T, D; reference date and world; Given / Designed |
| Machine specification | Scope, L, E; structure, components, operating principles, inputs and outputs, constraints, non-idealities |
| SF premises | Fictional assumptions, deviations from reality, characteristics, scope of effect |
| Implementation and verification | M, S, and V for each implementation; tools; abstractions; tests and acceptance criteria |
| Fiction | N; background setting; story; correspondence with the technical specification |
| Deliverables | Specifications, design data, code, measurement results, narrative materials, etc. |

### Example: Local-Gravity-Switching Conveyor

| Item | Example |
|---|---|
| Basic information | EX-01. A device that conveys objects by switching the direction of gravity. Purpose: conveyance. Selection: description example. Development status: hypothetical design stage. |
| Design boundary | F4 / T0 / D5, D7. Based on ordinary mechanics; the switching rules for local gravity and the conveying mechanism are newly designed. |
| Machine specification | Scope: Machine. L0, L1, L8 / E3 (target). Consists of a conveyor path, gravity-switching zones, and a controller. The input is a direction command, and the output is the movement of objects. Collisions and friction are taken into account. |
| SF premises | The direction of gravity acting on conveyed objects within a designated zone can be changed in 90-degree steps. The acceleration magnitude is assumed to be 9.81 m/s², and the switching time 0.2 s. The mechanism that generates the gravity field is not modeled. |
| Implementation and verification | M3 (physics simulator). S3 and S6: reproduces switching time, motion, and contact. V0 (current) → V2 (target). Verifies the time from command to completion of conveyance, and arrival at the designated position. |
| Fiction | N1. Set as conveyance equipment in a world where local gravity control technology exists. |
| Deliverables | Machine specification, physical model, control code, simulation results. |
