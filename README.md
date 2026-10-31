# GPS-Denied Indoor SLAM Navigation Quadrotor

## 📌 Project Overview
An autonomous aerial navigation system designed to operate in indoor or signal-blocked environments where GPS telemetry is completely unavailable.

![RViz2 SLAM Visualisation](<RViz2 Quadrotor SLAM Visualisation.png>)

## ⚙️ Key Technical Features
* **Cartographer SLAM:** Utilized 2D LiDAR sensor scans to construct real-time 2D occupancy grid maps and perform localization simultaneously.
* **Sensor Fusion:** Integrated optical flow sensors and IMU telemetry loops via ROS 2 to ensure high positional stability during hover and flight maneuvers.
* **Autonomous Offboard Control:** Developed flight control scripts interfacing with the PX4 autopilot architecture to execute path planning without human remote intervention.

## 🛠️ Tech Stack
* **Algorithms:** Cartographer SLAM
* **Sensors:** 2D LiDAR, Optical Flow, IMU
* **Frameworks:** ROS 2 (RViz2), PX4 Autopilot
* **Embedded Hardware:** STM32-based flight controller
* **Languages:** Python

## 📊 Performance & Results
* **Mapping Accuracy:** Generated high-resolution 2D occupancy grids in enclosed indoor environments using Cartographer LiDAR SLAM.
* **Position Hold:** Maintained low positional drift during autonomous hovering via optical flow and IMU sensor integration.
* **Offboard Execution:** Validated autonomous take-off, altitude hold (1.5m), and setpoint control routines via PX4 offboard messaging.
