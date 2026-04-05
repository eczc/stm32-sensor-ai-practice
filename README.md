# STM32 传感器 AI 练习项目

> 📚 **学习项目** | 练习在 STM32 上部署 TensorFlow Lite Micro 模型

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![STM32](https://img.shields.io/badge/MCU-STM32H7-blue.svg)](https://www.st.com/)
[![Platform](https://img.shields.io/badge/Platform-TFLite%20Micro-green.svg)](https://www.tensorflow.org/lite/microcontrollers)

---

## 📖 项目说明

这是一个**学习练习项目**，用于练习在 STM32 微控制器上部署 AI 模型。

**学习目标**：
- [ ] 掌握 STM32CubeIDE 开发流程
- [ ] 学会传感器数据采集
- [ ] 理解 TFLite 模型训练
- [ ] 掌握模型量化与部署
- [ ] 完成端到端的 AIoT 项目

**⚠️ 注意**: 本项目用于学习目的，代码可能不完善，欢迎交流改进！

---

## 🎯 当前进度

| 阶段 | 任务 | 状态 |
|------|------|------|
| 1 | 环境搭建 + Hello World | ⬜ 未开始 |
| 2 | 传感器数据采集 | ⬜ 未开始 |
| 3 | Python 模型训练 | ⬜ 未开始 |
| 4 | 模型转换与量化 | ⬜ 未开始 |
| 5 | STM32 部署 | ⬜ 未开始 |
| 6 | 实测与优化 | ⬜ 未开始 |

---

## 🛠️ 硬件平台

| 组件 | 型号 | 备注 |
|------|------|------|
| **MCU** | STM32H750XBH6 | 480MHz Cortex-M7, 1MB SRAM |
| **传感器** | 待定 | 加速度计/温度等 |
| **开发工具** | STM32CubeIDE 1.18.1 | ST 官方 IDE |
| **AI 框架** | X-CUBE-AI | ST AI 扩展包 |

---

## 📂 项目结构

```
stm32-sensor-ai-practice/
├── README.md              # 本文件
├── LICENSE                # MIT 许可证
├── docs/                  # 文档
│   ├── learning-log.md    # 学习日志
│   └── notes/             # 技术笔记
├── hardware/              # 硬件相关
│   ├── schematics/        # 原理图
│   └── pcb/               # PCB 文件
├── firmware/              # 固件代码
│   ├── Core/              # 核心代码
│   ├── Drivers/           # 驱动
│   └── AI/                # AI 模型相关
├── python/                # Python 训练脚本
│   ├── data_gen.py        # 数据生成
│   ├── train.py           # 模型训练
│   └── convert.py         # 模型转换
└── resources/             # 参考资料
```

---

## 📅 学习计划

### 第 1 周：环境准备
- [ ] STM32CubeIDE 配置
- [ ] 点灯测试
- [ ] 串口打印

### 第 2 周：传感器数据采集
- [ ] 连接传感器
- [ ] 读取数据
- [ ] 串口输出

### 第 3 周：Python 模型训练
- [ ] 生成模拟数据
- [ ] 训练 CNN 模型
- [ ] 保存模型

### 第 4 周：部署到 STM32
- [ ] 模型转换
- [ ] X-CUBE-AI 配置
- [ ] 实测推理

---

## 📝 学习日志

详细学习过程记录在：[docs/learning-log.md](docs/learning-log.md)

**最近更新时间**: 2026-04-05

---

## 🔧 快速开始

### 环境要求

- STM32CubeIDE 1.18.1+
- Python 3.8+
- TensorFlow 2.x

### 克隆项目

```bash
git clone https://github.com/eczc/stm32-sensor-ai-practice.git
cd stm32-sensor-ai-practice
```

### 运行 Python 训练

```bash
cd python
pip install -r requirements.txt
python train.py
```

---

## 📚 学习资源

### 官方文档
- [STM32CubeMX 用户手册](https://www.st.com/)
- [X-CUBE-AI 文档](https://www.st.com/en/embedded-software/x-cube-ai.html)
- [TFLite Micro 指南](https://www.tensorflow.org/lite/microcontrollers)

### 教程推荐
- [STM32H7 入门教程](https://www.bilibili.com/)
- [TensorFlow 官方教程](https://www.tensorflow.org/tutorials)

---

## 🤝 欢迎交流

**问题讨论**: 欢迎提 Issue  
**代码改进**: 欢迎提 PR  
**学习交流**: 邮件或私信

---

## 📄 许可证

本项目采用 [MIT License](LICENSE)

简单说：
- ✅ 你可以随便用（学习、商用都可以）
- ✅ 只需保留版权声明
- ❌ 不提供任何担保

---

## 📊 项目统计

![GitHub commits](https://img.shields.io/github/commits-since/eczc/stm32-sensor-ai-practice/initial?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/eczc/stm32-sensor-ai-practice/main?style=flat-square)

---

_最后更新：2026-04-05_  
_维护者：JeromeC (eczc)_

---

> 💡 **备注**: 这是一个学习项目，代码可能不完善。如果你发现错误或更好的实现方式，欢迎提 Issue 或 PR！
