<div align="center">

# 你好，我是 Charlie 👋

**从桌面运维工程师 → AI 应用开发工程师，正在转行路上**

我原本是一名驻场桌面运维工程师，2026 年开始自学 AI 应用开发。
下面是我的学习轨迹与作品，每一个项目都是真实可用、可在线访问的。

[![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://streamlit.io)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![Qwen](https://img.shields.io/badge/通义千问-Qwen-615EFF?style=flat-square)](https://dashscope.aliyun.com)
[![GitHub](https://img.shields.io/badge/GitHub-licharlie203-181717?style=flat-square&logo=github)](https://github.com/licharlie203)

</div>

---

## 🚀 在线作品（可直接打开体验）

| 项目 | 说明 | 在线地址 |
|------|------|---------|
| **AI 文档问答** | 上传文档，用自然语言提问，答案可溯源（RAG） | [ai-doc-qa.app.workbuddy.host](https://ai-doc-qa.app.workbuddy.host/) |
| **AI 网页助手** | 多轮对话 + 多语言翻译 | [ai-web-assistant.app.workbuddy.host](https://ai-web-assistant.app.workbuddy.host/) |
| **IT 运维故障知识库** | AI Agent 多轮追问式故障排查（HTTP 接口） | [接口文档 /docs](https://it-troubleshooter-79990.app.workbuddy.host/docs) |

---

## 📦 开源项目

<details>
<summary><b>🛠 it-troubleshooter — IT 运维故障知识库（AI Agent）</b></summary>

面向真实运维场景的排查 Agent：把"打印机连不上""域账号登不上"这类模糊描述，
转成一步一步可执行的排查清单，并支持像真人一样**追问补信息**。

- **结构化故障库**：SQLite 存储 20+ 条真实故障案例（症状 / 原因 / 排查步骤 / 分类标签）
- **语义检索**：text-embedding-v3 向量化 + Chroma 检索，按"意思像不像"召回，不是关键词硬匹配
- **Function Calling Agent**：模型自主决定调哪些工具（检索案例 / 查分类 / 存新案例），过程全程可视（trace）
- **多轮对话**：信息不足时主动追问 1–2 个关键点，用户补充后结合前文继续排查，不重复已做过的步骤
- **工程化**：FastAPI 提供 8 个 HTTP 接口 + Dockerfile 容器化 + 访问口令保护
- **自动化测试**：`test_ui.py`（AppTest 模拟真实点击）+ `test_api.py`（接口六步自测）

技术栈：Python · FastAPI · SQLite · Chroma · text-embedding-v3 · Function Calling · Docker · Streamlit

[查看仓库](https://github.com/licharlie203/it-troubleshooter) · [接口文档](https://it-troubleshooter-79990.app.workbuddy.host/docs)
</details>

<details>
<summary><b>🔍 ai-doc-qa — AI 文档问答（RAG 知识库）</b></summary>

基于通义千问 + Streamlit 的检索增强生成应用，支持 TXT / MD / PDF / DOCX。

- 完整 RAG 流程：文档解析 → 分块 → 向量化 → 余弦相似度检索 → LLM 生成
- 答案附带参考片段与相似度评分，**可溯源**
- 通过 Prompt 约束实现**防幻觉**：资料中没有时会主动拒答

技术栈：Python · Streamlit · text-embedding-v3 · NumPy · pypdf

[查看仓库](https://github.com/licharlie203/ai-doc-qa) · [在线体验](https://ai-doc-qa.app.workbuddy.host/)
</details>

<details>
<summary><b>🤖 ai-web-assistant — AI 网页助手</b></summary>

网页版 AI 应用，支持多轮上下文对话与六种语言翻译。

- 使用 `st.session_state` 管理会话状态，实现跨交互记忆
- API Key 三级读取：云端 Secrets → 环境变量 → 本地配置
- 侧边栏功能切换、清空对话、加载状态提示

技术栈：Python · Streamlit · Requests · 通义千问 API

[查看仓库](https://github.com/licharlie203/ai-web-assistant) · [在线体验](https://ai-web-assistant.app.workbuddy.host/)
</details>

<details>
<summary><b>🌐 ai-translator — AI 翻译工具</b></summary>

命令行版翻译工具，调用大模型 OpenAI 兼容接口，支持交互式多语言翻译。
包含完善的异常处理与友好错误提示。

[查看仓库](https://github.com/licharlie203/ai-translator)
</details>

<details>
<summary><b>📁 file-organizer — 文件整理工具</b></summary>

这是我的**第一个 Python 作品**，也是转行起点。
支持按文件类型 / 按修改日期两种整理模式，采用"先预览后执行"的安全设计。

[查看仓库](https://github.com/licharlie203/file-organizer)
</details>

---

## 🛠 技能栈

**语言**：Python

**AI 应用**：大模型 API 调用 · Prompt Engineering · RAG · 向量检索（Embedding）· Function Calling（Agent）· 多轮对话

**框架与库**：Streamlit · FastAPI · Chroma · Requests · NumPy · pypdf · python-docx

**工程化**：RESTful 接口设计 · Docker 容器化 · 自动化测试 · SQLite

**工具**：Git / GitHub · VS Code · pip · 服务部署上线

**其他**：3 年企业桌面运维经验，熟悉企业 IT 环境与硬件故障排查

---

## 📈 学习路线

```
Python 基础 ✅ → 调用大模型 API ✅ → 网页界面 ✅ → 部署上线 ✅ → RAG 基础 ✅
                                                              ↓
                   向量数据库 + 重排序 ✅ → Agent 开发 ✅ → FastAPI + Docker ✅ → 求职（进行中）
```

- [x] 掌握 Python 基础语法与文件操作
- [x] 独立完成大模型 API 调用
- [x] 用 Streamlit 构建网页应用
- [x] 项目部署上线，生成公网访问链接
- [x] 实现 RAG 检索增强问答
- [x] Chroma 向量数据库 + Rerank 重排序
- [x] Agent 开发（Function Calling 工具调用 + 多轮追问）
- [x] FastAPI + Docker 工程化
- [x] 垂直行业落地项目（IT 运维故障知识库）
- [ ] 拿到 AI 应用开发岗 offer 🎯

---

## 💡 关于我

- 🏢 目前在比亚迪驻场做桌面运维，利用空闲时间自学转行
- 🎯 目标岗位：**AI 应用开发工程师**（不走算法研究路线）
- 📚 每天都在学，每天都在往 GitHub 提交东西
- 🤝 欢迎交流 AI 应用开发、RAG、Agent 相关话题

<div align="center">

**持续学习中 · 每天进步一点点**

</div>
