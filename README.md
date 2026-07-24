# LLM Fundamentals

**大模型基础学习** — An interactive visualization tool to understand how Large Language Models work under the hood.

## Features

- **Zero dependencies** — Single HTML file, works in any modern browser
- **Real calculations** — All numbers are computed on-the-fly, not hardcoded
- **Chinese-first** — Designed for Chinese learners, demonstrates attention with Chinese sentences

## What's Inside

### Part 1 · Geometry of Parameters
- **Semantic Map**: Meaning is position (2D vector space visualization)
- **Attention Mechanism**: How the model knows what "it" refers to
- **Residual Flow**: Why deep networks can train stably
- **Dense vs MoE**: DeepSeek's Mixture-of-Experts architecture

### Part 2 · Into the Matrix Space
- **BPE Tokenization**: How text becomes tokens
- **QKV Projection**: Step-by-step matrix multiplication
- **Attention Heatmap**: What QKᵀ looks like
- **Multi-Head Split**: How one vector gets split across heads
- **MLP Matrix Flow**: Complete SwiGLU pipeline
- **RoPE Encoding**: How position information "rotates" into vectors

### Part 3 · Training Panorama
- **Four-Stage Timeline**: Pre-training → SFT → RLHF → Inference Optimization
- **KV Cache**: Why generation doesn't get slower over time
- **Learning Rate Schedule**: Warmup + Cosine Decay
- **GQA**: Memory-efficient attention used by Llama/DeepSeek

### Part 4 · Try Your Own Sentence
- Input any Chinese sentence and see attention distribution
- Local heuristic algorithm — no network, no latency

## Quick Start

Open `index.html` in your browser.

Or start a local server:
```bash
python -m http.server 8000
# Then visit http://localhost:8000
```

## Who Is This For

- Beginners who want to understand Transformer internals
- Developers explaining LLM concepts to others
- Anyone preparing for technical interviews

## Technical Details

- Pure frontend: HTML + CSS + JavaScript
- All calculations implemented in vanilla JS, no frameworks
- SVG for vector diagrams and heatmaps

## License

MIT