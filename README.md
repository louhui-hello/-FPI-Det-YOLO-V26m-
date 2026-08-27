# YOLO v26m - FPI-Det 目标检测模型

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

本项目包含一个基于 **YOLO v26m** 架构的目标检测模型权重文件，使用 **FPI-Det** 数据集训练，采用 **FP32** 精度。

## 模型信息

| 属性 | 描述 |
|------|------|
| **模型架构** | YOLO v26m (Medium) |
| **训练数据集** | FPI-Det（自定义目标检测数据集） |
| **权重精度** | FP32 (单精度浮点) |
| **文件格式** | PyTorch (.pt) |
| **文件大小** | 131 MB (压缩后 109 MB) |
| **许可证** | MIT |
| **框架** | Ultralytics YOLO / PyTorch |

## 适用范围

该模型适用于以下场景：

- PC 端目标检测推理
- 边缘计算设备（如香橙派、树莓派 5）推理
- 研究学习与二次开发
- 工业视觉检测原型验证
- **作为教师模型，量化蒸馏后部署到嵌入式设备**

> **注意**：FP32 模型大小为 131 MB，不适合直接在 STM32/ESP32 等资源受限的 MCU 上运行。如需部署到嵌入式设备，请先进行模型量化（FP16 / INT8）或蒸馏。

## 快速开始

### 1. 安装依赖

```bash
pip install torch ultralytics
