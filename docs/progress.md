# 📈 Real-Time Development Log

### Sprint 1: Baseline Hardware & Manual Control
- **Done:** Assembled physical base frame with 3 DC motors, castor wheel, and H-bridge.
- **Done:** Completed GPIO LED blink test on ESP32.
- **Done:** Flashed Dabble control firmware for remote driving checks.

### Sprint 2: Simulation & Sonar Sweep Integration
- **Done:** Modeled Tinkercad schematic for ultrasonic distance sensor + dual-servo assembly.
- **Next Step:** Mount ultrasonic sensor and servo motor onto physical chassis frame.
- **Next Step:** Program local sonar obstacle avoidance (turn left/right when path is blocked).

### Sprint 3: Web Dashboard & LiDAR Pipeline
- **Upcoming:** Deploy web dashboard for real-time telemetry display on onboard smartphone.
- **Upcoming:** Connect 2D LiDAR module and stream point-cloud packets over WebSockets to laptop SLAM backend.