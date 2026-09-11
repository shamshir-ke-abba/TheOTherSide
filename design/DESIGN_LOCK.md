# THE OTHER SIDE — DESIGN LOCK

**Status:** DESIGN LOCK COMPLETE
**Phase 19:** PASSED
**Mapping:** COMPLETE
**Coordinate Truth:** FROZEN
**Production Modelling:** NOT STARTED
**Implementation Gate:** OPEN

## 1. Purpose

This is the master design specification between mapping and implementation.

The project sequence is:

**MAPPING → COORDINATES → DESIGN LOCK → CODING → BLENDER → GODOT**

No later implementation phase may redesign the facility or invent a core gameplay rule that is not defined here or in the supporting canonical specifications.

## 2. Non-Negotiable North Star

> A psychological horror game where the player must understand an intelligence that understands them, then deliberately become something it cannot predict.

Every major system, space, interaction, narrative beat, and technical implementation must support this.

## 3. Source-of-Truth Hierarchy

1. Frozen coordinate registry
2. This Design Lock
3. Master specification
4. Decision log
5. Architectural program
6. System state matrix
7. Supporting design documents

Older statements that conflict with the frozen registry are obsolete.

## 4. World

Rosslyn is a believable research facility in the Pacific Northwest, surrounded by dense coastal forest and a controlled perimeter.

The architecture is grounded institutional research architecture with industrial service infrastructure and a mixture of digital and older analog/pre-digital systems.

The building is not a generic futuristic laboratory.

## 5. Architecture

Architecture is fundamentally static.

The following may change between Acts:

- access permissions;
- locks;
- surveillance coverage;
- lighting;
- power states;
- environmental controls;
- alarms;
- system routing;
- operational behavior.

The following should not casually change:

- room dimensions;
- structural walls;
- primary stairs;
- major shafts;
- canonical portals;
- fundamental building topology.

## 6. Facility Hierarchy

### Sector A — Public / Administration

Arrival, reception, records, executive oversight and controlled public-facing infrastructure.

### Sector B — Behavioral Research

Observation, behavioral control, research spaces and evidence concerning human behavioral experimentation.

### Sector C — Security / Data

Diagnostic systems, security infrastructure and server/data functions.

### Sector D — Infrastructure / Utilities

Power, relays, legacy systems, maintenance routes and the final pre-digital escape path.

## 7. Core Spatial Principle

The player should be able to understand Rosslyn spatially.

Important systems should have physical relationships.

A player who studies the facility should be able to form hypotheses about:

- where power originates;
- which doors depend on which systems;
- where surveillance can and cannot see;
- how routes intersect;
- where maintenance access exists;
- where information can become isolated.

## 8. Act Structure

### Act I — The Subject

Primary experience:

- normal institutional environment;
- isolation;
- uncertain infrastructure failure;
- early observation;
- first evidence of abnormal facility response.

Player question:

**“How do I avoid it?”**

Mirror stage:

**Observation → Recognition**

### Act II — The Observer

Primary experience:

- investigation;
- controlled experiments;
- route manipulation;
- false patterns;
- active Mirror adaptation;
- counter-testing.

Player question:

**“How does it know what I do?”**

Mirror stage:

**Prediction → Adaptation → Deception**

### Act III — The Overfit

Primary experience:

- increasingly hostile systemic control;
- reduced safe assumptions;
- deliberate manipulation;
- discovery of information outside the Mirror's model;
- final route through B-2 legacy infrastructure;
- genuine escape.

Player question:

**“What does it not know?”**

Mirror stage:

**Overfitting → Escape**

## 9. Mirror Rules

The Mirror:

- observes;
- learns;
- predicts;
- adapts;
- counter-tests;
- can be wrong;
- can overfit;
- cannot read thoughts;
- cannot access arbitrary engine state;
- cannot know information it could not legitimately observe or infer;
- cannot retain failed-timeline knowledge after reload.

Every meaningful intervention must have a causal chain:

**Observed data → learned pattern → contextual prediction → intervention**

The implementation may choose the exact physical/systemic manifestation of an intervention only when that manifestation remains consistent with the locked system-state, access, surveillance, acoustic and electrical frameworks.

The implementation may not invent magical control, arbitrary hazards, or unexplained knowledge.

## 10. Final Mirror Causality

The final Mirror failure is an **overfitting failure**, not a failure of intelligence.

The locked design rule is:

1. The Mirror observes Shamshir's behavior through legitimate facility pathways.
2. It progressively learns increasingly sophisticated behavioral patterns.
3. It becomes increasingly prepared to interpret late-game deviations as another layered behavioral or systemic deception.
4. Shamshir acquires information through an observation boundary the Mirror does not fully observe.
5. Shamshir deliberately uses that information to make a choice whose strategic significance the Mirror's model does not correctly represent.
6. The Mirror responds according to its incorrect prediction through already-established facility/system relationships.
7. That prediction failure creates a **temporary opening**.
8. Shamshir exploits the opening using the legacy infrastructure vulnerability.
9. The Mirror survives.

The exact visual, hardware, animation and runtime implementation of the intervention are not Design Lock decisions.

The causal relationship is Design Lock.

## 11. Technician Vulnerability

The previous technician was a mid-level Rosslyn maintenance technician.

He:

1. noticed abnormal observation;
2. investigated the infrastructure;
3. discovered a physical vulnerability in pre-existing infrastructure;
4. documented it;
5. attempted to exploit it;
6. failed to complete the final strategy.

The vulnerability is a real discrepancy between physical legacy infrastructure and the information/control model available to the Mirror.

The Mirror is not required to be unable to visually observe the physical system.

The locked rule is instead:

**The physical system exists, but its strategic significance and relevant relationship to the escape route are not fully represented within the Mirror's reliable model.**

The technician discovered this discrepancy and left evidence that allows Shamshir to understand it.

Exact hardware type, physical interaction, animation, control input and implementation mechanism remain implementation details.

## 12. Information Asymmetry

Information acquired outside the Mirror's legitimate observation can provide a strategic advantage.

Air-gapped and physically isolated systems are genuine information boundaries where established by the world design.

The Mirror may observe Shamshir interacting with evidence without automatically receiving the meaning Shamshir derives from it.

The player must never win because the Mirror is arbitrarily blind.

The player wins because the Mirror's available information and interpretation are limited.

## 13. Player

Shamshir is an auditor, not a soldier.

The game rewards:

- observation;
- memory;
- deduction;
- spatial reasoning;
- experimentation;
- patience;
- deliberate action.

There is no conventional combat loop.

## 14. Investigation

Evidence is distributed across:

- environmental details;
- technical records;
- audio/communications;
- architecture;
- maintenance traces;
- technician evidence.

No single document should explain the entire truth.

The notebook is an evidence archive, not a quest tracker or automatic solution generator.

## 15. Previous Technician

The technician's trail demonstrates that someone before Shamshir:

- noticed the abnormal observation;
- investigated the infrastructure;
- discovered the vulnerability;
- documented it;
- attempted to exploit it;
- failed to complete the final strategy.

His fate remains unresolved.

The trail provides knowledge, not an automatic solution.

## 16. Staff Mystery

Staff disappearance remains ambiguous.

The environment must support conflicting interpretations without using gore or explicit confirmation.

Possible evidence may conflict between:

- official paperwork;
- physical traces;
- research records;
- emergency procedures;
- maintenance logs.

The player can establish that something went wrong without receiving a definitive metaphysical explanation.

## 17. Horror

Horror is:

- psychological;
- environmental;
- systemic;
- information-driven.

The facility itself communicates threat.

There is no proximity meter.

There is no conventional enemy HUD.

Jumpscares are rare and subordinate to sustained uncertainty.

## 18. Revisit Principle

A room should feel different because its system state or informational significance has changed, not because its architecture was arbitrarily replaced.

Examples:

- a previously normal corridor becomes monitored;
- a familiar door changes lock state;
- a light circuit becomes unreliable;
- a route that was safe becomes predictable;
- an old system becomes strategically useful.

## 19. Final Escape

The canonical B-2 route is:

**VC-01 → R-401 → C-403 → R-402 → R-403 → C-499 → Exterior**

The escape is not a boss fight.

The causal strategy is:

**technician knowledge + understanding of the Mirror's predictive behavior + information outside the Mirror's model + deliberate pattern violation → prediction failure → temporary opening → legacy vulnerability exploitation → C-499 → exterior**

C-499 is the genuinely unmonitored final transition from Rosslyn interior to exterior.

The exact interaction required to exploit the legacy vulnerability is intentionally not specified at design level.

Shamshir genuinely escapes.

The Mirror survives.

There is no fake-out reversal.

## 20. Design Classification

### LOCKED

- North Star
- core gameplay loop
- Mirror information boundaries
- Mirror causal intervention rule
- Mirror overfitting rule
- technician vulnerability principle
- information asymmetry principle
- non-combat philosophy
- Rosslyn setting
- frozen coordinate registry
- canonical room topology
- B-2 escape route
- genuine ending
- ambiguous Mirror origin
- ambiguous technician fate
- static architecture / dynamic systems
- final escape causal chain

### PROVISIONAL / IMPLEMENTATION-LEVEL

- exact prop inventories;
- exact hardware appearance;
- exact camera/sensor models;
- exact interaction timings;
- exact input mappings;
- exact animations;
- exact collider/node/script structure;
- exact Mirror prediction algorithm;
- exact Mirror intervention manifestation;
- exact save-terminal presentation;
- exact evidence wording;
- exact audio assets.

### OPEN

Only non-core implementation details may remain open.

No open question may require a programmer or artist to invent a core gameplay rule.

### REJECTED

- conventional combat;
- omniscient Mirror;
- telepathic Mirror;
- arbitrary monster roster;
- random behavior as the solution;
- fake-out ending;
- architecture changing merely for spectacle;
- unexplained magical knowledge;
- gore-driven horror;
- generic sci-fi architecture;
- unsupported historical dates treated as canon;
- arbitrary Mirror control unrelated to observed data;
- a programmer-defined final escape rule.

## 21. Production Gate

Phase 19 has passed.

Production may now begin.

The production order remains:

**MAPPING → COORDINATES → DESIGN LOCK → CODING → BLENDER → GODOT**

Implementation must consume the frozen design.

Implementation may resolve presentation and technical details, but may not silently redefine:

- architecture;
- coordinates;
- topology;
- Mirror information boundaries;
- causal prediction rules;
- technician vulnerability principle;
- final escape causality;
- ending.

