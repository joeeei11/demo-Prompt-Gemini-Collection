# The-common-Prompt-of-Gemini-and-Gemini-Cli-and-Nano-Banana
# 🧠 AI Prompts Library & Engineering Workflow

![Status](https://img.shields.io/badge/Status-Active-success)
![Focus](https://img.shields.io/badge/Focus-System_Architecture_%7C_Dual--End_Dev-blue)
![Powered By](https://img.shields.io/badge/Powered_By-Gemini_%7C_AI_Studio-orange)

> **"Decision in the Brain, Execution in the Hands."**
>
> 本仓库收录了经过实战验证的高质量 Prompt，专用于复杂软件架构设计、嵌入式系统开发以及高效的 AI 辅助编程工作流。

## 📖 简介 (Introduction)

在现代 AI 辅助开发中，单纯的 "Write code for me" 往往无法满足工程级需求。本仓库通过结构化的 Prompt 设计，解决了以下核心痛点：

1.  **架构可视化**：生成符合 IEEE/教科书标准的系统分层架构图。
2.  **职责分离**：通过 **"The Brain" (决策参谋)** 与 **"The Hands" (代码执行)** 的双端模式，确保代码逻辑严密且无 "Lazy Coding"。
3.  **版本追踪**：引入 `Phase X.Y` 动态锚点协议，防止多轮对话后的上下文漂移。

## 📂 核心内容 (Core Contents)

### 1. [可视化与架构绘图](./prompts_library.md#1-可视化与架构绘图-visualization)
专用于生成纯净、无阴影、正交布局的系统架构图 Prompt。
- **适用场景**：论文配图、技术文档、系统蓝图。
- **风格**：IEEE Standard / Textbook Style (Black & White).

### 2. [双端开发工作流 (The Dual-End Protocol)](./prompts_library.md#2-双端开发工作流-dual-end-workflow)
这是本仓库的核心方法论。

* **🧠 The Brain (Gemini)**:
    * 负责：技术选型、文件规划、版本号管理 (Phase Protocol)。
    * 输出：生成发送给 IDE/Coding AI 的精准指令 (Payload)。
* **🛠️ The Hands (AI Studio/Cursor)**:
    * 负责：具体代码实现、全量文件输出。
    * 原则：**ABSOLUTELY NO LAZY CODING** (严禁省略代码)。

### 3. [复杂任务指令模版](./prompts_library.md#3-具体任务指令模板-specific-task-specs)
针对特定复杂场景（如 Python/Qt 外部脚本集成、嵌入式驱动层设计）的定制化指令。

---

## 🚀 使用指南 (Usage Guide)

### 步骤 1：启动决策中枢 (The Brain)
在对话开始时，将 [The Brain Role](./prompts_library.md#🧠-角色-a-技术参谋-the-brain) 发送给你的对话模型（如 Gemini Advanced）。

> **它将开始为你计算版本号 (Anchor)：**
> `Phase1.0——项目初始化`

### 步骤 2：获取执行指令
当你提出需求（如“我要加个登录页”）后，**The Brain** 会分析依赖，并为你生成一段 Markdown 代码块。

### 步骤 3：执行代码 (The Hands)
将上一步生成的 Prompt 复制到你的编程 AI (如 AI Studio) 中。
*注：首次使用编程 AI 时，建议先注入 [The Hands System Instruction](./prompts_library.md#🛠️-角色-b-代码执行者-the-hands)。*

---

## ⚙️ 动态版本协议 (Dynamic Version Protocol)

为了在长对话中保持上下文连贯，我们强制执行以下版本规则：

| 版本号格式 | 触发条件 | 示例 |
| :--- | :--- | :--- |
| **Phase X.0** | 架构变动 / 新模块 / 新页面 | `Phase2.0——引入LSL数据流模块` |
| **Phase X.Y** | UI微调 / Bug修复 / 逻辑补充 | `Phase2.1——修复线程阻塞问题` |

---

## 📝 License

[MIT License](./LICENSE) © 2026
