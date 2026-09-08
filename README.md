# Jzhoou

嵌入式系统 · 机器人 · 运动控制

Embedded Systems · Robotics · Motion Control

我关注嵌入式控制系统如何从传感器输入、实时决策走向可靠执行，主要使用 C/C++ 在 Arduino、STM32 与 TI MSPM0 平台上开发机器人下位机。实践内容覆盖电机与舵机驱动、编码器测速、PID 闭环、状态机、UART/I2C 通信，以及 OpenMV 视觉结果与运动控制的协同。

## 技术方向

- **嵌入式开发：** C/C++、Arduino、STM32、TI MSPM0
- **运动控制：** 直流电机与舵机、PWM、编码器测速、PID 闭环控制
- **系统设计：** 治疗/任务状态机、传感器采集、执行器控制、下位机任务流
- **接口与感知：** UART、I2C、OpenMV 视觉结果接收与联动

## 项目

### [AUV-CavePI](https://github.com/Jzhoou/AUV-CavePI)｜独立完成

面向水下机器人原型的机械、电气与密封工程实践。围绕亚克力密封舱、推进器、电源管理与一体抽拉式内部支撑持续完成 CAD 迭代和实物装配，定位并多轮整改穿线螺栓漏点，在当次条件下通过短时气密与分段浅水检查。仓库同时如实记录尚未完成的完整浸没、长期水密和运动控制验证。

### [Lymphedema-Massager](https://github.com/Jzhoou/Lymphedema-Massager)｜团队项目：下位机

仅负责下位机部分：设计治疗流程状态机，完成压力与阻抗数据采集、执行器控制及上下位机通信，使治疗步骤、传感反馈与动作输出在明确的状态转换中协同运行。

### [Smart-logistics-cart](https://github.com/Jzhoou/Smart-logistics-cart)｜团队项目：下位机

仅负责下位机部分：处理姿态信息与视觉结果接收，完成小车运动控制和任务流编排，将感知结果转换为可执行的底盘动作与阶段任务。

### [Line-following-aiming-car](https://github.com/Jzhoou/Line-following-aiming-car)｜团队项目：MSPM0 下位机

仅负责 TI MSPM0 下位机部分：实现编码器采样与 PWM 输出，形成双电机速度闭环控制链路，为循迹和瞄准任务提供底盘控制基础。

## English Summary

I focus on **embedded systems, robotics, and motion control**, building C/C++ firmware on Arduino, STM32, and TI MSPM0 platforms. My work covers motor and servo actuation, encoder-based speed measurement, PID control, state machines, UART/I2C communication, and integration of OpenMV vision results with motion control.

I independently developed **AUV-CavePI**, including mechanical and electrical integration, CAD iteration, enclosure sealing work, and documented testing. I located a leak around the cable-penetration bolts and carried out multiple rounds of rework; under the recorded test conditions, the prototype passed short-duration vacuum and segmented shallow-water checks. In the three team projects above, my scope was limited to the embedded controller: treatment sequencing and sensing for **Lymphedema-Massager**, motion/task control and perception-result handling for **Smart-logistics-cart**, and an MSPM0-based dual-motor speed closed-loop control path for **Line-following-aiming-car**.
