# THE OTHER SIDE — COORDINATE REGISTRY

**Status:** FROZEN
**Revision:** Mapping/Coordinate Truth Final
**Purpose:** Authoritative spatial truth for Rosslyn

> This file contains actual coordinates. Do not infer replacement coordinates from older design documents.

## 1. World Envelope

`X [-40,40]`
`Y [-30,30]`
Origin `(0,0,0)`

## 2. Core Rooms

### Ground — Level 0

| ID | Space | Sector | Bounds |
|---|---|---|---|
| R-101 | Primary Security Airlock | A | X[-6,6], Y[-30,-24], Z[0,3.2] |
| R-102 | Intake Reception | A | X[-12,12], Y[-24,-12], Z[0,3.2] |
| HUB-00 | Central Circulation Hub | A | X[-12,12], Y[-12,12], Z[0,3.2] |
| R-103 | Admin Records Office | A | X[12,27], Y[-12,12], Z[0,3.2] |

### Basement 1 — Level -1

| ID | Space | Sector | Bounds |
|---|---|---|---|
| HUB-B1 | Lower Circulation Hub | B/C | X[-12,12], Y[-12,12], Z[-4,-0.8] |
| R-201 | Observation Chamber 01 | B | X[-27,-12], Y[12,27], Z[-4,-0.8] |
| R-202 | Behavioral Control Room | B | X[-12,12], Y[12,27], Z[-4,-0.8] |
| R-301 | Diagnostic Terminal Hub | C | X[12,27], Y[-12,12], Z[-4,-0.8] |
| R-302 | Main Server Vault | C | X[12,27], Y[12,27], Z[-4,-0.8] |
| C-202 | Observation Ante-Room | B | X[-27,-12], Y[6,12], Z[-4,-0.8] |
| C-203 | Air-Gapped Crawlspace | B/D interface | X[-36,-27], Y[18,21], Z[-4,-0.8] |

### Basement 2 — Level -2

| ID | Space | Sector | Bounds |
|---|---|---|---|
| R-401 | Central Substation | D | X[-15,15], Y[-18,0], Z[-8,-4.8] |
| R-402 | Old Relay Room | D | X[-30,-15], Y[0,15], Z[-8,-4.8] |
| R-403 | Pre-Digital Escape Vault | D | X[-36,-24], Y[15,27], Z[-8,-4.8] |
| C-403 | B2 Infrastructure Connector | D | X[-30,-15], Y[-3,0], Z[-8,-4.8] |
| C-499 | Boundary Tunnel | D | X[-40,-36], Y[24,27], Z[-8,-4.8] |

### Upper Level +1

| ID | Space | Sector | Bounds |
|---|---|---|---|
| HUB-U1 | Upper Atrium Walkway | A | X[-12,12], Y[-12,12], Z[4,7.2] |
| R-501 | Facility Director's Office | A | X[-27,-12], Y[-3,12], Z[4,7.2] |
| R-502 | Observation Gallery | A/B | X[-27,-12], Y[-24,-3], Z[4,7.2] |
| R-503 | Secure Research Lab Alpha | B | X[15,30], Y[0,21], Z[4,7.2] |
| C-501 | East Executive Corridor | A/B | X[12,15], Y[3,21], Z[4,7.2] |

## 3. Vertical Cores

| ID | Function | Bounds |
|---|---|---|
| VC-01 | Main Stairwell | X[-15,-12], Y[-3,3], Z[-8,7.2] |
| VC-02 | Service Elevator | X[12,15], Y[-3,3], Z[-4,7.2] |
| VC-03 | Maintenance Ladder Shaft | X[-38,-36], Y[18,21], Z[-8,-0.8] |

VC-02 terminates at B-1. It does not directly serve B-2.

VC-03 is air-gapped from the main observation/control network and is a deliberate information boundary.

## 4. Corridor Spine

Primary circulation:

- Major spine: `Y[-12,12]`
- Nominal width: `2.4 m`

Peripheral maintenance/service routes:

- West service route around `X[-39,-36]`
- East service route around `X[36,39]`
- Nominal width: `1.2 m`

## 5. Portals

### Ground

- P-101-102 — center `(0,-24)`
- P-102-HUB00 — center `(0,-12)`
- P-HUB00-103 — center `(12,-6)`
- P-102-104 — center `(-12,-18)`
- P-HUB00-105 — center `(-12,-6)`

### B-1

- P-HUBB1-202 — center `(0,12)`
- P-HUBB1-C202 — center `(-12,9)`
- P-C202-201 — center `(-19.5,12)`
- P-201-C203 — center `(-27,19.5)`
- P-C203-VC03 — center `(-36,19.5)`, Z[-4,-1.6]
- P-HUBB1-301 — center `(12,0)`
- P-301-302 — center `(19.5,12)`
- P-202-302 — center `(12,19.5)`

R-201 ↔ R-202 is sealed.

### B-2

- P-401-C403 — center `(-15,-1.5)`, Z[-8,-5.6]
- P-C403-402 — center `(-22.5,0)`
- P-402-403 — center `(-27,15)`
- P-403-VC03 — center `(-36,19.5)`, Z[-8,-4.8]
- P-403-C499 — center `(-36,25.5)`, Z[-8,-4.8]
- P-C499-EXT — center `(-40,25.5)`, Z[-8,-4.8]

### +1

- P-HUBU1-501 — center `(-12,7.5)`, max width `9 m`, Z[4,6.4]
- P-HUBU1-C501 — center `(12,7.5)`, max width `9 m`, Z[4,6.4]
- P-C501-503 — center `(15,12)`, max width `18 m`, Z[4,6.4]
- P-501-502 — center `(-19.5,-3)`, max width `15 m`, Z[4,6.4]

## 6. Exterior Interfaces

- R-101 opens south through the primary entrance.
- C-499 breaches the west building boundary.
- The final escape exits through `P-C499-EXT`.

The exterior perimeter remains outside the structural envelope and is not represented as additional interior rooms.

## 7. Removed / Optional Spaces

### Permanently removed

`C-201` is not a separate space.

### Sealed

The direct R-201 ↔ R-202 relationship is sealed.

### Optional and unresolved

- C-401 Deep Spine — proposed only
- R-404 Main Cooling Plant — proposed only

Neither is part of the canonical connectivity graph and neither may be added merely to fill unused space.

## 8. Canonical Connectivity

### Ground

`Exterior → R-101 → R-102 → HUB-00 → R-103`

R-102 and HUB-00 provide the principal Ground Floor circulation.

### B-1 west

`HUB-B1 → C-202 → R-201 → C-203 → VC-03`

### B-1 east

`HUB-B1 → R-202 / R-301 → R-302`

### B-2

`VC-01 → R-401 → C-403 → R-402 → R-403 → C-499 → Exterior`

R-403 also connects to VC-03.

### +1

`HUB-U1 → R-501`
`HUB-U1 → C-501 → R-503`
`R-501 ↔ R-502`

## 9. Frozen Safety Rules

- No room may connect only by corner contact.
- No portal may bridge an actual gap.
- No portal may occupy an incompatible floor elevation.
- No route may depend on an absent vertical connection.
- No implementation may invent architecture outside this registry without a documented design revision.
