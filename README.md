<div align="center">

<img src="assets/supercharge-hero.png" alt="Supercharge: selecting a useful path from many possibilities" width="100%">

# Supercharge · 超给力

**给 AI 一套找方法、用方法、检查结果的工作方式。**<br>
**A practical methodology router for AI agents.**

拆解问题 · 选择方法 · 动手执行 · 检查结果<br>
Frame the problem · Choose a method · Act · Verify

[中文](#中文) · [English](#english)

</div>

---

## 中文

### Supercharge 是什么？

Supercharge 是一个面向 AI Agent 的 Skill。你用自然语言描述目标，它根据问题的性质、现有证据和现实约束，选择合适的思维方式或方法论，帮助你推进任务，并在交付时简要说明实际用了什么方法。

它不要求你记住每一个专业术语。无论你想排查增长问题、比较方案、检查论证，还是设计一次实验，Supercharge 都可以从方法库中寻找合适的起点。简单任务则可以直接处理，不必强行套用框架。

> **方法帮助我们提出更好的问题和检验路径；它本身不能替代数据、领域知识或真实验证。**

### 它如何工作？

![从问题到方法、执行和验证的工作流程](assets/supercharge-workflow.png)

1. **理解问题**：明确目标、交付物、约束、现有证据和关键未知。
2. **选择并执行**：从方法库中按需选择一种或多种互补方法；必要时结合专业 Skill 或查阅可靠资料。
3. **检查与交付**：根据任务核对事实、假设和结果，区分已经完成的验证与建议开展的测试。
4. **说明方法**：简要告诉你实际使用的方法及作用；如果要求纯代码或严格 JSON，则不破坏指定格式。

工作深度随任务复杂度和风险调整。出现新信息时，Supercharge 可以重新判断问题或更换方法。

### 安装到 Codex

需要 Git。以下命令将整个仓库克隆到**当前项目**的 Agent Skills 目录：

```bash
mkdir -p .agents/skills
git clone https://github.com/MJorgin/supercharge.git .agents/skills/supercharge
```

如需在多个项目中使用，可以将目标路径改为 `~/.agents/skills/supercharge`。如果目标目录已存在，`git clone` 会报错；请先检查现有内容，再决定如何更新。安装后，如 Skill 没有立即出现，可重新启动 Codex 或开启新会话。

其他支持 Agent Skills 的工具，也可以将完整目录放入对应的 Skills 目录。具体位置和调用方式取决于所用工具；请保留 `SKILL.md` 与 `references/` 的相对位置。

### 开始使用

在支持显式调用的环境中，可输入 `$supercharge`，也可以直接说“使用超给力”。例如：

```text
使用 $supercharge：我们的产品注册人数在增长，但新用户留存下降。
请帮我拆解可能原因，区分已有事实和待验证假设，设计下一步调查。
```

```text
使用超给力：我要比较三个供应商方案。
请考虑价格、交付风险、长期合作和谈判中的替代方案。
```

```text
使用超给力：检查下面这段论证的前提、推理和可能的反例。
```

对于第一个请求，它可能组合**漏斗分析、用户群组留存和假设驱动分析**；有真实数据时再进行分析。具体方法由任务与可用证据决定，而不是预设所有请求都走同一条流程。

### 使用边界

- **输入决定上限**：缺少数据、模型或权限时，说明缺口和假设，不编造结果。
- **验证要真实发生**：实验方案、模拟设计和已经完成的实验是不同的事情。
- **方法可以跨领域借鉴**：先检查问题结构和适用前提，再结合当前场景调整。
- **联网是按需能力**：是否可搜索取决于所用环境和用户要求；禁用联网时使用现有资料并说明限制。
- **方法库仍在完善**：条目提供适用场景、步骤和边界，但尚未逐项通过真实任务验证。

---

## English

### What is Supercharge?

Supercharge is an AI agent skill for choosing and applying practical methods. Describe your goal in plain language, and it considers the problem, available evidence, and constraints before selecting a useful way forward. After delivering the result, it briefly explains the methods actually used.

You do not need to memorize framework names. Supercharge can draw on its library for problems ranging from growth diagnostics and decision-making to argument review and experiment design. Straightforward tasks can remain straightforward.

> **Methods help frame questions and tests; they do not replace evidence, domain expertise, or real-world validation.**

### How it works

1. **Frame** the objective, deliverable, constraints, evidence, and unknowns.
2. **Choose and act** using one or more suitable methods, consulting specialist skills or reliable sources when appropriate.
3. **Verify and deliver** by checking facts, assumptions, and results; distinguish completed checks from proposed tests.
4. **Explain the approach** briefly, without breaking an explicitly requested format such as code-only or strict JSON.

The depth of work adapts to the task and its consequences. When new evidence changes the picture, the approach can change too.

### Install for Codex

Git is required. Clone the complete repository into the Agent Skills directory of your **current project**:

```bash
mkdir -p .agents/skills
git clone https://github.com/MJorgin/supercharge.git .agents/skills/supercharge
```

For use across projects, replace the destination with `~/.agents/skills/supercharge`. If that directory already exists, Git will refuse to clone into it; inspect the existing content before updating it. If the skill does not appear immediately, restart Codex or start a new session.

For other Agent Skills-compatible tools, put the complete directory in the tool's supported skills location. Discovery and invocation vary by tool; keep `SKILL.md` and `references/` together.

### Try it

In an environment that supports explicit invocation, use `$supercharge`, or ask the agent to use Supercharge directly:

```text
Use $supercharge: Our sign-ups are growing, but new-user retention is falling.
Separate known facts from hypotheses and propose the next investigation.
```

```text
Use Supercharge to compare three suppliers, considering price, delivery risk,
long-term cooperation, and our alternatives if negotiations fail.
```

```text
Use Supercharge to examine the premises, reasoning, and possible counterexamples
in the following argument.
```

For the first request, the agent might combine **funnel analysis, cohort retention, and hypothesis-driven analysis**, depending on the available evidence. These are examples, not a mandatory sequence.

### Boundaries

- **Evidence matters**: missing data, models, or permissions must be identified rather than invented.
- **Verification must be real**: a proposed experiment is not a completed experiment.
- **Cross-domain methods need adaptation**: check structural similarities and assumptions before transferring a method.
- **Web research is conditional**: it depends on the environment and the user's instructions.
- **The library is evolving**: entries describe use cases, steps, and limitations; they have not all been validated on real tasks.

---

## 方法库 / Method library

首页仅展示方法分类；完整方法库在公开仓库中，可通过以下链接查看和安装。每份手册都有中文与英文版本，Skill 主指令目前为中文。

This page shows categories only. The complete method library is public and included when you install the repository. Each guide is available in Chinese and English; the main skill instructions are currently in Chinese.

| 方法领域 / Area | 中文 | English |
| --- | --- | --- |
| 基础方法 / Foundations | [中文](references/methods.md) | [English](references/en/methods.md) |
| 调查、战略与协作 / Research, strategy & collaboration | [中文](references/field-methods.md) | [English](references/en/field-methods.md) |
| 增长与用户 / Growth & users | [中文](references/growth.md) | [English](references/en/growth.md) |
| 产品与执行 / Product & execution | [中文](references/product.md) | [English](references/en/product.md) |
| 商业与投资 / Business & investment | [中文](references/investment.md) | [English](references/en/investment.md) |
| 逻辑与论证 / Logic & argument | [中文](references/logic.md) | [English](references/en/logic.md) |
| 博弈与谈判 / Game theory & negotiation | [中文](references/game-theory.md) | [English](references/en/game-theory.md) |

```text
supercharge/
├── SKILL.md              # Routing and execution instructions
├── references/           # Chinese guides, sources, and English companions
├── assets/               # README illustrations
├── README.md
└── LICENSE
```

## License

[MIT](LICENSE) © 2026 MJorgin
