# PUI89 Hybrid End-to-End AI Adapter — PUI89 Sentinel — All-Terrain Inspection Robot

**Status:** Product-specific architecture allocation. This document is not evidence of model deployment, physical integration, field performance or certification.

## Product mission
Quadruped inspection and environmental awareness.

## Approved input boundary
Approved RGB/depth/IMU/other modalities only where present, calibrated and timestamped.

Every input must preserve source, timestamp, modality, coordinate frame/units where relevant, quality, calibration and provenance. Unsupported or unavailable sensors remain out of scope.

## E2E-capable intelligence tasks
Terrain/scene understanding, traversability assessment, obstacle/context prediction and inspection evidence capture.

The product may use modular pipelines, shared representations or joint/E2E models. Selection requires comparative evidence; no monolithic model is mandated.

## Product-specific safety and action boundary
Human-supervised; no validated autonomous traversal, stability, payload, environmental rating or physical inspection capability implied.

The shared model may produce an **ActionProposal** or advisory result only. The product adapter and independent safety/control system enforce permitted actions, preconditions, expiry, safe hold and human authority.

## First research/engineering slice
Begin with offline scene/terrain classification or traversability estimation; compare modular perception with joint context model; physical locomotion remains separately gated.

## Required evaluation
- Task-specific metrics and per-condition breakdowns.
- Confidence calibration, uncertainty and abstention quality.
- Missing, stale, conflicting and corrupted input behaviour.
- Out-of-distribution and domain-shift tests.
- CPU-first runtime, memory and reproducibility; target hardware profiling only when available.
- FailureReport and Evidence Passport for every test run.

## Shared contracts and architecture
Follow [PUI89 Hybrid End-to-End Multimodal AI Architecture v1.0](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/architecture/PUI89_HYBRID_END_TO_END_MULTIMODAL_AI_V1.0.md). The Shared AI Core owns common contracts; this repository owns product-specific requirements, data rights, operating limits and acceptance criteria.

## Evidence status
This is a proposed adapter and test plan. It does not claim datasets, models, sensors, prototypes, product integrations, benchmarks or field tests are complete.
