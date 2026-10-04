![MirageTransit — One fleet. One truth. Reproducible traces.](../assets/miragetransit.svg)

# MirageTransit

[← Back to profile](../README.md)

A transport security research lab built around one deterministic fleet state and verifiable command/event replay.

**Status:** 0.1.0.dev2 · deterministic core and replay delivered.  
**Stack:** Python · SQLite · uv · Typed contracts.  
**Source:** [Public repository](https://github.com/zCooperHD/MirageTransit).

## The engineering problem

A transport security lab becomes inconsistent when every protocol surface invents its own fleet state. A single deterministic coordinator can make command effects and replayed evidence reproducible before protocol decoys are added.

## Implemented

- Fixed-step synthetic fleet core with bounded vehicle dynamics and typed contracts.
- SQLite event/snapshot journal, restart recovery and transactional command handling.
- Command deduplication, explicit rejection receipts and bounded scenario work.
- Provenance-bound export/import and replay verification at every tick.
- Packaged CLI and a committed synthetic demonstration scenario.

## Verification

The Sprint 2 report records 59 tests and 20 matching 600-tick replays. CI passes lint, strict typing, lock provenance, test execution, packaging and installed-wheel checks.

See the [reviewer guide](https://github.com/zCooperHD/MirageTransit/blob/main/docs/PORTFOLIO.md) and [CI](https://github.com/zCooperHD/MirageTransit/actions) to inspect the public evidence.

## What remains

HTTP/MQTT decoys, analyst console, CAN adapters and contained deployment remain later milestones.

Portfolio checkpoint: **5 October 2026**. The project is presented at its actual delivery stage, with later capabilities left as explicit next steps.
