# THE OTHER SIDE — VALIDATION RULES

## 1. Purpose

Validation protects the locked map from implementation drift.

## 2. Rule V01 — No Disconnected Major Spaces

Every canonical major space must have at least one valid topological connection unless explicitly designated as sealed or intentionally inaccessible.

## 3. Rule V02 — Valid Portals

A portal must:
- connect touching spaces;
- have a valid center;
- have a compatible opening;
- have compatible floor elevation;
- not bridge a gap.

Corner-only contact is invalid.

## 4. Rule V03 — Escape Blind-Spot Continuity

The Act III escape must contain a continuous sequence of genuinely unmonitored/isolated spaces from B-2 to exterior.

The route must be physically represented by the coordinate registry.

## 5. Rule V04 — Circuit Dependency Integrity

Every electronic door must trace to a valid parent power/access-control dependency.

No door may work because code says it works.

## 6. Rule V05 — Vertical Clearance

Player walking routes must maintain the required clear height.

Default design target: `2.4 m` minimum.

## 7. Rule V06 — Save Accessibility

At least one diagnostic/save terminal must be reachable in each Act without creating an unavoidable progression deadlock.

## 8. Rule V07 — Coordinate Consistency

Blender source, exported GLB, Godot import and collision must preserve the same spatial relationships.

## 9. Rule V08 — Collision/Visual Agreement

Collision must correspond to intended physical architecture.

No collision-only walls.

No visible architectural wall without a corresponding intended physical boundary where traversal requires it.

## 10. Rule V09 — Mirror Causality

Every meaningful Mirror intervention must be traceable to:

**Observed data → learned pattern → contextual prediction → intervention**

The exact runtime algorithm and physical manifestation are implementation-level, but the causal relationship is mandatory.

## 11. Rule V10 — No Hidden Knowledge

The Mirror may not use:
- engine state;
- player intent;
- unobserved information;
- failed-timeline memory.

## 12. Sign-Off

A production build is not accepted until all mandatory rules pass.
