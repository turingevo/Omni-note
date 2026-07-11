
[![English](https://img.shields.io/badge/lang-English-blue)](README.md)
[![中文](https://img.shields.io/badge/语言-中文-red)](README_zh.md)

# OmniNote — 你的本地 AI 知识大脑

> **多模态笔记 × Graph RAG × 9 种产出引擎 × MCP 智能体**
> 100% 本地部署，数据不出你的电脑。

---

## 为什么选择 OmniNote？

| | OmniNote | 传统笔记 | 云端 AI 笔记 |
|---|:---:|:---:|:---:|
| 数据隐私 | ✅ 100% 本地，端到端加密 | ✅ 本地存储 | ❌ 上传云端 |
| 多模态理解 | ✅ 文本/图片/音频/视频 | ❌ 纯文本 | ⚠️ 部分支持 |
| 知识图谱检索 | ✅ Graph RAG 三路融合 | ❌ 无 | ❌ 无 |
| 结构化产出 | ✅ 9 种引擎（报告/导图/PPT…） | ❌ 无 | ⚠️ 有限 |
| AI 智能体 | ✅ MCP 协议，无限扩展 | ❌ 无 | ❌ 无 |
| 算力要求 | ✅ 纯 CPU 即可运行 | ✅ 低 | — |

---

## ✨ 核心能力

### 🧠 Graph RAG 知识库

基于 **BM25 关键词 + 向量语义 + 知识图谱** 三路 RRF 融合检索，配合实体抽取与社区聚类，让笔记不再只是"存"，而是真正"懂"。

- 自适应分块（parent-child 层级）
- 多知识库隔离管理
- ReAct Agent 智能编排，自动拆解复杂问题

### 📝 9 种结构化产出引擎

一键将知识库内容转化为生产力交付物：

| 引擎 | 产出 | 引擎 | 产出 |
|------|------|------|------|
| 📊 研究报告 | Markdown 长文 | 🗺️ 思维导图 | Markmap 可视化 |
| 🃏 学习闪卡 | 记忆卡片 | 📋 测验题 | 自测 Quiz |
| 📰 信息图 | 可视化海报 | 📖 Wiki | 知识库页面 |
| 📑 PPT 大纲 | .pptx 演示文稿 | 🎙️ 播客 | 音频（规划中） |
| 🎬 视频 | 视频（规划中） | | |

### 🤖 MCP 智能体平台

基于 MCP（Model Context Protocol）协议的开放架构，接入天气、火车票、Excel 等各类第三方工具，一个对话框调度一切。

### 🔀 模型自由切换

笔记与模型完全解耦，兼容 OpenAI API 格式，一键切换：

| 能力 | API 标准 | 默认模型 |
|------|----------|----------|
| 视觉语言模型 | OpenAI Chat | Qwen3.5-4B |
| 嵌入模型 | OpenAI Embedding | Qwen3-Embedding-0.6B |
| 重排模型 | Jina Rerank | Qwen3-Reranker-0.6B |
| 图像生成 | Stable Diffusion | Tiny-SD |
| 语音识别 | FunASR | Paraformer-large |

---

## 🛡️ 安全与性能

- **100% 本地部署** — 无需联网，数据库端到端 SQLCipher 加密，数据完全私有
- **纯 CPU 推理** — 基于低比特量化技术，推理速度提升 50%+，老旧设备也能跑 AI
- **灵活部署** — 单机即装即用 / 局域网多人协同 / Docker 容器化

---

## 🚀 快速开始

```bash
# 解压
tar -xf omni-note-linux-x64.tar.xz

# 启动主程序
chmod a+x ./OmniNote && ./OmniNote

# 浏览器访问
open http://localhost:7000
```

详细部署指南请参阅 [📖 快速上手](user/user-guide/quick-start.md)

---

## 🏆 荣誉

- **Arm 2024 人工智能创新应用大赛优秀奖**
- **Intel 2025 人工智能创新应用大赛优胜奖**
- **联想冠名顶级赞助商特别奖**
- **高通骁龙人工智能大赛优秀奖**

---

## 📚 文档导航

### 👤 用户文档 ([`user/`](user/))

| 目录 | 内容 |
|------|------|
| [`user/user-guide/`](user/user-guide/) | [快速上手](user/user-guide/quick-start.md) · [Nginx 部署](user/user-guide/nginx.md) · [PPT 模板](user/user-guide/ppt-templates.md) |
| [`user/deploy/`](user/deploy/) | [Docker 构建](user/deploy/Docker-build.md) · [Docker 部署](user/deploy/Docker-deploy.md) |
| [`user/admin/`](user/admin/) | [备份恢复](user/admin/backup.md) · [数据库](user/admin/database.md) · [许可证](user/admin/license.md) · [图片清理](user/admin/clean-images.md) |

### 🔧 开发文档 ([`dev/`](dev/))

| 目录 | 内容 |
|------|------|
| [`dev/server/`](dev/server/) | 服务端架构（[RAG](dev/server/rag/) · 产出引擎 · [管理工具](dev/server/manager/)） |
| [`dev/frontend/`](dev/frontend/) | 前端安装与配置 |
| [`dev/model_server/`](dev/model_server/) | 模型推理网关 API |
| [`dev/deploy/`](dev/deploy/) | [PyInstaller 打包](dev/deploy/pack.md) · [跨平台](dev/deploy/cross-platform.md) · [pysqlcipher3 编译](dev/deploy/pysqlcipher3-build.md) |
| [`dev/security/`](dev/security/) | 威胁模型与安全分析 |
| [`dev/ref/`](dev/ref/) | 外部参考与研究 |

### 💼 商业文档 ([`market/`](market/))

| 目录 | 内容 |
|------|------|
| [`market/`](market/) | [定价策略](market/pricing-and-feature-restriction.md) · [商业计划](market/business-plan-2026.md) · [宣传文案](market/advertise.md) |

---

## 🌐 联系我们

| | |
|---|---|
| 🌍 官网 | https://turingevo.com |
| 📝 博客 | https://turingevo.blog.csdn.net |
| 💻 GitHub | https://github.com/turingevo |
| 🤗 Hugging Face | https://huggingface.co/turingevo |
| 📧 邮箱 | wmx@turingevo.com |
