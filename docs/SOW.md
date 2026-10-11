# 📋 Statement of Work (SOW) & Roadmap

## 🎯 Core Feature Checklist
- [x] **Manual Drive Mobility:** Forward, reverse, left, and right directional control via direct micro-controller input.
- [ ] **Manual LED Control:** On/board physical control of the indicator light via micro-controller GPIO.
- [ ] **Sonar Obstacle Avoidance:** HC-SR04 ultrasonic distance sensor combined with servo sweep to detect and halt near obstacles automatically.
- [ ] **IoT Web Dashboard:** Asynchronous Wi-Fi web server (`ESPAsyncWebServer`) hosted on the ESP32 for remote browser-based control overrides (movement and indicator light).
- [ ] **ROS Serial Bridge:** Communication pipeline to transmit sensor telemetry and receive velocity twist commands from a workstation.
- [ ] **2D LiDAR SLAM Mapping:** Integration of the Slamtec RPLIDAR 2D LiDAR to stream raw point-cloud data and generate real-time indoor maps.

---

## Phase 1: Locomotion & Validation (Completed - 15%)
- [x] Assemble 3-motor rolling chassis base (transitioning to TT motor baseline for initial mobility).
- [x] Flash ESP32 with initial LED blink test to verify GPIO integrity.
- [x] Configure manual movement control (Forward, Reverse, Left, Right) via ESP32.
- [x] Design Tinkercad simulation connecting mobile base with ultrasonic sensor and dual-servo sweep assembly.

## Phase 2: Physical Sensor Integration & Sonar Radar (Current - October Weeks 1–2)
- [ ] **Lab Day 1 (Task Split):** 
  - Mi-ann: Wire standard indicator LED with current-limiting resistor to ESP32 GPIO pin (mockup for disinfection array) and test manual control logic.
  - Chero: Mount and wire HC-SR04 ultrasonic distance sensor and servo mechanism onto physical chassis.
- [ ] **Lab Day 2 (Integration & Testing):** Merge obstacle avoidance distance thresholds with motor-stop routines and run bug-fixing dry runs.

## Phase 3: IoT Connectivity & Web Dashboard (Target: Late October)
- [ ] Reconnect and test ESP32 Wi-Fi asynchronous web server for remote control overrides.
- [ ] Verify remote browser toggling for directional movement and indicator LED states over local network.

## Phase 4: ROS & Serial Communication Bridge (Target: November Week 1)
- [ ] Set up serial communication pipeline between the ESP32 and the workstation.
- [ ] Configure firmware to handle incoming velocity twist commands and parse encoder telemetry.

## Phase 5: LiDAR Integration & SLAM Mapping (Target: November Weeks 2–4)
- [ ] Mount the Slamtec RPLIDAR 2D LiDAR module onto the upper deck of the rover chassis.
- [ ] Stream raw point-cloud data from the sensor to the workstation.
- [ ] Run spatial SLAM mapping algorithms (such as Cartographer) to generate real-time indoor room layouts.

## Phase 6: Final Integration & Competition Pitch (Target: December Finals)
- [ ] Conduct full-system dry runs combining manual dashboard overrides, obstacle avoidance, indicator LED toggles, and SLAM navigation.
- [ ] Finalize repository documentation, budget sheets, and presentation slides for the Caribbean STEM Olympiads.
