## 2026-04-05 (Day 1)

### 完成内容
- [x] Python 环境配置 (conda + TensorFlow 2.21.0)
- [x] 数据生成脚本
- [x] 模型训练脚本
- [ ] 模型训练运行
- [ ] 学习日志

### 学到的东西
- TensorFlow 2.21.0 支持 Python 3.10
- 使用 conda 管理环境很方便
- 1D CNN 适合处理时间序列数据

### 下一步
- 转换 TFLite 格式
- 学习 X-CUBE-AI 部署流程

### 心情：9/10


## 2026-04-05 (Day 1) - Python 模型训练

### 完成内容
- [x] Python 环境配置 (conda + TensorFlow 2.21.0)
- [x] 数据生成脚本 (01_data_gen.py)
- [x] 模型训练脚本 (02_train_model.py)
- [x] 模型训练运行 - **准确率 100%!**
- [x] 模型保存 (0.74 MB)
- [ ] TFLite 转换
- [x] 学习日志

### 遇到的问题
1. Python 3.13 版本太高，TensorFlow 不支持
   - 解决：用 conda 创建 Python 3.10 环境

2. ProgbarLogger 参数错误
   - 解决：移除这个回调函数

### 学到的东西
- TensorFlow 2.21.0 支持 Python 3.10
- 1D CNN 适合处理时间序列数据
- EarlyStopping 防止过拟合
- 模拟数据可以快速验证模型

### 模型结构



Conv1D (32) → BN → Conv1D (32) → BN → MaxPool → Dropout
→ Conv1D (64) → BN → Conv1D (64) → BN → MaxPool → Dropout
→ Conv1D (128) → BN → GlobalAvgPool
→ Dense (64) → Dropout → Dense (2)

Copy
总参数：56,354 (220 KB)

### 下一步
- [ ] 转换 TFLite 格式
- [ ] 学习 X-CUBE-AI 部署流程
- [ ] 拿到开发板后实测

### 心情：10/10 🎉



## 2026-04-05 (Day 1) - 完整总结

### 完成内容
- [x] Python 环境配置
- [x] 数据生成 (3000 样本)
- [x] 模型训练 (100% 准确率)
- [x] TFLite 转换 (78.51 KB)
- [x] 项目框架创建

### 关键数据
- 模型输入：(100, 3) - 100 点序列 × 三轴
- 模型输出：(2) - 正常/故障分类
- 模型大小：78.51 KB (TFLite)
- 准确率：100%

### 学到的东西
1. TFLite 压缩率很高 (90%+)
2. 78KB 模型适合 STM32H7
3. 模拟数据可以快速验证流程

### 下一步
- 拿到开发板
- 配置 STM32CubeMX
- 部署 TFLite 模型
- 实测传感器

### 心情：10/10 🎉
