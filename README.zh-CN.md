<p align="center">
  <a href="https://github.com/yulianQS">English</a> · <strong>简体中文</strong>
</p>

<p align="center">
  <picture>
    <source media="(prefers-reduced-motion: reduce)" srcset="assets/hero.svg" />
    <img src="assets/hero.gif" width="100%" alt="yulianQS — 机器人、嵌入式 Linux、计算机视觉" />
  </picture>
</p>

# 嵌入式 Linux 与机器人软件开发者

> **“Where there is a will, there is a way.”**
>
> 我的座右铭：有志者，事竟成。— yulianQS

**从感知到运动，连接嵌入式硬件、机器人与边缘视觉。**

## 01 / 关于我

我是 **yulianQS**。我的工程实践涵盖嵌入式固件、Linux 伴随计算机、机器人控制与计算机视觉，关注如何通过软件接口，将传感器数据连接到可观察的状态反馈与实际运动执行。

项目方向包括**移动机器人自主导航、无人机伴随计算机集成、边缘视觉推理与桌面工程工具**。我的工作涉及板端部署、设备通信、任务协同和诊断分析，尤其关注各模块连接之后的整体行为。

- **自主导航：** 建图、定位、路径导航与移动机器人控制。
- **无人机集成：** 飞控通信、伴随计算机与视觉定位。
- **嵌入式 Linux：** 板端部署、交叉编译与软硬件协同开发。
- **边缘视觉：** 模型转换、端侧推理与运动控制中的视觉反馈。

## 02 / 技术栈

<p align="center">
  <img src="assets/stack-embedded.svg" width="420" alt="Embedded Systems: C/C++, STM32, ESP32, FreeRTOS" />
  <img src="assets/stack-linux.svg" width="420" alt="Embedded Linux: RK3588, RK3506, Ubuntu, Buildroot" />
  <img src="assets/stack-robotics.svg" width="420" alt="Robotics: ROS 2, Cartographer, Nav2, PX4, VIO" />
  <img src="assets/stack-vision.svg" width="420" alt="Computer Vision: OpenCV, YOLO, ONNX, RKNN" />
</p>

### 嵌入式固件与外设集成

- **语言与平台：** 使用 C / C++、STM32、ESP32、HAL / CubeMX 与 FreeRTOS 开展嵌入式固件开发，使用 Python 完成上位机集成与工具开发。
- **接口与外设：** 涉及 GPIO、定时器、PWM、ADC / DMA、UART、SPI、I²C，用于传感采集、设备通信与执行器接口；使用 MQTT 连接系统中的消息交互。
- **工程应用：** 面向 MCU 端底盘与电机执行、状态回传，以及 Linux 上层任务逻辑与嵌入式控制器之间的通信协同。

### 嵌入式 Linux 与板端部署

- **平台与系统：** RK3588、RK3506、Ubuntu、Buildroot、BusyBox、Shell 与交叉编译。
- **部署与集成：** 板端应用配置、远程部署、V4L2 摄像头访问、设备节点检查与外设集成。
- **系统实践：** RK3506 看门狗集成与内存带宽测试；连接 Linux 应用、MCU 控制器和板端视觉推理运行环境。

### ROS 2 与移动机器人自主导航

- **中间件与导航框架：** ROS 2 Humble、节点通信、TF 坐标变换、里程计、Cartographer 与 Nav2。
- **导航集成：** 激光建图、定位、导航任务配置，以及麦克纳姆轮移动机器人的 MPPI 控制器集成。
- **控制架构：** RK3588 承担上层计算，STM32 承担底盘执行，ESP32 参与通信，连接各层之间的运动指令与状态反馈。

### 无人机飞控与伴随计算机集成

- **通信与控制：** PX4、MAVLink、Offboard、串口通信、遥测、指令回执与基于心跳的状态跟踪。
- **任务协同：** 相对运动任务、反馈处理、超时、取消，以及用于控制与观察的网页界面。
- **定位信息集成：** 具有将 VIO 位姿信息、视觉任务接口连接到伴随计算机任务逻辑的实践。公开 PX4 仓库记录了台架集成，实际飞行行为仍需验证。

### 计算机视觉与边缘模型部署

- **传统视觉：** 使用 Python 与 OpenCV 进行轮廓提取、几何匹配、目标偏差提取，并连接视觉结果、路径规划与电机执行流程。
- **检测与部署：** YOLO 工作流，以及 PyTorch → ONNX → RKNN 模型转换，在 RK3588 板端进行 NPU 推理。
- **数据集工具：** QSflow 中的模型辅助标注、人工审阅、轻量训练流程，以及 Pascal VOC / YOLO Detection / COCO Detection 数据格式支持。

### 桌面工具与工程诊断

- **应用开发：** 使用 Python 与 PySide6 构建遥测展示、交互曲线、诊断界面与工程工作流。
- **数据处理与界面响应：** MAVLink 遥测和 DataFlash 日志解析、时间序列联动曲线、后台工作线程，以及对数据缺失和证据不足的明确处理。
- **验证与可追溯性：** Git 版本管理、项目测试与诊断报告，区分离线检查、台架集成与实际硬件验证。

## 03 / 工程能力

- **连接硬件与应用逻辑。** 在传感器、摄像头、Linux 计算、MCU 或飞控通信和执行器指令接口之间完成软件协同。
- **组织感知、规划与执行。** 将视觉或位姿结果连接到导航任务、运动指令与状态反馈，同时明确模块之间的职责。
- **让系统行为可观察。** 构建遥测界面与诊断工具，展示真实消息、时间对齐的信号、任务状态和数据缺口。
- **将软件部署到目标平台。** 将模型转换和应用开发连接到板端部署、运行环境集成与硬件通信检查。

## 04 / 精选公开项目

<p align="center">
  <a href="https://github.com/yulianQS/px4-companion-control"><img src="assets/project-px4.svg" width="270" alt="PX4 Companion Control — open public repository" /></a>
  <a href="https://github.com/yulianQS/QSflow"><img src="assets/project-qsflow.svg" width="270" alt="QSflow — open public repository" /></a>
  <a href="https://github.com/yulianQS/ardupilot-flow-analyzer"><img src="assets/project-ardupilot.svg" width="270" alt="ArduPilot Flow Analyzer — open public repository" /></a>
</p>

> **PX4 验证状态：** 已记录台架集成结果，实际飞行行为仍需验证。

<details>
<summary>展开项目说明与验证状态</summary>

### 01 · [PX4 伴随计算机控制](https://github.com/yulianQS/px4-companion-control)

**飞控通信 → 遥测反馈 → 运动任务协同**

围绕 MAVLink 通信、Offboard 集成与网页控制界面开发的伴随计算机项目。代码包含相对运动任务、反馈处理、超时与取消逻辑。

`Python` `PX4` `MAVLink` `Offboard`

> **当前状态：** 已记录台架集成结果。起飞、悬停、平移与降落行为仍需实际飞行验证。

### 02 · [QSflow](https://github.com/yulianQS/QSflow)

**图像 → 辅助标注 → 审阅 → 检测数据集**

本地优先的目标检测标注桌面应用。支持 Pascal VOC、YOLO Detection 和 COCO Detection，提供模型辅助标注、标注审阅与轻量训练流程。

`Python` `YOLO` `计算机视觉` `桌面工具`

> **工程重点：** 使用统一标注数据模型，连接人工编辑、模型推理与数据集审阅。

### 03 · [ArduPilot 光流分析工具](https://github.com/yulianQS/ardupilot-flow-analyzer)

**MAVLink / DataFlash → 同步信号 → 诊断依据**

面向光流、测距与飞控遥测的 Windows 诊断应用，结合本地日志解析、联动曲线与基于实际数据的 Loiter 筛查。

`Python` `PySide6` `MAVLink` `ArduPilot` `DataFlash`

> **工程重点：** 飞控只读通信、后台解析，以及对数据缺失或证据不足情况的明确处理。

</details>

## 05 / 代表性工程实践

### 自主导航机器人

面向麦克纳姆轮机器人进行 RK3588 / STM32 / ESP32 分层集成，将 ROS 2 通信、TF 与里程计、Cartographer 建图、Nav2 MPPI 导航连接到底盘指令和状态反馈。

### 视觉引导拼图

使用 Python / OpenCV，将碎片轮廓提取、几何匹配连接到拼装路径规划与电机执行，重点打通图像理解到实体运动之间的接口。

### RK3588 边缘推理与双轴云台

通过 PyTorch → ONNX → RKNN 转换部署板端 YOLO 推理；同时开展视觉与运动协同，在 RK3588 上提取目标偏差，并连接 STM32 双轴云台和步进电机执行。

### RK3506 Buildroot 开发

基于 Buildroot / BusyBox 开展板端系统与应用部署，实践内容包括看门狗集成与内存带宽测试。

---

[浏览我的公开仓库 →](https://github.com/yulianQS?tab=repositories)
