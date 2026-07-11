
[![English](https://img.shields.io/badge/lang-English-blue)](README.md)
[![中文](https://img.shields.io/badge/语言-中文-red)](README_zh.md)

# OmniNote — Your Local AI Knowledge Brain

> **Multimodal Notes × Graph RAG × 9 Output Engines × MCP Agents**
> 100% local deployment. Your data never leaves your machine.

---

## Why OmniNote?

| | OmniNote | Traditional Notes | Cloud AI Notes |
|---|:---:|:---:|:---:|
| Data Privacy | ✅ 100% local, E2E encrypted | ✅ Local storage | ❌ Uploaded to cloud |
| Multimodal | ✅ Text / Image / Audio / Video | ❌ Text only | ⚠️ Partial |
| Knowledge Graph | ✅ Graph RAG triple fusion | ❌ None | ❌ None |
| Structured Output | ✅ 9 engines (reports, mindmaps, PPT…) | ❌ None | ⚠️ Limited |
| AI Agents | ✅ MCP protocol, infinite extensions | ❌ None | ❌ None |
| Hardware | ✅ Runs on CPU-only | ✅ Low | — |

---

## ✨ Core Capabilities

### 🧠 Graph RAG Knowledge Base

Triple-fusion retrieval: **BM25 keywords + Vector embeddings + Knowledge graph**, combined with entity extraction and community clustering. Your notes don't just *store* information — they *understand* it.

- Adaptive chunking (parent-child hierarchy)
- Multi-KB isolation & management
- ReAct Agent for intelligent multi-step reasoning

### 📝 9 Structured Output Engines

Transform knowledge base content into actionable deliverables with one click:

| Engine | Output | Engine | Output |
|--------|--------|--------|--------|
| 📊 Research Report | Markdown long-form | 🗺️ Mind Map | Markmap visualization |
| 🃏 Flashcards | Study cards | 📋 Quiz | Self-assessment |
| 📰 Infographic | Visual poster | 📖 Wiki | Knowledge pages |
| 📑 PPT Outline | .pptx presentation | 🎙️ Podcast | Audio (planned) |
| 🎬 Video | Video (planned) | | |

### 🤖 MCP Agent Platform

Built on the MCP (Model Context Protocol) — connect weather, train tickets, Excel, and any third-party tool through a single conversational interface.

### 🔀 Model-Agnostic Design

Notes are fully decoupled from models. Switch providers with one click:

| Capability | API Standard | Default Model |
|------------|--------------|---------------|
| Vision-Language | OpenAI Chat | Qwen3.5-4B |
| Embedding | OpenAI Embedding | Qwen3-Embedding-0.6B |
| Reranker | Jina Rerank | Qwen3-Reranker-0.6B |
| Image Generation | Stable Diffusion | Tiny-SD |
| Speech Recognition | FunASR | Paraformer-large |

---

## 🛡️ Security & Performance

- **100% Local** — No internet required. SQLCipher end-to-end encryption. Your data stays private.
- **CPU-Only Inference** — Low-bit quantization delivers **50%+ faster inference**. Even old hardware runs AI smoothly.
- **Flexible Deployment** — Single machine / LAN multi-user / Docker containerized.

---

## 🚀 Quick Start

```bash
# Extract
tar -xf omni-note-linux-x64.tar.xz

# Launch
chmod a+x ./OmniNote && ./OmniNote

# Open browser
open http://localhost:7000
```

See [📖 Quick Start Guide](user/user-guide/quick-start.md) for full deployment instructions.

---

## 🏆 Recognitions

- **Arm 2024 AI Innovation Application Contest — Excellence Award**
- **Intel 2025 AI Innovation Application Contest — Winner Award**
- **Lenovo Title Sponsor Special Award**
- **Qualcomm Snapdragon AI Contest — Excellence Award**

---

## 📚 Documentation

### 👤 User Docs ([`user/`](user/))

| Directory | Content |
|-----------|---------|
| [`user/user-guide/`](user/user-guide/) | [Quick Start](user/user-guide/quick-start.md) · [Nginx Deploy](user/user-guide/nginx.md) · [PPT Templates](user/user-guide/ppt-templates.md) |

---

## 🌐 Connect

| | |
|---|---|
| 🌍 Website | https://turingevo.com |
| 📝 Blog | https://turingevo.blog.csdn.net |
| 💻 GitHub | https://github.com/turingevo |
| 🤗 Hugging Face | https://huggingface.co/turingevo |
| 📧 Email | wmx@turingevo.com |
