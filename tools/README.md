# THE OTHER SIDE — TOOLS

This directory contains development and validation tooling.

## Current Status

Production tooling is not yet authoritative.

The implementation gate is open, but tools remain subordinate to the canonical design.

## Planned Tools

- coordinate registry validation;
- portal topology validation;
- architectural consistency checks;
- system dependency validation;
- observation-network validation;
- build/export validation;
- regression tests;
- Mirror causality validation;
- escape-route continuity validation.

## Rule

Tools must validate the design.

They must not silently rewrite canonical design decisions.

The coordinate registry remains the source of truth for actual spatial data.

No tool may invent a room, portal, coordinate, Mirror capability or escape mechanic.
