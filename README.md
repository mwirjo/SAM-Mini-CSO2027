# SAM-Mini: Autonomous IoT UV-C Disinfection Robot with Wi-Fi Cloud SLAM

SAM-Mini is an autonomous, smart co-bot engineered for automated, chemical-free surface disinfection in laboratory and healthcare environments. 

To achieve maximum performance-to-cost efficiency, heavy spatial computing is offloaded using a **Decoupled SLAM architecture**. An onboard ESP32 microcontroller manages physical locomotion and telemetry, streaming spatial data over Wi-Fi (ESPAsyncWebServer / WebSockets) to a local backend laptop that processes SLAM spatial mapping and returns navigation commands.

---

## 🛠️ Current Project Status (15% Complete)

- **Physical Base:** Assembled 3-DC-motor rolling RC chassis with castor wheel, H-bridge motor driver, and battery pack.
- **Microcontroller Baseline:** ESP32 flashed and tested. Verified core GPIO control via basic LED blink tests and Dabble telemetry (Forward, Backward, Left, Right).
- **Circuit Simulation:** Built and verified a 100% functional Tinkercad circuit simulation integrating the mobile base setup with an ultrasonic distance sensor and dual servo motors for sweeping obstacle detection.

---

## 📂 Repository Structure

```text
SAM-Mini-CSO2027/
├── README.md                 # Main overview & setup guide
├── docs/                     # Comprehensive technical documentation
│   ├── SETUP.md             # Pinout map, wiring, & flashing guide
│   ├── SKILLS.md            # Hardware & software technical competencies
│   ├── SOW.md               # Statement of Work & project timeline
│   ├── ACHIEVEMENTS.md      # Milestones, field test proofs & past rover baselines
│   └── PROGRESS.md          # Real-time build log & sprint tracker
├── hardware/                 # Circuit schematics and CAD design files
│   ├── schematics/          # Tinkercad circuit diagrams & pin layouts
│   └── cad/                 # 3mm laser-cut plywood profiles & 3D print mounts
├── src/                      # Firmware & backend software stack
│   ├── esp32/               # Embedded C++ scripts (Dabble, WebSockets, motor control)
│   └── backend/             # Laptop WebSockets server & telemetry dashboard
├── photos/                   # Close-up hardware photos with descriptive filenames
└── video/                    # Video submission directory & links