# 📋 Statement of Work (SOW) & Roadmap

## Phase 1: Locomotion & Validation (Completed - 15%)
- [x] Assemble 3-motor rolling chassis base.
- [x] Flash ESP32 with initial LED blink test to verify GPIO integrity.
- [x] Configure Dabble Bluetooth control for manual movement (Forward, Reverse, Left, Right).
- [x] Design Tinkercad simulation connecting mobile base with ultrasonic sensor and dual-servo sweep assembly.

## Phase 2: Physical Sensor Integration & Sonar Radar (In Progress)
- [ ] Migrate ultrasonic distance sensor and dual servos from Tinkercad simulation onto physical chassis.
- [ ] Code automated pan-sweep obstacle detection loop (Sonar navigation).
- [ ] Implement safety PIR sensor and 5V isolation relay mockup for the IR/UV-C light array.

## Phase 3: Decoupled SLAM & Web Interface (Remaining)
- [ ] Integrate laboratory 2D LiDAR module with ESP32.
- [ ] Establish ESPAsyncWebServer / WebSockets pipeline to stream raw point-cloud data to laptop.
- [ ] Run spatial SLAM mapping on laptop and feed real-time navigation paths back to the rover.