# THE OTHER SIDE — COORDINATE SYSTEM

**Status:** LOCKED
**Phase:** Mapping / Coordinate Truth complete
**Implementation:** Not started

## 1. Purpose

This document defines the rules for the canonical Rosslyn coordinate system. It is a spatial contract for later production.

The coordinate registry is authoritative for actual room and portal coordinates. This document defines the rules; it does not replace the registry.

## 2. Canonical World Space

- Origin: `(0, 0, 0)`
- Logical unit: `1 unit = 1 metre`
- Structural grid: `3 m`
- Design snap grid: `1 m`
- Fine placement is permitted only when required by a locked architectural dimension.
- World envelope: `X [-40, 40]`, `Y [-30, 30]`

The origin is the central reference of the Rosslyn Ground Floor plan.

## 3. Axes

The logical design coordinate system is:

- X = east / west
- Y = north / south
- Z = vertical elevation

All mapping decisions are expressed in this system.

Any later Blender export conversion must be documented once. Runtime code must never compensate for an undocumented axis change.

## 4. Floors

| Level | Floor elevation |
|---|---:|
| +1 | `Z = 4` |
| 0 | `Z = 0` |
| B-1 | `Z = -4` |
| B-2 | `Z = -8` |

Nominal floor-to-floor separation is `4 m`.

Typical occupied clear height is `3.2 m`; the remaining `0.8 m` is reserved for structural/services/plenum interpretation where appropriate.

## 5. Architectural Envelope

The mapped building occupies:

`X [-40,40] × Y [-30,30]`

This is the planning envelope, not a statement that every point is occupied.

Unused areas remain intentionally available for circulation, structure, service infrastructure, setbacks, or later detailed architectural subdivision only when justified by the Design Lock.

## 6. Structural Rules

- Primary structural module: `3 m × 3 m`
- Secondary planning module: `1 m`
- Standard interior wall thickness: `0.2 m`
- Standard exterior wall thickness: `0.4 m`
- Major corridors: `2.4 m`
- Research/office corridors: `1.8 m`
- Maintenance routes: `1.2 m`

These are design targets and must not be used to silently alter the frozen room registry.

## 7. Portal Rules

A portal is a topological connection between two mapped spaces.

Every portal must:
1. connect two spaces that physically meet;
2. have a defined center;
3. have a defined width;
4. have a defined vertical opening range when relevant;
5. respect the floor elevations of both connected spaces;
6. never be created solely to make a graph connected.

Point-touching rooms are not valid connections.

## 8. Vertical Connection Rules

Vertical circulation is represented explicitly by vertical cores.

- VC-01: main stair
- VC-02: service elevator
- VC-03: maintenance ladder shaft

A vertical route must have a continuous physical interpretation. A connection cannot jump between floors without a mapped vertical mechanism.

## 9. Collision/Geometry Rule for Later Production

Visual geometry and collision must share the same canonical spatial reference.

No later implementation may:
- rotate the world to fix an export;
- swap axes per segment;
- offset collision to compensate for bad geometry;
- invent walls that are absent from the map;
- omit mapped walls because implementation is inconvenient.

## 10. Change Control

The coordinate registry is frozen.

If a design problem is discovered:
1. identify the affected design decision;
2. determine whether the problem is architectural or coordinate-related;
3. prefer correcting the design specification;
4. change coordinates only through an explicit coordinate revision;
5. update all dependent documents.

No silent coordinate changes are permitted.

## 11. Authoritative Source Order

1. `design/COORDINATE_REGISTRY.md`
2. `design/DESIGN_LOCK.md`
3. `docs/MASTER_SPEC.md`
4. `docs/DECISIONS.md`
5. supporting design documents

When an older document conflicts with the frozen registry, the registry wins and the older document must be corrected.
