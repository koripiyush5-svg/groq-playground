# Groq Playground — Zero-Shot, One-Shot & Fused-Shot Classifier ⚡

An interactive, high-speed LLM playground powered by **Groq LPU™ Inference Engine** that provides real-time detection, benchmarking, and classification of prompting paradigms into **Zero-Shot**, **One-Shot**, and **Fused-Shot** architectures.

![Groq Playground](https://img.shields.io/badge/Groq-LPU™%20Ultra--Fast-F55036?style=for-the-badge&logo=fastapi&logoColor=white)
![Status](https://img.shields.io/badge/Status-Production%20Ready-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

---

## 🚀 Key Features

### 1. 🔑 Native Groq API Integration
- Connects directly to Groq's official API (`https://api.groq.com/openai/v1/chat/completions` & `/models`).
- Secure API key storage in browser memory or local storage.
- Real-time connection tester verifying key validity and model catalog latency.
- Dynamic model selector supporting:
  - `llama-3.3-70b-versatile`
  - `llama-3.1-8b-instant`
  - `deepseek-r1-distill-llama-70b`
  - `mixtral-8x7b-32768`
  - `gemma2-9b-it`
- Built-in **Demo / Simulation Mode** to explore the entire UI and shot classification without needing an API key immediately.

### 2. 🎯 Shot Architecture Classifier
The playground's classification engine analyzes prompt structure, exemplar syntax, delimiters, and context density:
- **0-Shot (Zero-Shot)**: Direct inquiry with zero examples. Relies purely on Groq's pre-trained parametric knowledge.
- **1-Shot (One-Shot)**: Provides exactly 1 demonstration / reference pattern (input $\rightarrow$ output) to steer tone, syntax, or format.
- **Fused-Shot (Multi-Shot / Hybrid)**: Fuses $2+$ demonstrations, chain-of-thought rules, or multi-source context patterns for deep semantic precision.
- **Verdict Card**: Displays classification badge, confidence percentage, detected exemplar counts, and analytical explanation.

### 3. ⚔️ 3-Way Simultaneous Shot Benchmark
- Test the exact same query across **Zero-Shot**, **One-Shot**, and **Fused-Shot** concurrently.
- Side-by-side comparison of outputs, token usage, and latency metrics.

### 4. 🔍 Shot Detective & Auditor
- Dedicated auditor where you can paste any arbitrary prompt, search snippet, or RAG context.
- Deconstructs delimiter patterns (`Q:/A:`, `Input:/Output:`, `->`, few-shot dividers) and highlights structural evidence.

### 5. ⚡ Real-Time Performance Telemetry
- Total generation latency ($\text{ms}$).
- Groq LPU speed ($\text{tok/s}$).
- Token breakdown (Prompt + Completion).

---

## 🛠️ Tech Stack & Architecture

- **Single-File Architecture**: Self-contained `index.html` with zero build tools or complex dependencies required.
- **Tailwind CSS**: Modern dark developer UI themed with Groq orange (`#F55036`).
- **Marked.js & Highlight.js**: Full Markdown rendering with syntax-highlighted code blocks.
- **Pure Client-Side**: Safe, direct browser-to-Groq requests with CORS compatibility.

---

## 💻 Quick Start

Simply open `index.html` in your web browser:

```bash
# Clone the repository
git clone https://github.com/koripiyush5-svg/groq-playground.git

# Enter the directory
cd groq-playground

# Open in default browser (macOS)
open index.html

# Or on Linux
xdg-open index.html
```

---

## 📄 License

MIT License © 2026 Piyush Kori
