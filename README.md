# Jzhoou · Zhenyu Zhao

**汕头大学｜嵌入式开发 · 机械结构设计**

面向秋招的项目作品集，求职方向为**嵌入式软件/控制开发、机械结构设计**。我的项目实践涵盖下位机固件、传感器与执行器接入、运动控制，以及 CAD 建模、装配迭代与样机验证。

我希望把程序与实物连接起来：既能围绕传感反馈编写控制逻辑，也能结合安装、布线和维护需求调整结构，并通过实物调试检验方案。

## 能力与项目依据

| 方向 | 项目实践 | 对应项目 |
| --- | --- | --- |
| 嵌入式开发 | C/C++；Arduino、STM32F1、TI MSPM0G3507；外设驱动、定时中断与状态机 | 按摩仪、物流小车、MSPM0 电机控制 |
| 运动控制与通信 | PWM、编码器测速、双电机增量式速度 PI；UART、I²C；步进电机与舵机控制 | MSPM0 电机控制、物流小车、按摩仪 |
| 传感与系统联调 | 压力与阻抗采集、串口协议解析、OpenMV 视觉数据接收与动作协调 | 按摩仪、物流小车 |
| 机械建模与装配 | SolidWorks 零件与装配建模；支撑与安装结构、空间布置及装配干涉调整 | AUV、按摩仪部分机械建模 |
| 样机迭代与验证 | 试装反馈、线束与接口避让、穿线密封整改、气密与分段浅水测试记录 | AUV-CavePI |

## 代表项目

### [CavePI 水下机器人原型](https://github.com/Jzhoou/AUV-CavePI)

**独立项目｜机械结构 · 电气集成 · 样机验证**

围绕亚克力密封舱、推进器和电源布局推进 CAD 设计与实物装配，重点处理有限舱内空间中的固定、布线与维护问题。

- 设计并试装一体抽拉式内部支撑，结合试装结果调整铜柱配合、螺母沉孔、接口避让和内部高度。
- 规划 14.8 V 4S 电源与分电路径，完成穿线封灌、装配及漏点定位，多轮改进线缆周边密封。
- 已记录短时负压气密与头尾分段浅水检查；整机完整浸没、长期水密及水下运动控制仍待验证。

**仓库可查看：** CAD 迭代、实物照片、电源管理与测试日志。

### [淋巴水肿按摩仪工程原型](https://github.com/Jzhoou/Lymphedema-Massager)

**团队项目｜负责下位机电控，参与部分机械建模**

- 实现治疗流程状态机，组织压力与 AD5933 阻抗采集、舵机压力反馈及步进电机动作。
- 完成 BM53 帧协议相关通信、命令处理与状态上报，连接设备控制流程和上位机联调。
- 参与部分机械建模；仓库归档整机、按摩环、舵机按摩头、丝杆及压力传感器等团队模型。

**仓库可查看：** 下位机源码、机械模型与模块说明。WPF 上位机作为团队系统背景展示。该项目为工程原型。

### [智能物流搬运小车](https://github.com/Jzhoou/Smart-logistics-cart)

**团队项目｜负责下位机电控**

- 基于 Arduino 多文件工程编排扫码、取放、分类搬运及返回等阶段任务。
- 接入 HWT101 姿态信息与 OpenMV 视觉结果，协调底盘电机、物料盘和舵机夹爪动作。
- 完成扫码任务解析、串口屏交互及电机驱动协议命令组织。

**仓库可查看：** 控制源码、任务流程与配套机械模型；机械资料作为团队项目背景归档。

### [MSPM0G3507 双电机速度闭环](https://github.com/Jzhoou/Line-following-aiming-car)

**团队项目｜负责 MSPM0 下位机电控**

- 通过正交编码器 GPIO 中断计数和周期采样换算电机转速。
- 为左右电机分别实现增量式速度 PI，结合方向 GPIO、PWM 输出与限幅形成速度控制链路。
- 保留按键、定时器及外设实验工程，便于对照控制代码与 SysConfig 配置。

**仓库可查看：** 电机控制、编码器采样与定时调度源码。

## 其他项目

- [STM32F1 循迹避障小车](https://github.com/Jzhoou/Line-following-obstacle-avoiding-car)：负责下位机固件，包含红外循迹、PWM 电机控制与 USART 外部感知数据接入。
- [智慧草莓种植系统](https://github.com/Jzhoou/Smart-Strawberry-Growing-System)：负责下位机电控，包含环境采集、执行器控制、联网通信与串口 HMI 联调；历史快照的已知问题见仓库说明。

## About me

Student at **Shantou University**, seeking opportunities in **embedded development and mechanical design**. My projects cover C/C++ firmware, motor control, sensor integration, CAD modeling, physical assembly, and prototype testing.

**CavePI** is my independent underwater-robot prototype. In team projects, I developed embedded controllers and also contributed to part of the **Lymphedema-Massager** mechanical modeling. Each repository documents my contribution and the available implementation or test evidence.
