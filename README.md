International-Rover-Challenge-2026

A modular six-wheeled autonomous rover developed for International Rover Challenge 2026. The system was designed to perform multiple competition missions including soil analysis, autonomous navigation, and robotic arm operations.The Intel NUC served as the primary computational unit, running ROS2 for system coordination. Multiple embedded subsystems including drive, arm, sensing, and communication were integrated for reliable field performance.

System Architecture:
1. Processing Unit:
   Intel NUC (Main onboard computer),
   ROS2-based software architecture and
   ESP32 modules interfaced with NUC
2. Drive System (6-Wheel Configuration):
   6-wheel differential drive mechanism
   3 Dual-Channel Cytron motor drivers
   Powered via dedicated PCB-based power distribution
   Motor drivers connected through custom PCB routing
3. Robotic Arm (6 DOF):
   6 Degree-of-Freedom robotic arm
   Single-channel motor driver configuration
   Independent PCB for arm power management
   Camera mounted for gripper-level visibility
4. Sensing & Navigation:
   GPS module for global positioning
   BNO085 IMU for orientation and directional feedback
   LiDAR for spatial orientation and obstacle mapping
   Labart 7-in-1 environmental sensor
   MQ135 gas sensor
   BME280 environmental sensor
5. Vision System:
   Top-mounted camera for wide-angle monitoring
   Front camera integrated with LiDAR for navigation
   Arm-mounted camera for precision manipulation tasks
6. Communication System:
   Antenna-based long-range communication
   Signal conversion interface connected to Intel NUC
   Real-time telemetry exchange between rover and base station

Competition Missions:
1. ABEX Mission
   Soil excavation using auger mechanism:
   Labart sensor integrated for in-soil environmental measurement and chemical parameter analysis.
2. RADO Mission
   Autonomous navigation toward target using GPS, BNO085, and camera-based localization.
3. IDMO Mission
   Robotic arm used to complete task-specific manipulation objectives.

My Contribution (Hardware-Focused):
I contributed to the hardware integration of the rover’s drive and manipulation subsystems, assisting in the interfacing of Cytron motor drivers for the 6-wheel drive mechanism and supporting PCB-based power distribution for both the drive and 6-DOF arm systems. I was involved in wiring and integrating environmental sensing modules, ensuring stable connections and reliable operation. Additionally, I participated in mechanical assembly, subsystem integration, and field-level debugging to improve overall system stability and performance during testing.

Technical Challenges:
  Stable power distribution across multiple PCBs
  Managing signal integrity between sensors and Intel NUC
  Mechanical stability of arm during dynamic movement
  Field troubleshooting under time constraints
