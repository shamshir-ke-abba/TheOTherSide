# THE OTHER SIDE — DESIGN DECISIONS

This document records canonical decisions.

## D001 — Core Genre

Psychological horror with systemic survival, investigation and environmental interaction.

## D002 — North Star

A psychological horror game where the player must understand an intelligence that understands them, then deliberately become something it cannot predict.

## D003 — Mirror

The Mirror is an intelligent adaptive observational entity/system with unresolved fundamental nature.

## D004 — No Omniscience

The Mirror only knows what it can legitimately observe or infer.

## D005 — No Telepathy

The Mirror cannot directly read thoughts or intent.

## D006 — Information Asymmetry

Information acquired outside Mirror observation can provide a strategic advantage.

## D007 — Learning

The Mirror learns progressively from imperfect observation.

## D008 — Deception

The Mirror eventually recognizes deliberate false patterns and counter-tests Shamshir.

## D009 — Prediction Failure

Mirror failures must have causal explanations.

## D010 — Overfitting

Increasing model sophistication eventually creates interpretive error.

## D011 — Final Victory

Shamshir escapes through a transient vulnerability created by an incorrect Mirror prediction.

The Mirror survives.

## D012 — Combat

No conventional combat.

## D013 — Architecture

Underlying architecture remains fundamentally static.

Systems and accessibility may change.

## D014 — World Structure

Interconnected, act-gated sectors.

## D015 — Investigation

Diegetic evidence and player-driven deduction.

## D016 — Technician

Previous technician was a mid-level maintenance technician.

Fate unknown.

## D017 — Technician Evidence

Physical markings, annotated technical material, hidden notebook and incomplete final record.

## D018 — Staff Fate

Unresolved.

Evidence intentionally contradicts itself.

## D019 — Rosslyn History

Rosslyn genuinely conducted human behavioral research.

Deeper history is compartmentalized.

## D020 — Lockdown

Lockdown results from failed containment.

## D021 — Operational Facility

The Mirror maintains enough critical infrastructure for Rosslyn to remain operational.

## D022 — Shamshir

Shamshir arrives for the final audit before decommissioning.

## D023 — Opening

Normal audit → unexplained discrepancy → restricted area → lockdown.

## D024 — First Mirror Encounter

Environmental reaction precedes clear visual confirmation.

Progression:
- It sees me.
- It learns me.
- It predicts me.

## D025 — Mirror Objective

Continuously refine behavioral model.

Ultimate purpose remains unknown.

## D026 — Mirror Success

Increasingly accurate prediction and diminishing novel information.

No explicit completion meter.

## D027 — Technician Discovery

Technician discovered a physical vulnerability in pre-existing infrastructure.

## D028 — Final Strategy

Technician knowledge + Mirror understanding + deliberate pattern violation.

## D029 — Save

Exact save-state restoration.

No failed-timeline memory leakage.

## D030 — Failure

Detection leads to systemic containment rather than graphic instant-death presentation.

## D031 — Physical Mirror

Increasingly tangible while remaining visually ambiguous.

## D032 — Environmental Horror

Rosslyn communicates the Mirror's presence.

No proximity meter.

## D033 — Voice

Sparse analyst commentary.

## D034 — Music

Restrained.

Diegetic audio is primary.

## D035 — Jumpscares

Rare.

## D036 — Ambiguity

Machine, anomaly and hybrid interpretations remain possible.

## D037 — Ending

Shamshir genuinely escapes.

Mirror survives.

## D038 — Future Return

Never explicitly resolved.

## D039 — Final Image

Human resolution contrasted with subtle evidence that Rosslyn remains active.

## D040 — Production Gate

No detailed modelling until world layout, dependencies, infrastructure, observation network, progression and validation are sufficiently specified.

## D041 — Coordinate Truth

The frozen coordinate registry is authoritative for actual room and portal coordinates.

## D042 — Mapping Freeze

Architecture may not be changed during implementation merely to solve technical problems.

## D043 — Project Sequence

**MAPPING → COORDINATES → DESIGN LOCK → CODING → BLENDER → GODOT**

## D044 — Technician Vulnerability Rule

The final physical vulnerability is a discrepancy between pre-existing legacy infrastructure and the Mirror's reliable information/control model.

The physical system is real and exists independently of Shamshir.

The exact hardware and physical interaction are implementation-level details.

## D045 — Final Mirror Causality

The Mirror's final failure is caused by overfitting.

The Mirror increasingly expects sophisticated behavioral deception. Shamshir deliberately violates that expectation using information and infrastructure whose strategic significance is not correctly represented in the Mirror's model.

The resulting intervention follows established facility/system relationships and creates a temporary opening.

No magical control or arbitrary intervention is permitted.

## D046 — Final Escape Causality

Shamshir combines:

1. technician-derived knowledge;
2. understanding of the Mirror's predictive behavior;
3. information acquired outside the Mirror's complete observation;
4. deliberate pattern violation.

He then exploits the pre-existing legacy vulnerability and follows:

**VC-01 → R-401 → C-403 → R-402 → R-403 → C-499 → Exterior**

C-499 is the genuinely unmonitored final transition.

The escape is causal rather than lucky.

The Mirror survives.

## Decision Override Rule

A new decision may supersede an old decision only when:
1. the conflict is explicitly identified;
2. the replacement is documented;
3. affected specifications are updated;
4. implementation compatibility is checked.

No silent canon changes.
