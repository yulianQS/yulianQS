<p align="center">
  <strong>English</strong> · <a href="https://github.com/yulianQS/yulianQS/blob/main/README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  <img src="assets/hero.svg" width="100%" alt="yulianQS — Robotics, Embedded Linux, Computer Vision" />
</p>

# Embedded Linux & Robotics Software Developer

Robotics · Embedded Linux · Computer Vision

## About Me

I work across embedded software, robot control, and vision applications, with an interest in connecting perception to motion on real hardware.

- **Autonomous navigation:** mapping, localization, navigation, and mobile robot control.
- **UAV integration:** flight controller communication, companion computers, and vision-based positioning.
- **Embedded Linux:** board deployment, cross-compilation, and hardware–software integration.
- **Edge vision:** model conversion, on-device inference, and visual feedback for motion control.

## Tech Stack

| Area | Technologies used in my projects and engineering work |
| :--- | :--- |
| **Embedded Systems** | C / C++, STM32, ESP32, FreeRTOS · UART, SPI, I²C, PWM |
| **Embedded Linux** | RK3588, RK3506 · Ubuntu, Buildroot, BusyBox, Shell, cross-compilation |
| **Robotics** | ROS 2 Humble, TF, odometry · Cartographer, Nav2, MPPI · PX4, MAVLink, Offboard, VIO |
| **Computer Vision** | Python, OpenCV, YOLO · ONNX, RKNN, NPU inference |

## Featured Public Projects

### 01 · [PX4 Companion Control](https://github.com/yulianQS/px4-companion-control)

**Flight controller communication → telemetry → motion task coordination**

A companion-computer project for MAVLink communication, Offboard integration, and a web control interface. The code includes relative motion tasks, feedback handling, timeouts, and cancellation.

`Python` `PX4` `MAVLink` `Offboard`

> **Status:** Bench integration is documented. Takeoff, hover, translation, and landing behavior still require flight validation.

### 02 · [QSflow](https://github.com/yulianQS/QSflow)

**Images → assisted annotation → review → detection datasets**

A local-first desktop application for object detection annotation. It supports Pascal VOC, YOLO Detection, and COCO Detection, with model-assisted labeling, annotation review, and a lightweight training workflow.

`Python` `YOLO` `Computer Vision` `Desktop Tools`

> **Engineering focus:** A shared annotation model connects manual editing, inference, and dataset review.

### 03 · [ArduPilot Flow Analyzer](https://github.com/yulianQS/ardupilot-flow-analyzer)

**MAVLink / DataFlash → synchronized signals → diagnostic evidence**

A Windows diagnostic application for optical flow, range sensing, and flight controller telemetry. It combines local log parsing, linked plots, and evidence-based Loiter checks.

`Python` `PySide6` `MAVLink` `ArduPilot` `DataFlash`

> **Engineering focus:** Read-only flight controller communication, background parsing, and explicit handling of missing or insufficient data.

## Engineering Highlights

- **Autonomous navigation robot:** RK3588 with ROS 2 Humble, Cartographer, and Nav2 MPPI; a layered control architecture connecting navigation to an STM32 chassis controller and ESP32 communication.
- **Vision-guided puzzle assembly:** Python and OpenCV for contour extraction and geometric matching, connected to path planning and motor execution.
- **RK3588 edge inference:** YOLO conversion through PyTorch → ONNX → RKNN, followed by board-side NPU inference.
- **Vision-to-motion integration:** RK3588 target offset extraction connected to STM32 dual-axis gimbal and stepper motor control.
- **RK3506 system development:** Buildroot deployment, watchdog integration, and memory bandwidth testing.

---

[Explore my public repositories →](https://github.com/yulianQS?tab=repositories)
