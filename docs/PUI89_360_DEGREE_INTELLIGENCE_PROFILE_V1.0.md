# PUI89 Sentinel — 360° Intelligence Profile v1.0

**Official identity:** PUI89 Sentinel — All-Terrain Exploration & Inspection Robot  
**Platform:** Human-supervised four-legged quadruped  
**Status:** Proposed product-specific requirements; no integrated 360° sensor suite or physical field validation is established.

## Mission

Provide authorised industrial, infrastructure, logistics and selected outdoor inspection operators with a traceable view of relevant surroundings around a quadruped platform. The system supports situational awareness, inspection evidence capture and human-reviewed anomaly cues. The operator retains mission authority.

## Candidate 360° workflow

1. Define the authorised inspection site, route, terrain envelope, hazards, operator role and mission stop conditions.
2. Define the robot body frame, leg/foot geometry, payload configuration, mounting locations and sensor fields of view.
3. Acquire only approved sensor observations with source ID, timestamp, coordinate frame, calibration revision, health and provenance.
4. Assess terrain, obstacles, traversability cues and inspection targets by sector; keep unseen, occluded, stale or conflicting regions explicitly unknown.
5. Estimate local position, motion and map only when sensor calibration, timing and localisation evidence satisfy the mission's acceptance criteria.
6. Present traceable inspection observations, anomaly cues and bounded recommendations to the operator; no perception output independently authorises hazardous entry or robot motion.

## Candidate AI and sensing

- Object Detection and Image Segmentation for inspection targets, people, obstacles and terrain-relevant objects.
- Object Tracking and multi-view association for continuity across viewpoints, subject to measured identity-switch and occlusion performance.
- SLAM / visual-inertial or LiDAR odometry for localisation and mapping where justified by the selected inspection mission.
- Sensor Fusion and state estimation across approved RGB, depth, LiDAR, IMU, thermal, audio or environmental inputs only after time alignment, calibration and health checks.
- Traversability assessment, foothold/footstep planning and terrain classification as candidate quadruped robotics capabilities; these require separate simulation, bench and controlled hardware validation.
- Anomaly Detection and evidence-linked VLM/LLM summaries for operator review, never as substitutes for certified instruments or safety controls.

Exact sensors, model families, compute hardware and runtime are not selected by this profile. No model or package installation is authorised by this document.

## 360° coverage requirements

- Define horizontal azimuth and vertical elevation coverage around the quadruped body frame, including ground-level foot zones, overhead structures and payload occlusion.
- Model self-occlusion from the torso, legs, head, payload, cable routing and any operator-handling configuration.
- Include near-field blind zones, leg sweep, body pitch/roll, vibration, gait motion, dust, low light, rain and reflective surfaces.
- Distinguish nominal sensor field-of-view from actual visible coverage; do not treat a sensor specification or stitched panorama as proof of perception performance.
- Preserve sensor-specific observations and disagreement; fuse only calibrated, synchronised and frame-compatible inputs.
- Report sensor failures and loss of sector coverage as degraded/unknown states, not as clear space.

## Quadruped safety and human authority

- A 360° perception result is not a permission to enter a hazardous area.
- Do not use RGB, depth, thermal or LiDAR alone to declare an atmosphere safe; use appropriate certified instruments and site procedures.
- Keep an independent emergency stop, actuator limits, watchdogs, communication-loss response, safe-hold and manual recovery strategy outside learned-model authority.
- Gait, foothold planning, locomotion and recovery require separate hazard analysis and staged simulation/bench/controlled-prototype validation.
- No autonomous enforcement, pursuit, confrontation or unsupervised hazardous-area entry is in scope.

## Explicit exclusions

PUI89 Sentinel is the quadruped exploration and inspection robot—not a narcotics-screening product. The following are explicitly outside its current product scope and must not be reintroduced through this 360° work:
- Narcotics detection or screening.
- X-ray screening, X-ray payloads or X-ray datasets.
- Narcotics datasets and associated forensic spectra.
- Chemical identification or enforcement functions associated with the retired screening work.

## Evidence gates

G0 mission and hazard definition → G1 rights-cleared/synthetic data and sector test cases → G2 sensor bench calibration and time synchronisation → G3 quadruped integration, fault injection and safe-state verification → G4 supervised controlled-site inspection with independent review.

Measure azimuth/elevation coverage, near-field blind zones, terrain/obstacle recall by sector, false alerts, track continuity, localisation error, timestamp skew, calibration error, latency, peak RAM, energy, sensor-loss detection and safe-recovery time only after a defined configuration is tested.

**Shared architecture:** [PUI89 360° Intelligence Architecture v1.0](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/PUI89_360_DEGREE_INTELLIGENCE_V1.0.md)

**Evidence boundary:** This profile is a requirements document. It does not establish installed cameras, LiDAR, radar, depth sensors, SLAM, 360° detection, validated gait, all-terrain performance or a built robot.
