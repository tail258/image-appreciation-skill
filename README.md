<div align="center">

# 🖼️ Image Appreciation Skill

**从视觉结构走向审美理解，让图片鉴赏有依据、有层次、不空泛。**

**From visual structure to aesthetic understanding—thoughtful image appreciation grounded in visible evidence.**

<p>
  <a href="./LICENSE">
    <img alt="MIT License" src="https://img.shields.io/badge/License-MIT-4C8BF5?style=for-the-badge">
  </a>
  <img alt="Codex Skill" src="https://img.shields.io/badge/Codex-Skill-111827?style=for-the-badge">
  <img alt="Language" src="https://img.shields.io/badge/Language-中文%20%7C%20English-EF4444?style=for-the-badge">
  <img alt="Runtime Dependencies" src="https://img.shields.io/badge/Runtime_Dependencies-None-10B981?style=for-the-badge">
</p>

[中文](#中文) · [English](#english) · [目录结构](#目录结构) · [License](#license)

</div>

---

## 中文

### 项目简介

`Image Appreciation Skill` 是一个面向 Codex 的通用图片鉴赏技能。它不满足于复述“画面里有什么”，也不使用“很美、很可爱、很震撼”等缺乏依据的形容词堆叠，而是解释：

> **图像的视觉设计，如何改变观看者的感知，并进一步生成情绪、叙事和审美吸引力。**

该 Skill 适用于动漫人物、角色插画、摄影、传统与现代绘画、艺术风景、概念艺术、CG、海报、建筑、室内、静物、产品图和抽象作品。

### 核心方法

```mermaid
flowchart LR
    A["视觉证据<br/>色彩 · 光影 · 构图 · 材质"] --> B["感知变化<br/>注意 · 距离 · 重量 · 速度 · 空间"]
    B --> C["情绪与叙事效果"]
    C --> D["视觉—情绪模型"]
    D --> E["吸引力机制"]
```

每项主要判断遵循同一条推理链：

```text
视觉参数 → 感知变化 → 情绪或叙事效果
```

例如：

```text
低地平线 + 大面积云层 + 极小人物参照
→ 天空获得压倒性尺度，人物控制感降低
→ 形成崇高感，并混入轻微的脆弱与敬畏
```

### 功能亮点

| 🔍 结构先行 | 🧠 因果推导 | 🎨 多题材适配 |
|---|---|---|
| 先拆解色彩、光影、构图、空间、线条与材质，再进入情绪评价 | 所有关键结论都由可见证据推导，避免空泛审美词 | 分别适配人物、动漫、风景、抽象、建筑、静物与产品图 |

| 🧩 模型归纳 | ✨ 吸引力解释 | ⚖️ 保留不确定性 |
|---|---|---|
| 归纳“温柔疏离型”“开阔崇高型”等视觉—情绪模型，并给出依据 | 解释注意力为何被捕获、维持，以及画面为何值得再次观看 | 区分观察与推断，避免武断确认作者、流派、媒介或人物心理 |

### 支持的鉴赏模式

- **完整鉴赏**：视觉结构、情绪机制、主体关系、风格模型、吸引力机制与综合评价。
- **简洁鉴赏**：保留关键证据、至少两条因果链、模型判断和吸引力结论。
- **对比鉴赏**：逐项比较两幅或多幅作品，不把差异简化为绝对优劣。
- **专项鉴赏**：聚焦色彩、构图、光影、角色表现、场景氛围或视觉吸引力。
- **创作反馈**：在完成作品现状判断后，给出独立、可执行的调整方向。

### 安装

将仓库克隆到 Codex Skills 目录，并使用与 Skill 名称一致的目标文件夹：

<details>
<summary><strong>Windows PowerShell</strong></summary>

```powershell
git clone https://github.com/tail258/image-appreciation-skill.git `
  "$HOME\.codex\skills\analyze-image-aesthetics"
```

</details>

<details>
<summary><strong>macOS / Linux</strong></summary>

```bash
git clone https://github.com/tail258/image-appreciation-skill.git \
  "${CODEX_HOME:-$HOME/.codex}/skills/analyze-image-aesthetics"
```

</details>

重新启动或刷新 Codex，使其发现新 Skill。

### 使用方式

显式调用：

```text
$analyze-image-aesthetics 请鉴赏这张动漫人物插画，重点解释角色的姿态、视线与亲近感。
```

```text
$analyze-image-aesthetics 分析这幅风景画如何通过空间、色彩和尺度产生崇高感。
```

```text
$analyze-image-aesthetics 对比这两张图片的构图逻辑与吸引力机制。
```

当用户提出图片赏析、审美分析、画面解读、构图与色彩分析、角色视觉心理分析或作品吸引力分析时，Skill 也可以被隐式触发。

### 输出原则

1. 先写可见证据，再写情绪结论。
2. 每个主要判断都建立明确因果链。
3. 人物图分析姿态、视线、肢体语言和表情微变化。
4. 无人物图使用尺度、纵深、路径、自然力和空间可进入性等变量。
5. 必须给出有依据的视觉—情绪模型。
6. 必须回答“这张图的吸引力来自什么机制？”
7. 不诊断现实人物，不虚构画外信息，不做无关的道德评价。

---

## English

### Overview

`Image Appreciation Skill` is a general-purpose Codex skill for thoughtful visual appreciation. Instead of merely listing visible objects or stacking vague adjectives such as “beautiful,” “cute,” or “stunning,” it explains:

> **How visual design shapes perception—and how those perceptual changes produce emotion, narrative, and aesthetic appeal.**

The skill works with anime characters, illustrations, photography, traditional and contemporary paintings, artistic landscapes, concept art, CG, posters, architecture, interiors, still life, product imagery, and abstract art.

### Core Method

Every major interpretation follows an evidence-based causal chain:

```text
Visual parameters → Perceptual change → Emotional or narrative effect
```

The skill first examines color, lighting, composition, space, line, shape, texture, and detail. It then evaluates how these elements guide attention, establish distance, suggest weight or motion, organize space, and ultimately create an emotional experience.

### Highlights

| 🔍 Structure First | 🧠 Causal Reasoning | 🎨 Medium-Agnostic |
|---|---|---|
| Examines visible structure before making emotional judgments | Grounds every important claim in visual evidence | Adapts its vocabulary to characters, landscapes, abstraction, architecture, still life, and product imagery |

| 🧩 Visual–Emotional Models | ✨ Appeal Mechanisms | ⚖️ Calibrated Uncertainty |
|---|---|---|
| Derives models such as “gentle distance” or “expansive sublime” and explains why they fit | Explains how attention is captured, sustained, and rewarded | Separates observation from inference and avoids unsupported attribution |

### Appreciation Modes

- **Full appreciation**: visual structure, emotional mechanisms, subject relationships, style model, appeal mechanisms, and overall evaluation.
- **Concise appreciation**: essential evidence, at least two causal chains, one model, and a clear appeal conclusion.
- **Comparative appreciation**: compares multiple works across shared dimensions without reducing them to a simplistic ranking.
- **Focused appreciation**: concentrates on color, composition, lighting, character expression, atmosphere, or visual appeal.
- **Creative feedback**: separates the current-work assessment from optional, actionable revision suggestions.

### Installation

Clone the repository into the Codex Skills directory using a destination folder that matches the Skill name:

<details>
<summary><strong>Windows PowerShell</strong></summary>

```powershell
git clone https://github.com/tail258/image-appreciation-skill.git `
  "$HOME\.codex\skills\analyze-image-aesthetics"
```

</details>

<details>
<summary><strong>macOS / Linux</strong></summary>

```bash
git clone https://github.com/tail258/image-appreciation-skill.git \
  "${CODEX_HOME:-$HOME/.codex}/skills/analyze-image-aesthetics"
```

</details>

Restart or refresh Codex so that it can discover the new Skill.

### Usage

Invoke the Skill explicitly:

```text
$analyze-image-aesthetics Appreciate this anime character illustration, focusing on posture, gaze, and perceived intimacy.
```

```text
$analyze-image-aesthetics Explain how space, color, and scale create a sense of the sublime in this landscape.
```

```text
$analyze-image-aesthetics Compare the compositional logic and appeal mechanisms of these two images.
```

The Skill may also trigger implicitly when a user requests image appreciation, aesthetic interpretation, composition or color analysis, character-focused visual psychology, atmosphere critique, or an explanation of visual appeal.

### Design Principles

1. Describe visible evidence before drawing emotional conclusions.
2. Express major judgments through explicit causal chains.
3. Analyze posture, gaze, body language, and micro-expression when a character is present.
4. Use scale, depth, pathways, natural forces, and spatial accessibility when no character is present.
5. Derive and justify a visual–emotional model.
6. Directly answer: “What mechanism makes this image appealing?”
7. Avoid diagnosing real people, inventing unseen information, or making irrelevant moral judgments.

---

## 目录结构

```text
analyze-image-aesthetics/
├── SKILL.md
├── README.md
├── LICENSE
├── agents/
│   └── openai.yaml
└── references/
    ├── analysis-framework.md
    └── output-patterns.md
```

- `SKILL.md`：触发条件、核心工作流、写作约束与完成标准。
- `agents/openai.yaml`：Codex 界面显示名称、简介和默认调用提示。
- `references/analysis-framework.md`：跨题材视觉鉴赏框架。
- `references/output-patterns.md`：完整、简洁和对比鉴赏模板。

## Contributing

Issues and pull requests are welcome. When proposing a new analytical dimension or output pattern, please include:

- the image category it serves;
- the visible evidence it relies on;
- the causal chain it enables;
- an example that avoids vague aesthetic language.

欢迎提交 Issue 与 Pull Request。新增分析维度或输出模式时，请说明其适用图片类型、依赖的视觉证据、能够建立的因果链，并提供一个避免空泛审美词的示例。

## License

Released under the [MIT License](./LICENSE).

本项目采用 [MIT 许可证](./LICENSE) 开源。

<div align="center">

**Look closely. Explain clearly. Appreciate deeply.**

**看得细，讲得清，鉴赏得更深。**

</div>
