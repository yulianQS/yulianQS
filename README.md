<p align="center">
  <strong>English</strong> · <a href="https://github.com/yulianQS/yulianQS/blob/main/README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  <picture>
    <source media="(prefers-reduced-motion: reduce)" srcset="assets/hero.svg" />
    <img src="assets/hero.gif" width="100%" alt="yulianQS — Robotics, Embedded Linux, Computer Vision" />
  </picture>
</p>

# Embedded Linux & Robotics Software Developer

> **“Where there is a will, there is a way.”**
>
> My motto — yulianQS

**From perception to motion — across boards, robots, and edge vision.**

## 01 / About Me

I am **yulianQS**. My engineering work connects embedded firmware, Linux companion computers, robot control, and computer vision. I focus on the software interfaces that turn sensor data into useful feedback and motion on real hardware.

My projects span **mobile robot navigation, UAV companion integration, edge inference, and desktop engineering tools**. I work across board deployment, communication, task coordination, and diagnostics, with particular attention to how the modules behave together.

- **Autonomous navigation:** mapping, localization, navigation, and mobile robot control.
- **UAV integration:** flight controller communication, companion computers, and vision-based positioning.
- **Embedded Linux:** board deployment, cross-compilation, and hardware–software integration.
- **Edge vision:** model conversion, on-device inference, and visual feedback for motion control.

## 02 / Tech Stack

<p align="center">
  <img src="assets/stack-embedded.svg" width="420" alt="Embedded Systems: C/C++, STM32, ESP32, FreeRTOS" />
  <img src="assets/stack-linux.svg" width="420" alt="Embedded Linux: RK3588, RK3506, Ubuntu, Buildroot" />
  <img src="assets/stack-robotics.svg" width="420" alt="Robotics: ROS 2, Cartographer, Nav2, PX4, VIO" />
  <img src="assets/stack-vision.svg" width="420" alt="Computer Vision: OpenCV, YOLO, ONNX, RKNN" />
</p>

### Embedded firmware & peripheral integration

- **Languages and platforms:** C / C++, STM32, ESP32, HAL / CubeMX, and FreeRTOS for embedded firmware work; Python for host-side integration and tooling.
- **Interfaces and peripherals:** GPIO, timers, PWM, ADC / DMA, UART, SPI, and I²C for sensing, communication, and actuator interfacing; MQTT for message exchange in connected systems.
- **Engineering applications:** MCU-side chassis and motor execution, status feedback, and communication between Linux-level task logic and embedded controllers.

### Embedded Linux & board-side deployment

- **Platforms and systems:** RK3588 and RK3506, Ubuntu, Buildroot, BusyBox, Shell, and cross-compilation.
- **Deployment and integration:** board-side application setup, remote deployment, V4L2 camera access, device-node checks, and peripheral integration.
- **System work:** watchdog integration and memory bandwidth testing on RK3506; connecting Linux applications to MCU controllers and board-side vision runtimes.

### ROS 2 & autonomous mobile robots

- **Middleware and navigation:** ROS 2 Humble, node communication, TF coordinate transforms, odometry, Cartographer, and Nav2.
- **Navigation integration:** laser mapping, localization, navigation task configuration, and MPPI controller integration for a mecanum-wheel mobile robot.
- **Control architecture:** RK3588 for upper-level computation, STM32 for chassis execution, and ESP32 communication, with motion commands and state feedback across the layers.

### UAV flight controller & companion integration

- **Communication and control:** PX4, MAVLink, Offboard control, serial communication, telemetry, command acknowledgements, and heartbeat-based state tracking.
- **Task coordination:** relative motion tasks, feedback handling, timeouts, cancellation, and web interfaces for control and observation.
- **Positioning integration:** experience connecting VIO pose information and vision task interfaces with companion-computer task logic. The public PX4 repository documents bench integration; actual flight behavior remains under validation.

### Computer vision & edge model deployment

- **Classical vision:** Python and OpenCV for contour extraction, geometric matching, target offset extraction, and the connection from visual results to path planning and motor execution.
- **Detection and deployment:** YOLO workflows and PyTorch → ONNX → RKNN conversion for board-side RK3588 NPU inference.
- **Dataset tooling:** model-assisted annotation, manual review, lightweight training workflows, and Pascal VOC / YOLO Detection / COCO Detection support in QSflow.

### Desktop tools & engineering diagnostics

- **Application development:** Python and PySide6 for telemetry views, interactive plots, diagnostic interfaces, and engineering workflows.
- **Data and responsiveness:** MAVLink telemetry and DataFlash parsing, linked time-series plots, background workers, and explicit handling of missing or insufficient data.
- **Verification and traceability:** Git-based development, project tests, diagnostic reports, and a clear distinction between offline checks, bench integration, and physical validation.

## 03 / Engineering Capabilities

- **Connect hardware to application logic.** Work across sensors and cameras, Linux computation, MCU or flight controller communication, and actuator-facing command interfaces.
- **Coordinate perception, planning, and execution.** Integrate vision or pose results with navigation tasks, motion commands, and state feedback, while keeping module responsibilities clear.
- **Make system behavior observable.** Build telemetry views and diagnostic tools that expose actual messages, time-aligned signals, task states, and data gaps.
- **Carry software onto the target platform.** Connect model conversion and application development to board deployment, runtime integration, and hardware communication checks.

## 04 / Featured Public Projects

<p align="center">
  <a href="https://github.com/yulianQS/px4-companion-control"><img src="assets/project-px4.svg" width="270" alt="PX4 Companion Control — open public repository" /></a>
  <a href="https://github.com/yulianQS/QSflow"><img src="assets/project-qsflow.svg" width="270" alt="QSflow — open public repository" /></a>
  <a href="https://github.com/yulianQS/ardupilot-flow-analyzer"><img src="assets/project-ardupilot.svg" width="270" alt="ArduPilot Flow Analyzer — open public repository" /></a>
</p>

> **PX4 validation:** Bench integration is documented; actual flight behavior remains under validation.

<details>
<summary>Read project details and validation notes</summary>

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

</details>

## 05 / Selected Engineering Work

### Autonomous navigation robot

Layered RK3588 / STM32 / ESP32 integration for a mecanum-wheel robot. The work connects ROS 2 communication, TF and odometry, Cartographer mapping, and Nav2 MPPI navigation to chassis commands and status feedback.

### Vision-guided puzzle assembly

A Python / OpenCV workflow connecting fragment contour extraction and geometric matching to assembly path planning and motor execution. The focus is the full interface from image interpretation to physical movement.

### RK3588 edge inference & dual-axis gimbal

Board-side YOLO deployment through PyTorch → ONNX → RKNN, alongside vision-to-motion work that extracts target offsets on RK3588 and connects them to STM32-controlled dual-axis gimbal and stepper motor execution.

### RK3506 Buildroot development

Board-side system and application deployment with Buildroot / BusyBox, including watchdog integration and memory bandwidth testing.

---

[Explore my public repositories →](https://github.com/yulianQS?tab=repositories)
