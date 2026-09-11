# THE OTHER SIDE — TECHNICAL SPECIFICATION

## 1. Current Status

Architecture and coordinate truth are locked.

Implementation is intentionally not started.

Phase 19 has passed and the implementation gate is open.

## 2. Production Order

1. Mapping
2. Coordinate truth
3. Design Lock
4. Coding specification
5. Blender production
6. Godot integration
7. Validation

## 3. Coordinate Standard

- metric units;
- one logical unit = one metre;
- 3 m structural grid;
- 1 m design snap;
- canonical X/Y/Z system;
- four levels: +1, 0, B-1, B-2.

## 4. Geometry

Later production must preserve:
- room bounds;
- portal topology;
- floor elevations;
- vertical cores;
- corridor dimensions;
- architectural hierarchy.

## 5. Systems

Later technical design must represent:
- access control;
- power dependencies;
- surveillance;
- audio/acoustic relationships;
- lighting;
- save state;
- Mirror observation and behavioural state;
- investigation evidence.

## 6. Save State

A save captures the relevant game state, including Mirror behavioural state.

Reload restores the exact snapshot.

No failed-timeline information leaks across reload.

## 7. Validation

Mandatory validation must include:
- topology;
- coordinate integrity;
- vertical clearance;
- circuit dependencies;
- save-terminal accessibility;
- blind-spot escape continuity.

## 8. Technical Non-Goals

Do not use technical shortcuts to solve design problems.

Implementation must follow the map.
