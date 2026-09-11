# THE OTHER SIDE — ASSET PIPELINE

**Status:** Pre-production specification
**Implementation:** Not started

## 1. Pipeline

The intended production pipeline is:

**Canonical Mapping → Coordinate Data → Blender Generation → GLB → Godot**

The pipeline must consume the frozen design rather than redefine it.

## 2. Source of Truth

Production geometry must originate from:
- coordinate registry;
- architectural program;
- design lock;
- system state matrix.

## 3. Blender

Blender is a production tool, not a design authority.

Scripts must generate canonical geometry from approved data.

No script may silently invent rooms, move portals, or alter the coordinate system.

## 4. Export

The Blender-to-GLB transformation must be documented exactly once.

No ad-hoc global rotation may be used to repair an export.

## 5. Godot

Godot consumes the approved GLB and approved gameplay/system specifications.

Runtime scripts must not compensate for modelling mistakes with transforms.

## 6. Collision

Collision must correspond to actual mapped physical boundaries.

No collision-only architecture.

No visual wall without intended physical interpretation.

## 7. Validation

Before an environment is accepted:
1. source coordinates are checked;
2. exported geometry is checked;
3. imported Godot geometry is checked;
4. collision is checked;
5. player traversal is checked;
6. portal topology is checked.

## 8. Production Gate

No modelling begins until Design Lock is accepted.
