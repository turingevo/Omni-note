[![English](https://img.shields.io/badge/lang-English-blue)](README_en.md) [![中文](https://img.shields.io/badge/语言-中文-red)](README.md) [![Release](https://img.shields.io/github/v/release/turingevo/Omni-note)](https://github.com/turingevo/Omni-note/releases) [![WebSite](https://img.shields.io/badge/官网-turingevo.com-2ea44f)](https://turingevo.com)

# OmniNote — 你的本地 AI 知识大脑

> **多模态笔记 × Graph RAG × 9 种产出引擎 × AGENT 平台**
> 本地版数据不出电脑；云端版填一个 API Key 就能用。

---

## 🎬 视频演示

[![OmniNote 视频演示](bilibili-demo-cover.jpg)](https://www.bilibili.com/video/BV1nUxB65EHS?t=5.2)

📺 **[B 站：免费替代 NotebookLM —— 本地知识库 + 九种 AI 产出](https://www.bilibili.com/video/BV1nUxB65EHS?t=5.2)**

![OmniNote 界面](turingevo.com-OmniNote-1.png)

![OmniNote 知识库](turingevo.com-OmniNote-2.png)

---

## 为什么选择 OmniNote？

| | OmniNote | 传统笔记 | 云端 AI 笔记 |
|---|:---:|:---:|:---:|
| 数据隐私 | ✅ 本地版 100% 本地，数据加密 | ✅ 本地存储 | ❌ 上传云端 |
| 多模态理解 | ✅ 文本/图片/音频/视频 | ❌ 纯文本 | ⚠️ 部分支持 |
| 知识图谱检索 | ✅ Graph RAG 三路融合 | ❌ 无 | ❌ 无 |
| 结构化产出 | ✅ 9 种引擎（报告/导图/PPT…） | ❌ 无 | ⚠️ 有限 |
| AI 智能体 | ✅ MCP / SKILL 无限扩展 | ❌ 无 | ❌ 无 |
| 算力要求 | ✅ CPU 可跑，有显卡自动加速 | ✅ 低 | — |

---

## ✨ 核心能力

### 🧠 Graph RAG 知识库

基于 **BM25 关键词 + 向量语义 + 知识图谱** 三路 RRF 融合检索，配合实体抽取与社区聚类，让笔记不再只是"存"，而是真正"懂"。

- PDF / Word / PPT / Excel / Markdown / 图片 / 音视频自动解析入库
- 自适应分块（parent-child 层级）、多知识库隔离管理
- ReAct Agent 智能编排，自动拆解复杂问题，回答自带出处引用

### 📝 9 种结构化产出引擎

一键将知识库内容转化为生产力交付物：

| 引擎 | 产出 | 引擎 | 产出 |
|------|------|------|------|
| 📊 研究报告 | Markdown 长文 | 🗺️ 思维导图 | Markmap 可视化 |
| 🃏 学习闪卡 | 记忆卡片 | 📋 测验题 | 自测 Quiz |
| 📰 信息图 | 可视化海报 | 📖 Wiki | 知识库页面 |
| 📑 PPT | .pptx 演示文稿 | 🎙️ 音频访谈 | 双人对谈音频 |
| 🎬 讲解视频 | 讲义卡 + 配音 + 字幕 | | |

### 🤖 AGENT 平台

MCP（Model Context Protocol）协议接入天气、搜索、文件处理等第三方工具，技能（SKILL）市场把提示词与工作流打包复用——一个对话框调度一切。

### 🔀 模型自由切换

笔记与模型完全解耦，所有能力统一走 OpenAI 兼容接口：

- **优先推荐：[官方 API](https://api.turingevo.com)** — 填入 API Key 即用，按量计费，无需下载模型、不占显存
- **可选：本地模型** — 任一项能力都可以切到本机推理，完全离线

| 能力 | API 标准 | 本地模型（可选） |
|------|----------|------------------|
| 视觉语言模型 | OpenAI Chat | Qwen3.5-4B |
| 嵌入模型 | OpenAI Embedding | Qwen3-Embedding-0.6B |
| 重排模型 | Rerank | Qwen3-Reranker-0.6B |
| 图像生成 / 信息图 | OpenAI Images | SenseNova-U1.5-8B（8 步出图） |
| 语音识别 | OpenAI Audio | Qwen3-ASR-0.6B |
| 语音合成 | TTS | Qwen3-TTS-1.7B |

### 🧩 模型按需启停

常驻的只有对话、向量、重排三个服务；生图、语音识别、语音合成按产出需求自动启停，显存不够也能跑完整的 9 种产出。

---

## 🛡️ 安全与性能

- **数据私有** — 本地版全部推理在本机完成，无需联网；数据库端到端加密
- **低比特量化** — GGUF Q4_K_M / Q5_K_M / Q8_0 量化，CPU 即可推理，有显卡自动卸载到 GPU
- **灵活部署** — 单机即装即用 / 局域网多人协同 / Docker 容器化

---

## 📦 版本与下载

| 版本 | 安装包 | 说明 |
|------|--------|------|
| **云端版（推荐）** | `omni-note-cloud-linux-x64-v2.1.4.tar.xz` | 只填 API Key，模型调用走云端 |
| **本地版** | `omni-note-local-linux-x64-v2.1.4.tar.xz` | 模型全部跑在本机，可完全离线 |
| **Docker / 服务器** | `omni-note-app_latest.tar.gz` + `instance-init.zip` | 配合 `omniManager-linux-x64.zip` 管理模型 |

> 版本说明见 [Release Notes](https://github.com/turingevo/Omni-note/releases)，历史版本可在 Releases 中下载。

---

## 🚀 快速开始

```bash
# 解压（本地版把 cloud 换成 local）
tar -xf omni-note-cloud-linux-x64-v2.1.4.tar.xz
cd OmniNote-cloud-linux-x64

# 启动主程序
chmod a+x ./OmniNote && ./OmniNote

# 浏览器打开 http://localhost:7000
```

- **云端版**：启动后登录 turingevo 账号，在「设置 → 模型服务」填入 API Key 即可使用（[获取入口](https://api.turingevo.com/pricing)）
- **本地版**：用随包的 `omniManager` 下载模型与推理工具，再按需启动模型服务
- **Docker**：导入镜像，配合 `instance-init.zip` 初始化数据目录即可

---

## 🏆 荣誉

- **Arm 2024 人工智能创新应用大赛优秀奖**
- **Intel 2025 人工智能创新应用大赛优胜奖**
- **联想冠名顶级赞助商特别奖**
- **高通骁龙人工智能大赛优秀奖**

---

## 📚 文档导航

产品文档在线托管在 **[turingevo.com/blog](https://turingevo.com/blog)**，位于左侧「产品文档」分组：

| 文档 | 内容 |
|------|------|
| [Docker 部署](https://turingevo.com/blog) | 镜像、compose、数据包，模型服务跑在宿主机 |
| [准备数据](https://turingevo.com/blog) | Docker 部署所需的 instance 数据（模板/字体/技能） |
| [快速开始 Cloud](https://turingevo.com/blog) | 云端版：注册登录、获取 API Key、配置模型 |
| [快速开始 Local](https://turingevo.com/blog) | 本地版：模型下载、服务启停与编排 |
| [知识库使用指南](https://turingevo.com/blog) | 启动 EBD/RNK、构建与增量同步、文件上传检索 |
| [管理界面使用说明](https://turingevo.com/blog) | omniManager：下载模型、启停服务、MCP 与硬件信息 |

> 博客前端为单页应用，链接统一指向文档首页；打开后在最左侧「产品文档」分组点选对应标题即可。

---

## 🌐 联系我们

| | |
|---|---|
| 🌍 官网 | https://turingevo.com |
| 📝 博客 | https://turingevo.com/blog |
| 🔑 模型 API | https://api.turingevo.com |
| 💻 GitHub | https://github.com/turingevo |
| 🤗 Hugging Face | https://huggingface.co/turingevo |
| 🤖 ModelScope | https://www.modelscope.cn/profile/TuringEvo |
| 💬 QQ 群 | 873673497 |
| 📧 邮箱 | wmx@turingevo.com |
