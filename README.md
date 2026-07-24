# LLM Fundamentals · 大模型基础学习

一个交互式的大模型原理学习工具，用真实计算带你理解 Transformer 是怎么"思考"的。

**🌐 在线体验：[https://ydsgangge-ux.github.io/llm-fundamentals/](https://ydsgangge-ux.github.io/llm-fundamentals/)**

## ✨ 特点

- **零依赖**：单个 HTML 文件，打开浏览器就能用
- **真实计算**：所有数字都是当场算的，不是假数据
- **中文优先**：专为中文学习者设计，用中文句子演示注意力机制

## 📦 包含内容

### Part 1 · 参数的几何意义
- **语义地图**：意义即位置（2D 向量空间可视化）
- **注意力机制**：模型怎么知道"它"指的是什么
- **残差流**：为什么深层网络能稳定训练
- **Dense vs MoE**：DeepSeek 的专家混合架构

### Part 2 · 钻进矩阵空间
- **BPE 分词**：文本怎么变成 token
- **QKV 投影**：矩阵乘法逐步演示
- **注意力热力图**：QKᵀ 长什么样
- **多头分块**：一个向量怎么被切成多个头
- **MLP 矩阵流**：SwiGLU 完整流程
- **RoPE 旋转编码**：位置信息怎么"转"进向量

### Part 3 · 训练全景
- **四阶段时间线**：预训练 → SFT → RLHF → 推理优化
- **KV Cache**：为什么逐词生成不会越来越慢
- **学习率调度**：Warmup + Cosine Decay
- **GQA**：Llama/DeepSeek 都在用的省显存术

### Part 4 · 试试你的句子
- 输入任意中文句子，看注意力如何分配
- 本地启发式算法，无需联网、无延迟

## 🚀 使用方法

**在线访问**：[https://ydsgangge-ux.github.io/llm-fundamentals/](https://ydsgangge-ux.github.io/llm-fundamentals/)

或本地运行：
```bash
# 克隆仓库
git clone https://github.com/ydsgangge-ux/llm-fundamentals.git

# 打开 index.html 即可
```

## 🎯 适合谁看

- 想理解 Transformer 内部原理的初学者
- 需要向别人讲解大模型的技术人员
- 准备面试、想复习核心概念的开发者

## 📝 技术实现

- 纯前端 HTML + CSS + JavaScript
- 所有计算用原生 JS 实现，无框架依赖
- SVG 绑制向量图和热力图

## 📄 开源协议

MIT