# Webnovel Serial Architect

[English README](README.en.md)

`webnovel-serial-architect` 是一个面向中文网文长篇创作的 Codex skill。它不是单纯的大纲生成器，而是帮助作者从零散灵感开始，逐步形成过稿大纲、开篇执行方案，并在连载过程中滚动维护人物、伏笔、时间线和后续章节。

## 适合什么场景

- 你只有一个脑洞、人物、设定、画面或爽点，想判断能不能发展成长篇。
- 你想整理一份给编辑、平台或自己评估用的网文过稿大纲。
- 你不想一开始定完整全书大纲，只想先把第一章、前三章、前十章写起来。
- 你已经写了一部分，需要根据现有正文滚动补纲、续线、补伏笔或修节奏。
- 你卡文了，需要诊断主角目标、冲突、爽点兑现、人物动机或时间线问题。

## 核心理念

```text
先记录灵感，再形成卖点；
先能开写，再逐步补全；
先跑通前十章，再滚动维护长线。
```

长篇网文不一定要在第一天就确定全书完整结局。这个 skill 会把内容标记为 `固定`、`暂定`、`延后`，帮助作者保留创作弹性，同时避免越写越散。

## 能力模块

- **灵感库**：记录脑洞、人物、冲突、设定、爽点、场景、对白、伏笔和市场观察。
- **题材定位**：判断类型、目标读者、核心情绪、卖点、读者期待和长篇可持续性。
- **过稿大纲**：整理书名方向、题材、主角、金手指、核心冲突、前十章钩子、第一卷和文案。
- **开篇执行**：设计第一章、前三章、前十章的冲突、爽点、钩子和推进节奏。
- **滚动补纲**：从已写内容中提取当前剧情状态，再规划后续 5-10 章。
- **卡文诊断**：检查目标不清、冲突不足、设定堆砌、爽点过慢、伏笔过载等问题。
- **创作资料维护**：维护人物状态卡、伏笔日志、时间线和待用素材。

## 目录结构

```text
webnovel-serial-architect/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── inspiration-system.md
│   ├── market-positioning.md
│   ├── submission-outline.md
│   ├── opening-chapters.md
│   ├── rolling-outline.md
│   └── plot-diagnosis.md
└── assets/
    ├── inspiration-card-template.md
    ├── inspiration-bank-template.md
    ├── submission-outline-template.md
    ├── first-ten-chapters-template.md
    ├── rolling-outline-template.md
    ├── character-state-card.md
    └── timeline-template.md
```

## 使用方式

把 `webnovel-serial-architect/` 目录放入 Codex 的 skills 目录后，可以这样使用：

```text
Use $webnovel-serial-architect 帮我把这个脑洞整理成网文过稿大纲。
```

也可以直接描述当前状态：

```text
我只有一个重生复仇的脑洞，想先写前三章，不想现在定完整结局。
```

```text
我已经写了 8 章，后面卡住了，帮我根据已有剧情滚动补接下来 10 章。
```

## 设计来源

这个 skill 的设计参考了三类网文创作流程：

- 有规划写作：题材定位、灵感库、核心冲突、人物、时间线和章节节奏。
- 过稿大纲模板：类型、基调、主线、人物关系、结尾方向和文案。
- 雪花写作法：一句话概括、一段式扩写、人物、大纲、场景清单和动笔。

最终设计重点放在“可开始、可过稿、可滚动更新”，而不是一次性生成完整全书设定。
