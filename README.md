# PUI89 Sentinel — All-Terrain Inspection Robot Dog

[English](README.md) · [ภาษาไทย](README.th.md)


**A supervised four-legged quadruped for exploration, situational awareness and inspection evidence capture.**

[English project page](https://pui89.github.io/sentinel.html) · [ภาษาไทย](https://pui89.github.io/sentinel-th.html) · [PUI89 portfolio](https://pui89.github.io/)

![PUI89 Sentinel quadruped inspection robot concept](docs/images/pui89-sentinel-quadruped-inspection-v3.svg)

*Concept illustration only. It is not evidence of a built, integrated, tested or validated robot.*

## What this product is

PUI89 Sentinel is a **four-legged ground robot** intended for human-supervised inspection in authorised industrial, infrastructure, logistics and selected outdoor environments. Its mission is to help operators observe difficult-to-access areas and collect traceable evidence while the human operator retains authority.

**ผู้ใช้งาน:** เจ้าหน้าที่ตรวจสอบโรงงาน โครงสร้างพื้นฐาน คลังสินค้า และพื้นที่ที่ได้รับอนุญาต  
**ประโยชน์หลัก:** ช่วยสำรวจ สังเกตสภาพแวดล้อม และรวบรวมหลักฐานเพื่อให้เจ้าหน้าที่ตรวจสอบ โดยมีมนุษย์กำกับภารกิจ

## Product-specific functions

- Quadruped mobility and terrain perception are engineering priorities, not validated capabilities.
- Intended inspection evidence may combine authorised camera, audio, map, spatial and other sensor observations.
- Support operator-reviewed inspection notes, anomaly cues and evidence records.
- Treat uncertain, missing, stale or conflicting observations as unknown and request human review.
- Select payloads and sensors only after the first mission, site hazards and operating envelope are defined.

## What is not established or in scope

- No physical prototype, integrated sensor suite, validated gait, terrain traversal, field deployment or all-terrain performance is established.
- “All-terrain” is the product direction, not a guarantee of access to every surface or hazardous area.
- **Narcotics detection, X-ray screening, chemical identification and enforcement are outside current Sentinel scope.** Historical screening material is legacy work, not current product capability.
- RGB, depth or LiDAR observations alone cannot authorise entry into a hazardous atmosphere.

## Current development status

**Specified — quadruped product requirements are documented.** No physical robot or field validation is claimed.

**Next evidence gate:** select one supervised inspection mission; define its site, users, operating envelope, hazards, sensor requirements and measurable acceptance criteria before selecting hardware.

## Product documentation

- [Complete system blueprint](docs/COMPLETE_SYSTEM_BLUEPRINT.md)
- [Validation matrix](docs/VALIDATION_MATRIX.md)
- [Sentinel quadruped concept and scope](docs/PUI89_SENTINEL_ROBOT_CONCEPT.md)
- [All-terrain quadruped requirements](docs/SENTINEL_ALL_TERRAIN_INSPECTION_ROBOT_DOG_REQUIREMENTS_V0.2.md)
- [Lightweight-to-balanced engineering baseline v0.1](docs/SENTINEL_LIGHTWEIGHT_BALANCED_ENGINEERING_BASELINE_V0.1.md)
- [Mass budget & actuator sizing framework v0.1](docs/SENTINEL_MASS_BUDGET_ACTUATOR_SIZING_FRAMEWORK_V0.1.md)
- [Representative warehouse inspection mission v0.1](docs/SENTINEL_REPRESENTATIVE_MISSION_PROFILE_V0.1.md)
- [Joint load case matrix v0.1](docs/SENTINEL_JOINT_LOAD_CASE_MATRIX_V0.1.md)
- [Robot geometry specification v0.1](docs/SENTINEL_ROBOT_GEOMETRY_SPECIFICATION_V0.1.md)
- [Historical scope migration register](docs/SENTINEL_SCOPE_MIGRATION.md)

## Shared PUI89 engineering

Cross-product architecture, evidence contracts, safety, privacy, security, recovery, device interaction and localization requirements are maintained in the [PUI89 Shared AI Core](https://github.com/Pui89/PUI89-Shared-AI-Core). Sentinel-specific mobility, inspection payloads and mission risks remain defined and validated separately.

Current maturity labels follow the [PUI89 Portfolio Alignment Register](https://github.com/Pui89/Pui89.github.io/blob/main/docs/PUI89_PORTFOLIO_ALIGNMENT_REGISTER_2026-11-18.md) and [Evidence-Based Development Maturity Standard](https://github.com/Pui89/Pui89.github.io/blob/main/docs/PUI89_DEVELOPMENT_STAGE_STANDARD.md).

## AI Model & Intelligence profile

**Candidate capability profile:** Object Detection, Image Segmentation, Object Tracking, SLAM, Sensor Fusion and Anomaly Detection for supervised quadruped inspection; Predictive Models for condition/risk trends; VLM/LLM for evidence-linked, human-reviewed inspection summaries. No autonomous gait or actuator authority is implied.

All nine shared capability families and their definitions, evaluation requirements, provenance/uncertainty rules and safety boundaries are maintained in the [PUI89 Shared AI Core Model Intelligence Framework](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/architecture/PUI89_MODEL_INTELLIGENCE_FRAMEWORK_V1.0.md). This product profile is a **candidate engineering allocation**, not evidence of model installation, runtime integration, benchmark results, field validation or certified performance. Select and enable each capability only after product-specific requirements, approved data, compute/energy budgets and verification gates are satisfied.

## Robot Capabilities & Functional Capacity

**Scope boundary:** PUI89 Sentinel is currently defined as a human-supervised, four-legged quadruped for exploration, situational awareness and inspection evidence capture in authorised environments. It is not the historical narcotics/X-ray screening concept; narcotics detection, X-ray screening, chemical identification and enforcement are explicitly outside the current product scope.

### 1. Physical capacity
- Four-legged quadruped ground robot; physical prototype and integrated hardware are not established.
- Define dimensions, complete mass, payload, leg reach, foot geometry, centre of gravity, structural limits and recovery/handling points after the first inspection mission is selected.
- Payload and sensor mounting capacity: **TBD**; no carrying rating is claimed.

### 2. Mobility capacity
- Quadruped locomotion and traversal of selected terrain are engineering objectives, not validated capabilities.
- Define gait modes, speed, slope, step/obstacle height, ground clearance, surface friction, stability margins, endurance and recovery behaviour for the chosen mission.
- Do not interpret “all-terrain” as access to every surface or hazardous area.
- **Validated terrain envelope and mobility performance:** not established.

### 3. Perception capacity
- Candidate perception includes authorised camera, audio, spatial/depth, mapping and selected environmental observations appropriate to the inspection mission.
- Support scene understanding, obstacle/terrain cues, anomaly observations, spatial context and traceable inspection evidence.
- Fuse observations with timestamps, source provenance, sensor-health status, confidence and uncertainty.
- Treat missing, stale, conflicting or out-of-distribution observations as unknown and request operator review.
- RGB, depth or LiDAR observations alone cannot establish that a hazardous atmosphere is safe to enter.
- Detection ranges, coverage, localisation accuracy and environmental limits remain TBD.

### 4. Computing capacity
- Define onboard compute, memory, storage, latency and thermal budgets after mission and sensor selection.
- Prefer local processing for inspection data; document model provenance, version, resource use and failure behaviour.
- **Processor, RAM, storage and measured inference performance:** TBD.

### 5. Power capacity
- Define battery chemistry, usable energy, peak leg-actuator power, mission runtime, charging, thermal limits and safe low-battery recovery.
- **Battery capacity, runtime and charging time:** TBD.

### 6. Communication capacity
- Define operator control/telemetry link, range, latency, local data storage, approved remote access and loss-of-link behaviour for the selected site.
- The robot must enter a mission-appropriate safe state on communication loss; no unapproved cloud or remote access is assumed.
- **Protocols, range and link reliability:** TBD.

### 7. Safety capacity
- Require supervised missions, pre-mission site/hazard review, emergency stop, safe gait/actuator state, fall detection/recovery strategy and manual recovery procedures before field trials.
- Do not enter a hazardous atmosphere based solely on robot perception; require appropriate certified instruments and site procedures.
- No autonomous enforcement, pursuit, confrontation or unsupervised entry into dangerous areas is claimed.

### 8. Maintenance capacity
- Plan inspection and replacement for legs, joints, actuators, feet, fasteners, batteries, connectors and sensor mounts.
- Include actuator diagnostics, joint/IMU calibration, sensor cleaning, mechanical wear checks and traceable maintenance history.
- **Service intervals and validated repair procedures:** TBD.

### 9. Operating limits
- Current status is requirements/specification; no physical prototype, integrated sensor suite, validated gait, terrain traversal or field deployment is established.
- Actual payload, terrain, slope, speed, endurance, weather resistance and sensor performance remain TBD.
- Narcotics detection, X-ray screening, chemical identification and enforcement are outside the current Sentinel scope.

**Capacity evidence status:** Quadruped design direction documented; all physical and operational capacities remain TBD / not validated until supported by test evidence.


## Physical & Multimodal Sensor Privacy

PUI89 adopts the [Physical & Multimodal Sensor Privacy Standard v1.0](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/privacy/PUI89_PHYSICAL_MULTIMODAL_SENSOR_PRIVACY_STANDARD_V1.0.md) as a shared engineering requirement. Every installed inspection camera requires a manual physical cover; every microphone requires a hardware disconnect. Spatial scans, maps and inspection evidence are local by default. Disabling required perception restricts or stops the supervised mission.

**Evidence status:** requirements/specification only. No product-level hardware implementation or verification is claimed by this README section.


## Long-Life Battery & Energy Intelligence

PUI89 adopts the [Long-Life Battery & Energy Intelligence Standard v1.0](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/energy/PUI89_LONG_LIFE_BATTERY_ENERGY_INTELLIGENCE_STANDARD_V1.0.md) as a shared engineering requirement. Prioritise locomotion, perception, mapping, communication and inspection-payload efficiency. Validate mission runtime across terrain and payload, including a safe stop/return reserve.

Battery runtime, chemistry, capacity, cycle life, charging performance and safety compliance remain **TBD until designed and evidenced**. No unverified runtime or battery-life claim is made. The design must include an energy budget, independent BMS protections, thermal/electrical safety, service strategy and representative runtime validation.


## Offline Independence & Connectivity Resilience

**The product must work without the app. Safety must work without connectivity.** Basic supported local operation, local status and safety controls must not require a smartphone, app, Wi-Fi, internet or cloud. The complete printed User Manual and printed Quick Start & Safety Guide are supplied inside the product box in the destination-market language. Both are readable without a smartphone, QR scan, account, app, Wi-Fi or internet. QR and short URL are optional supplements. QR and short URL are optional supplements. On link loss, remote commands are disabled and the product follows its own hazard-based safe state. See the [PUI89 Offline Independence & Connectivity Resilience Standard v1.0](https://github.com/Pui89/Pui89.github.io/blob/main/docs/PUI89_OFFLINE_INDEPENDENCE_CONNECTIVITY_RESILIENCE_STANDARD_V1.0.md) and the [product manual/Remote Companion specification](docs/PRODUCT_MANUAL_AND_REMOTE_COMPANION_STANDARD_V1.md).

**Product-specific offline baseline:** Physical local operator controls, local stop/emergency stop, local status/fault indication and safe shutdown. A supervised inspection task may continue only if the approved mission risk assessment, onboard sensing and local operator control permit it. On remote-link loss, use the validated mission-specific response (controlled stop, hold, or a verified safe-point procedure); do not assume return-to-home is always safe. No unattended hazardous movement or remote safety override.

These are development requirements, not claims of implemented, tested or validated capability.


## Latest engineering progress — 22 November 2026

**Maturity:** Specified — product and engineering requirements are documented. **Evidence status:** PARTIAL. No physical robot or field capability is established.

**Recent verified repository progress:**
- Merged the representative warehouse inspection mission profile (PR #224), defining a concrete first inspection use case.
- Added and linked the Sentinel geometry specification and joint-load-case matrix as engineering inputs.
- A warehouse site-survey and measurement worksheet is proposed in PR #225; it is not treated as completed site evidence while that PR remains unmerged.

**Not established:** a built quadruped, integrated sensor suite, validated gait or terrain traversal, measured durability, actuator performance, or field safety.

**Next evidence gate:** complete a permitted site survey; baseline the inspection route, operating envelope, hazards, sensor needs and measurable acceptance criteria; then close the mass/actuator budget and prepare separately labelled simulation, bench and controlled-prototype protocols.

**Last reviewed:** 22 November 2026. See [representative mission PR #224](https://github.com/Pui89/PUI89-All-Terrain-Inspection-Robot/pull/224) and [site-survey worksheet PR #225](https://github.com/Pui89/PUI89-All-Terrain-Inspection-Robot/pull/225).

## Global manufacturing engineering

The product-specific [PUI89 Global Manufacturing Design Brief v1.0](docs/PUI89_GLOBAL_MANUFACTURING_DESIGN_BRIEF_V1.0.md) defines the preliminary product envelope, candidate material families, component architecture, global human-factors requirements, extreme-environment design strategy, manufacturing transfer package, quality gates and unresolved specifications. It distinguishes proposed targets from tested or verified performance. Candidate materials and component types are not an approved BOM; exact grades, models, dimensions and tolerances remain open until engineering analysis and validation.

## Global engineering and manufacturing control

For international engineering, factory and worker handoff, use the controlled PUI89 documents:
- [PUI89 Global Engineering & Manufacturing Portal](https://pui89.github.io/global-engineering.html)
- [PUI89 Global Manufacturing Handoff System v1.0](https://github.com/Pui89/Pui89.github.io/blob/main/docs/PUI89_GLOBAL_MANUFACTURING_HANDOFF_SYSTEM_V1.0.md)

**Production rule:** Build, buy, substitute, inspect or release only against the exact approved product configuration, revision, drawing, BOM and work instruction. Missing or conflicting values are **STOP — DO NOT GUESS**; raise a Technical Query (TQ). The shared blank manufacturing templates are being reviewed in [PUI89 website PR #639](https://github.com/Pui89/Pui89.github.io/pull/639) and are not yet production authority.

## Future-Ready Technology Policy

This product follows the portfolio-wide [PUI89 Future-Ready Technology Policy v1.0](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/architecture/PUI89_FUTURE_READY_TECHNOLOGY_POLICY_V1.0.md). The policy requires upgradeable interfaces, evidence-based technology selection, provenance/licence review, local-first resource discipline, compatibility testing, safe fallback and controlled release scope. Technology candidates are reviewed monthly and architecture decisions quarterly. This link records policy adoption intent; it does **not** claim that model switching, hardware abstraction, sensor adapters, automated monitoring or product-level validation are already implemented.

## Product-Specific Technology Upgrade Plan

**Gartner 2026 alignment:** Physical AI, hybrid/AI supercomputing, Digital Provenance and AI Security. See the [canonical portfolio policy](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/architecture/PUI89_FUTURE_READY_TECHNOLOGY_POLICY_V1.0.md).

| Upgrade area | Planned sequence (not yet a capability claim) |
|---|---|
| Multimodal perception | Specify sensor contracts, timestamps, calibration and coordinate frames; validate each sensor stream independently before fusion. |
| Sensor fusion | Evaluate RGB/depth/thermal/LiDAR only where justified by mission needs; measure failure/degraded modes and sensor disagreement. |
| Navigation & quadruped robotics | Define autonomy boundaries, localisation/navigation interfaces and safe-stop behaviour; simulate first, then controlled hardware verification. |
| Edge reliability & mission orchestration | Measure compute/power/thermal budgets; define fallback and fault reporting; permit bounded missions only with explicit human authorization and audit. |

**First gate:** verified platform interfaces, sensor provenance/calibration and simulation-to-hardware test plan. **Status:** Planned roadmap only.


## Long-Term Technology Evolution & Anti-Obsolescence Strategy (2027–2030+)

This forward-looking roadmap extends the current P1–P4 development sequence beyond the 2026 trend baseline. It identifies evaluation horizons, not guaranteed future capabilities or fixed adoption dates. Each technology remains conditional on verified user value, provenance and licensing, target-hardware fit, safety, maintainability and reproducible evidence.

| Horizon | Product evolution focus |
|---|---|
| 2027 | Specify sensor/time/coordinate contracts, calibration records, modular perception interfaces, mission boundaries and safe-stop requirements. |
| 2028 | Evaluate sensor fusion and semantic mapping in simulation and controlled trials; add depth, thermal or ranging sensors only when mission evidence supports them. |
| 2029 | Explore adaptive inspection, robust localisation, degraded-mode autonomy and coordinated multi-robot/fleet concepts under explicit human authorization. |
| 2030+ | Support replaceable compute, sensor and navigation modules with regression-tested upgrades, auditable mission records and product-specific safety envelopes. |

**Continuous anti-obsolescence rule:** review technology signals monthly, architecture quarterly and the full roadmap annually; trigger an out-of-cycle review when a critical dependency is unsupported, a security issue emerges, or measured performance/resource limits are breached. Keep a verified baseline, migration and rollback path, compatibility/regression tests and a documented decision for every upgrade. Do not adopt a trend solely because it is new. **Status:** Planned roadmap; no future capability is claimed as implemented or validated.


---

## Academic Research Direction — Q1-Targeted Study (Proposed)

**Research topic:** Uncertainty-Aware Multimodal AI for Quadruped Environmental Inspection  
**Working manuscript title:** *Reliability-Aware Multimodal Perception and Terrain-Condition Assessment for Human-Supervised Quadruped Inspection*

**Status:** Proposed research direction for academic review. Novelty and feasibility require a systematic literature review and a defined inspection mission. No physical robot, sensor integration or field performance is claimed.

### 1. Problem and motivation

A quadruped inspection platform may encounter changing terrain, poor illumination, occlusion, dust, reflective surfaces and unreliable or unavailable sensors. A perception system that produces a confident output despite degraded evidence can mislead an operator. The research will study how sensor reliability, terrain understanding and uncertainty-aware human review can improve inspection evidence quality.

### 2. Research gap to verify

- Whether sensor-quality-aware fusion outperforms fixed fusion when modalities are missing, stale or degraded.
- How uncertainty should affect terrain and inspection-event interpretation.
- How to preserve traceable links between observations, sensor health, location and operator-reviewed findings.
- Whether results generalise across sites and terrain conditions rather than one controlled route.

### 3. Research questions and hypotheses

- **RQ1:** Does reliability-aware multimodal fusion improve terrain-condition and inspection-cue assessment over single-sensor and fixed-fusion baselines?
- **RQ2:** Can modality-quality estimation detect when a sensor should be down-weighted or excluded?
- **RQ3:** Does uncertainty-aware abstention reduce unsupported inspection conclusions?
- **H1:** Quality-aware fusion will improve robustness under controlled sensor degradation compared with fixed fusion.
- **H2:** Explicit unknown/abstention states will reduce overconfident errors under missing or conflicting sensor evidence.

### 4. Proposed hybrid-AI method and workflow

1. Define one authorised, human-supervised inspection mission and its hazard envelope.
2. Collect time-synchronised RGB, depth and/or LiDAR observations; include thermal or other modalities only if available and justified.
3. Run specialist models for terrain segmentation, obstacle detection and selected anomaly cues.
4. Estimate per-modality freshness, calibration, noise and quality.
5. Compare early, late and quality-aware fusion; use a VLM only for evidence-grounded semantic summaries, never as an unverified sensor substitute.
6. Attach location, timestamp, sensor status, model version and uncertainty to each inspection record.
7. Present recommendations to an operator; retain human authority over movement and mission continuation.

### 5. Candidate datasets and data collection

- **Original data is essential:** authorised, synchronised quadruped inspection sequences with terrain labels, sensor-health metadata, robot pose and operator-reviewed inspection events.
- Candidate transferable benchmarks include **RELLIS-3D** for off-road scene understanding, **SemanticKITTI** for LiDAR semantics, **OpenLORIS-Scene** for long-term RGB-D perception and **TartanAir** for simulation-based visual robustness.
- These datasets are not equivalent to a validated quadruped inspection benchmark. Their modality coverage, origin, licence and suitability must be checked before use.
- Use synthetic modality dropout/noise only as a controlled robustness experiment, clearly separated from real field evidence.

### 6. Experimental design

- **Baselines:** RGB-only specialist model; geometry-only baseline where applicable; conventional early/late fusion; proposed quality-aware fusion.
- **E1:** modality ablation and complementary-sensor contribution.
- **E2:** missing, stale, noisy, misaligned and degraded sensor conditions.
- **E3:** terrain classes, slopes, uneven surfaces, shadows, glare and occlusion.
- **E4:** uncertainty calibration, abstention and operator-review workload.
- **E5:** held-out site/route and repeated-session generalisation.
- **E6:** inference latency, memory and power/energy only where measured on declared hardware.

**Primary outcomes:** pre-register terrain/inspection event macro-F1 or event-level recall at a defined false-alarm rate.  
**Secondary outcomes:** localisation error, false-safe/false-hazard rates, calibration, abstention coverage, evidence completeness, latency and resource use.

### 7. Expected scientific contribution

A reproducible inspection-perception benchmark/protocol and a reliability-aware multimodal fusion method that explicitly models sensor quality, uncertainty and human review for quadruped environmental inspection.

### 8. Safety, ethics and publication gates

Sentinel remains a **human-supervised four-legged inspection robot**. Narcotics screening, X-ray screening, chemical identification and enforcement are outside scope. Do not infer that an environment is safe to enter from RGB, depth or LiDAR alone. Require site-specific hazard assessment and appropriate certified instruments where needed. No gait, terrain traversal, physical integration or field performance is claimed until separately tested. Protect site-sensitive data and obtain permissions. Q1 publication is a target, not a guarantee.

## 360° Intelligence

The [360° Intelligence Profile v1.0](docs/PUI89_360_DEGREE_INTELLIGENCE_PROFILE_V1.0.md) defines supervised quadruped surround perception for authorised industrial, infrastructure, logistics and selected outdoor inspection missions. It covers body-frame sectors, leg/foot and payload occlusion, terrain cues, sensor synchronisation, localisation evidence, and human-reviewed inspection records.

**Scope clarification:** Sentinel is the All-Terrain Exploration & Inspection Robot Dog. Narcotics detection, X-ray screening, X-ray/narcotics datasets, related forensic spectra, chemical identification and enforcement are excluded. **Status: Proposed**; no integrated 360° sensor suite or physical field validation is established.

