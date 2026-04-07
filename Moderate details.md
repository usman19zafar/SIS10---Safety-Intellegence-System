SIS-Models
High‑Velocity Data Streams — Element‑by‑Element Breakdown

Kafka SPS What it is:
High‑throughput distributed streaming backbone for ingesting millions of OT/IT events per second.
Utility in SIS‑10:

Provides the real‑time event bus for safety‑critical signals.

Ensures ordered, durable, replayable data for RCA, hazard propagation, and anomaly detection.

Enables parallel analytics pipelines without impacting control systems.

PLC/DCS/SIS Signals What they are:
Raw control‑layer signals from logic solvers, controllers, and safety systems (analog, digital, status, mode, trip, bypass, override).
Utility in SIS‑10:

Forms the ground‑truth operational state of the plant.

Enables detection of faults, overrides, bypasses, degraded SIL, and unsafe states.

Feeds the Mosaic engine for hazard propagation modeling.

Allen‑Bradley ControlLogix / CompactLogix Tags What they are:
Rockwell Automation controller tags representing real‑time process values, states, alarms, and interlocks.
Utility in SIS‑10:

Provides high‑resolution, deterministic data from widely deployed North American PLCs.

Enables SIS‑10 to detect logic‑level anomalies, scan‑time drift, and unsafe interlock behavior.

Bridges Rockwell ecosystems into Kafka + analytics pipelines.

Sensor Telemetry What it is:
Continuous readings from pressure, temperature, flow, vibration, level, gas detection, and SIL‑rated sensors.
Utility in SIS‑10:

Detects drift, bias, noise, failure modes, and calibration issues.

Enables predictive hazard detection before PLC logic trips.

Supports SIL verification by tracking sensor reliability and performance.

Network Heartbeats What they are:
Periodic signals confirming network, device, and system health.
Utility in SIS‑10:

Detects latency spikes, packet loss, jitter, and network segmentation failures.

Identifies communication degradation before it becomes a safety event.

Supports time‑sync integrity for event ordering.

Hardware Diagnostics What it is:
Self‑tests, watchdogs, module health, I/O card faults, power supply status, redundancy states.
Utility in SIS‑10:

Identifies latent hardware faults that compromise SIL.

Enables early detection of failing modules before a trip or dangerous failure.

Feeds lifecycle compliance and proof‑test optimization.

Historians (PI / Canary / Aspen) What they are:
Long‑term time‑series storage systems for process and operational data.
Utility in SIS‑10:

Provides historical baselines for ML models (drift, anomaly, degradation).

Enables trend‑based hazard prediction.

Supports post‑incident RCA with high‑resolution replay.

Reuters Feeds What they are:
External market, commodity, geopolitical, and macro‑risk data streams.
Utility in SIS‑10:

Supports risk‑aware operational decisions (e.g., supply shocks, geopolitical instability).

Enables correlation between external events and plant risk posture.

Useful for enterprise‑level safety governance.

OT‑Cyber Signals What they are:
Firewall logs, IDS/IPS alerts, anomaly detection, access logs, endpoint telemetry.
Utility in SIS‑10:

Detects cyber‑physical threats that could compromise safety logic.

Correlates cyber anomalies with process deviations.

Enables SIS‑cyber convergence, a requirement in modern safety standards.
