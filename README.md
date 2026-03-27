# notebooklm-slide-prompt-coach

把“我喜欢这种感觉的参考图”翻译成 **NotebookLM 可直接粘贴使用的 YAML 幻灯片提示词**。

这个 skill 不会强行替用户做审美决定。它更像一个轻量翻译器：

- 先看参考图和材料
- 轻轻说出它看到的感觉
- 必要时只做一点点对照
- 最后直接产出可贴进 NotebookLM 的 YAML 提示词

## 适合什么场景

- 你有几张喜欢的 slide 截图或参考图
- 你想让 NotebookLM 的幻灯片更像某种气质
- 你不想自己从零写复杂提示词
- 你喜欢 YAML 这种更清楚、更好改的形式

## 会产出什么

默认输出是：

- 一段可以直接粘贴进 NotebookLM 的 YAML 风格提示词

它会尽量包含这些部分：

- 目标
- 受众
- 风格方向
- 配色和情绪
- 版式节奏
- 图像与图示语言
- 避免事项

## 安装

### 给 AI Agent 安装

可以直接把这句话发给你的 AI agent：

```text
帮我安装 notebooklm-slide-prompt-coach：https://raw.githubusercontent.com/bilppppp/notebooklm-slide-prompt-coach/main/install.md
```

### 用 `npx skills add` 安装整个仓库

```bash
npx skills add https://github.com/bilppppp/notebooklm-slide-prompt-coach
```

### 用仓库路径安装这个 skill

这个仓库的 skill 就在根目录，所以直接用根路径即可：

```bash
npx skills add https://github.com/bilppppp/notebooklm-slide-prompt-coach/tree/main
```

## 怎么触发

适合在这些说法下触发：

- “帮我把这组参考图翻成 NotebookLM 的 slide 提示词”
- “我想做成这种气质的幻灯片”
- “请直接给我 YAML”
- “我有参考图和材料，帮我出 NotebookLM 提示词”

## 工作方式

这个 skill 默认比较轻：

- `quick`
  适合已经有明确感觉，只想直接出 YAML
- `normal`
  默认模式。会做一点点对照，再给 YAML
- `refined`
  适合重要材料。会更认真地收一版，但仍然尽量不把流程做重

它遵循一个很简单的原则：

**先翻译用户已经喜欢的感觉，再把它落成 NotebookLM 能执行的 YAML。**

## 风格范围

除了基础的讲解、结构、战略、亲和、高冲击几类，这个 skill 还扩展了更多具体方向，比如：

- 商业媒体风
- 高端极简商业风
- 蓝图工程风
- 拆解结构风
- 杂志封面风
- 漫画叙事风
- 数码拼贴潮流风
- 专业未来科技风

中文风格索引见：

- [`references/style-catalog-zh.md`](./references/style-catalog-zh.md)

## 仓库结构

```text
.
├── SKILL.md
├── README.md
├── install.md
├── evals/
├── examples/
└── references/
```

主要文件：

- [`SKILL.md`](./SKILL.md)
  主工作流
- [`references/output-template.md`](./references/output-template.md)
  最终 YAML 输出模板
- [`references/style-map.md`](./references/style-map.md)
  核心判断逻辑
- [`references/style-catalog-zh.md`](./references/style-catalog-zh.md)
  中文风格索引
- [`references/preferences.md`](./references/preferences.md)
  轻量偏好记忆说明

## 一个很短的使用例子

用户说：

> 我有几张深色 SaaS 参考图，想做一套 AI 战略汇报，给老板看。稳一点，但要有下一代科技感。直接给我 YAML。

这个 skill 会更倾向于：

- 先复述参考图的感觉
- 只在必要时提一个更稳的替代方向
- 直接给出一段 YAML 提示词

示例见：

- [`examples/example-output.md`](./examples/example-output.md)

## 偏好记忆

这个 skill 支持轻量偏好记忆，但不是强制的。

比如你可以长期保存：

- 输出语言
- 常用品牌色
- 常见气质偏好
- 默认模式

说明见：

- [`references/preferences.md`](./references/preferences.md)

## 说明

这个仓库吸收了一部分公开 NotebookLM prompt 集合的风格灵感，并转成了更适合这个 skill 的轻量工作流和 YAML 输出形式。

来源说明见：

- [`references/source-notes.md`](./references/source-notes.md)
