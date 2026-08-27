# YOLO v26m - FPI-Det 目标检测模型

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub release](https://img.shields.io/github/v/release/louhui-hello/-FPI-Det-YOLO-V26m-)](https://github.com/louhui-hello/-FPI-Det-YOLO-V26m-/releases)

本项目包含基于 **YOLO v26m** 架构的目标检测模型权重，使用 **FPI-Det** 数据集训练，采用 **FP32** 精度。

---

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

---

## 适用范围

| 场景 | 是否适用 | 说明 |
|------|----------|------|
| PC 端推理 | ✅ | 原生支持，性能最佳 |
| 边缘设备（香橙派、树莓派5） | ✅ | 可运行，建议使用 FP16 或 INT8 量化版 |
| 嵌入式 MCU（STM32、ESP32） | ❌ | 模型过大，需量化蒸馏后部署 |
| 教师模型（蒸馏/量化） | ✅ | 可作为教师模型训练轻量化学生模型 |
| 研究与学习 | ✅ | 完全开源，适合学习 YOLO 架构 |

> **注意**：FP32 模型大小为 131 MB，不适合直接在 STM32/ESP32 等资源受限的 MCU 上运行。如需部署到嵌入式设备，请先进行模型量化或蒸馏。

---

## 快速开始

### 环境准备

```bash
pip install -r requirements.txt
