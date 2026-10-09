# Steer-telem-sym
Fly by write steering simulation
46-48
# The LeFrois C++20 Monorepo: Advanced Systems & Edge Compute

## Executive Summary
The LeFrois Portfolio is a multi-module C++20 ecosystem demonstrating enterprise-grade software architecture and test-driven development (TDD). Orchestrated via a modern CMake build system, this repository powers four distinct consumer and mobility hardware prototypes—autonomous vehicle logic, DSP bone-conduction equalization, acoustic climate control, and computer vision thermodynamics. 

By integrating Google Test (`gtest`) natively, the infrastructure guarantees mathematical precision across complex hardware interfaces, ensuring scalability, memory safety, and rapid iteration across isolated development environments.

## Master Table of Contents

### I. Build Infrastructure & CI/CD
* **Modern CMake Orchestration:** Managing multi-module dependencies and root-level linking.
* **Test-Driven Development (TDD):** Utilizing Google Test for deterministic algorithm validation.
* **Cross-Compilation Strategy:** Building for local terminal simulation vs. Nvidia Jetson / ARM deployment.

### II. Core Libraries & Shared Architecture (The "Brain")
* **Sensor Fusion (`lib_perception`):** mmWave radar and ultrasonic data pipelines.
* **Computer Vision (`lib_cv`):** OpenCV-based material and object recognition.
* **Digital Signal Processing (`lib_dsp`):** Low-latency audio equalization algorithms.
* **State Machine Framework (`lib_fsm`):** Thread-safe state transitions for vehicle and appliance lifecycles.

### III. Module 1: `quintillion_drive` (Autonomous Vehicle Logic)
* **Drive-by-Wire Subsystem:** Electronic shift actuators and Heim-joint suspension compensation.
* **Collision Avoidance Matrix:** Radar threshold triggers and emergency overrides.
* **Series-Hybrid Telemetry:** 2-stroke generator to 72V electric hub hand-offs.

### IV. Module 2: `titanium_dsp` (Biometric Audio Interfaces)
* **Near-Field Magnetic Induction (NFMI):** Low-level communication protocols.
* **Bone-Conduction Equalization:** Titanium acoustic resonance profiles.
* **Power Management:** Inductive charging state triggers.

### V. Module 3: `stealth_climate` (IoT Environmental Control)
* **Acoustic-Dampening Algorithms:** Dynamic compressor load balancing based on ambient room noise.
* **Thermodynamic Loop Control:** Sensor-driven climate adjustments.

### VI. Module 4: `flash_frost_cv` (Targeted Thermal Exchange)
* **Material Identification Logic:** Differentiating glass vs. aluminum using visual markers.
* **Phase-Change Thermal Battery Management:** Ventless heat rejection cycles.
* **Dynamic Cooling Curves:** Real-time chilling adjustments to prevent liquid expansion/freezing.

### VII. Abstraction Strategy & IP Protection
* **Dual-Layer Architecture:** Strict separation of public API contracts/mocked interfaces from private, trade-secret mathematical implementations.
