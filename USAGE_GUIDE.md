# 🚀 Trae Skills 使用指南与示例大全

本文档旨在通过丰富的实战示例，帮助你快速掌握并充分利用 Trae Skills 库的强大能力。无论你是产品经理、架构师、全栈开发者还是测试人员，这里都有适合你的工作流。

## 🌟 核心理念：Skill First

在开始任何任务之前，先问自己：**“有没有 Skill 可以帮我做这件事？”**
Trae Skills 不是简单的代码片段，而是封装了专家经验的智能助手。

---

## 📚 目录

1.  [🧩 基础用法：如何调用 Skill](#-基础用法如何调用-skill)
2.  [🧠 场景一：从想法到方案 (Brainstorming & Architecture)](#-场景一从想法到方案-brainstorming--architecture)
3.  [💻 场景二：全栈开发 (Frontend & Backend)](#-场景二全栈开发-frontend--backend)
4.  [🛠️ 场景三：DevOps 与工具链 (Git, Docker, Testing)](#-场景三devops-与工具链-git-docker-testing)
5.  [🤖 场景四：构建 AI 应用 (MCP & RAG)](#-场景四构建-ai-应用-mcp--rag)
6.  [📄 场景五：文档与办公自动化 (Office & PDF)](#-场景五文档与办公自动化-office--pdf)

---

## 🧩 基础用法：如何调用 Skill

在对话框中，你只需要明确表达你的意图，或者直接提及 Skill 的名称（如果是为了测试）。但在实际工作中，**自然语言描述**效果最好。

*   **直接调用**: `请使用 brainstorming skill 帮我构思...`
*   **自然语言**: `我想设计一个电商系统的数据库结构...` (会自动触发 `Backend Database Expert`)

---

## 🧠 场景一：从想法到方案 (Brainstorming & Architecture)

### 1. 头脑风暴与需求澄清
**Skill**: `brainstorming`, `Meta Orchestrator`

> **User**: "我想做一个类似 Notion 的个人知识库应用，帮我规划一下功能。"
>
> **AI Action**: 调用 `brainstorming` skill。
>
> **Output**:
> 1.  **提问**: "目标用户是极客还是普通用户？侧重文档编辑还是数据库关联？"
> 2.  **核心功能列表**: 块级编辑器、双向链接、多视图数据库。
> 3.  **MVP 建议**: 先做 Markdown 编辑器和本地存储。

### 2. API 架构设计
**Skill**: `api-design-principles`

> **User**: "为这个知识库应用设计一套 RESTful API，包括笔记的增删改查和标签管理。"
>
> **AI Action**: 调用 `api-design-principles` skill。
>
> **Output**:
> ```yaml
> # RESTful API Design
> GET /notes?tags=work,urgent  # 过滤
> POST /notes                  # 创建
> PATCH /notes/{id}            # 部分更新
> GET /tags/{id}/notes         # 获取标签下的笔记
> ```
> *还会包含错误处理规范、分页策略等专家建议。*

---

## 💻 场景二：全栈开发 (Frontend & Backend)

### 1. 前端组件开发 (React/Vue/Flutter)
**Skill**: `frontend-design`, `Flutter Development Expert`

> **User (Web)**: "帮我写一个现代化的登录页面，使用 React 和 Tailwind CSS，要有极光风格的背景。"
>
> **AI Action**: 调用 `frontend-design` skill。
>
> **Output**: 生成包含 `shadcn/ui` 组件、响应式布局和精美 CSS 动画的完整代码。

> **User (Mobile)**: "用 Flutter 写一个带有下拉刷新和无限加载的商品列表页面。"
>
> **AI Action**: 调用 `Flutter Development Expert` skill。
>
> **Output**: 生成基于 BLoC 或 Provider 状态管理的高性能 ListView 代码。

### 2. 后端服务与数据库
**Skill**: `Backend Node.js Expert`, `Backend Python Expert`, `Backend Database Expert`

> **User**: "用 Node.js 写一个文件上传接口，要把文件存到 S3，并把元数据存到 MySQL。"
>
> **AI Action**: 调用 `Backend Node.js Expert` 和 `Backend Database Expert`。
>
> **Output**:
> 1.  **SQL**: `CREATE TABLE files (...)` (包含索引优化建议)
> 2.  **Node.js**: 使用 `multer` 处理流式上传，`aws-sdk` 对接 S3，包含完整的错误重试机制。

---

## 🛠️ 场景三：DevOps 与工具链 (Git, Docker, Testing)

### 1. Git 工作流管理
**Skill**: `git-workflow`

> **User**: "我要开始开发新功能 feature-login，帮我创建分支并推送到远程。"
>
> **AI Action**: 调用 `git-workflow` skill。
>
> **Output**:
> ```bash
> git checkout -b feature/login
> # 开发完成后...
> git commit -m "feat(auth): implement login page with validation"
> git push -u origin feature/login
> ```
> *它会指导你使用 Conventional Commits 规范。*

### 2. 自动化测试
**Skill**: `webapp-testing`

> **User**: "帮我测试一下刚才写的登录页面，确保输入错误的密码会显示红色警告框。"
>
> **AI Action**: 调用 `webapp-testing` skill (Playwright)。
>
> **Output**: 编写并运行 Playwright 脚本，自动打开浏览器，模拟用户输入，截图并验证 UI 状态。

---

## 🤖 场景四：构建 AI 应用 (MCP & RAG)

### 1. 开发 MCP Server
**Skill**: `mcp-builder`

> **User**: "我想把我的本地 SQLite 数据库变成一个 MCP Server，让 Claude 能直接查数据。"
>
> **AI Action**: 调用 `mcp-builder` skill。
>
> **Output**: 生成完整的 `server.py` (FastMCP) 或 `index.ts` (MCP SDK)，包含 `read_query` 和 `list_tables` 工具定义。

### 2. 寻找现成方案
**Skill**: `GitHub Search & Discovery`

> **User**: "有没有现成的 Notion MCP Server？"
>
> **AI Action**: 调用 `GitHub Search & Discovery` skill。
>
> **Output**: 搜索 GitHub，推荐 `modelcontextprotocol/servers` 中的官方实现，并告诉你如何配置。

---

## 📄 场景五：文档与办公自动化 (Office & PDF)

### 1. Excel 数据分析
**Skill**: `xlsx`

> **User**: "分析这个 `sales.xlsx` 文件，帮我计算每个季度的总销售额，并画一个柱状图。"
>
> **AI Action**: 调用 `xlsx` skill。
>
> **Output**: 读取 Excel 数据，使用 Pandas 进行聚合计算，并生成一个新的 Excel 文件，里面包含计算结果和嵌入的图表。

### 2. 批量生成 Word 报告
**Skill**: `docx`

> **User**: "根据 `data.json` 里的 100 个用户数据，用 `template.docx` 模板生成 100 份合同。"
>
> **AI Action**: 调用 `docx` skill。
>
> **Output**: 读取模板，替换占位符（如 `{{name}}`），批量生成并打包下载。

---

## 💡 进阶技巧：组合技 (Combo)

最强大的用法是将多个 Skill 串联起来：

> **User**: "帮我分析一下当前项目的 Python 代码质量，找出性能瓶颈，然后生成一份 PDF 格式的优化报告。"
>
> **Workflow**:
> 1.  **Backend Python Expert**: 扫描代码，分析复杂度。
> 2.  **brainstorming**: 构思优化方案。
> 3.  **pdf**: 将分析结果和方案写入 PDF 文档。

---

希望这份指南能帮你释放 Trae Skills 的无限潜力！🚀
