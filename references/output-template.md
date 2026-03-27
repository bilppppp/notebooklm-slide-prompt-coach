# Output Template

Use this file to assemble the final paste-ready NotebookLM prompt.

The final prompt should be one coherent instruction block, not a fragmented note dump.

Write the final prompt in the user's language unless they explicitly request another language.

Default output format: YAML-style prompt block.

Fallback format: plain natural language only if the user explicitly dislikes YAML.

## Required Structure

Build the final NotebookLM prompt with these parts, in this order:

1. role
2. objective
3. audience
4. visual direction
5. color and mood
6. layout and composition
7. text treatment
8. images, diagrams, and visual language
9. slide behavior rules
10. negative constraints
11. final quality check

## Assembly Rules

### 1. Role

Frame NotebookLM as:

- a senior presentation designer
- an information designer
- a visual strategist

Pick whichever best fits the project.

### 2. Objective

State what the deck is trying to do.

Examples:

- explain a technical system clearly
- persuade stakeholders
- train new team members
- summarize a research report
- make a strategic case with confidence

### 3. Audience

Name the audience plainly.

Examples:

- internal team members
- executives
- customers
- investors
- trainees with little prior knowledge

### 4. Visual Direction

Describe the chosen direction in natural language.

Include:

- overall feel
- closest style family or hybrid
- what should dominate visually

Examples:

- calm swiss-style structure with restrained futuristic polish
- high-clarity blueprint logic with editorial whitespace
- human, workshop-like sketch-note warmth with soft corporate polish

### 5. Color and Mood

Write this as a small system:

- background tone
- main text tone
- accent colors
- emotional temperature

If brand colors are provided, explicitly fold them in.

### 6. Layout and Composition

Always include widescreen guidance.

Use practical rules such as:

- 16:9 widescreen layout
- strong asymmetrical compositions
- one message per slide
- generous whitespace
- left-to-right or top-to-bottom reading flow
- hero visuals on one side, text on the other
- reserve empty space for NotebookLM text overlays when useful

### 7. Text Treatment

State:

- how dense the text should be
- headline style
- subtitle style
- whether lists should be bullets, numbered, or diagram-based

Prefer short text blocks.

### 8. Images, Diagrams, and Visual Language

State what kind of visuals should appear.

Examples:

- flat diagrams and minimal icons
- cutout monochrome photography
- isometric systems
- hand-drawn arrows and sketch icons
- dashboard-like modules

If the task is technical, say that the visuals should prioritize explanation over decoration.

### 9. Slide Behavior Rules

Use practical operating rules like:

- each slide should communicate one key message
- use diagrams where relationships matter
- use comparison layouts for trade-offs
- avoid crowding too many claims on one page
- keep the deck visually consistent from slide to slide

### 10. Negative Constraints

Include only what matters.

Examples:

- avoid cluttered backgrounds
- avoid generic stock-photo energy
- avoid long decorative text inside images
- avoid excessive gradients
- avoid shiny effects that reduce clarity
- avoid forcing every slide into the same layout

### 11. Final Quality Check

End with a short check line.

Examples:

- prioritize clarity first, style second
- keep the result elegant but readable
- make the deck feel intentional, not generic

## Suggested Final YAML Format

Use this pattern and fill it with project-specific choices:

```yaml
role: "你是一位资深演示设计师兼信息设计顾问"

presentation:
  objective: "【目标】"
  audience: "【受众】"
  format: "16:9 widescreen"
  language: "【跟随用户语言】"

style:
  direction: "【视觉方向】"
  reference_family: "【最贴近的风格或混合方向】"
  priority: "【结构清晰 / 愿景感 / 亲和感 / 冲击力】"
  mood: "【情绪温度】"

  color_palette:
    background:
      - "【背景色 1】"
      - "【背景色 2】"
    text:
      - "【文字色】"
    accent:
      - "【强调色 1】"
      - "【强调色 2，可选】"

  typography:
    headline: "【标题风格】"
    body: "【正文风格】"
    text_density: "short blocks, avoid long paragraphs"

layout:
  composition:
    - "每页只表达一个核心信息"
    - "优先使用【构图方式】"
    - "保持【留白 / 模块化 / 左右分栏 / 时间线 / 仪表盘式】的页面节奏"
  reading_flow: "【左到右 / 上到下 / 模块化扫描】"
  overlay_space: "【左侧 / 右侧 / 上方 / 下方】预留文字空白"

visuals:
  preferred:
    - "【图像语言 1】"
    - "【图像语言 2】"
    - "【图像语言 3】"
  diagrams: "图示应服务于【解释 / 结构 / 愿景 / 说服】，不要只做装饰"
  image_treatment: "【真实 / 插画 / 手绘 / 等距 / 仪表盘】保持一致"

rules:
  - "尽量减少长段文字，更多使用【列表 / 图示 / 对比 / 流程】"
  - "如果画面中需要出现文字，请控制在极短词组内"
  - "保持整套幻灯片视觉一致，不要每页换一套风格"

avoid:
  - "【限制 1】"
  - "【限制 2】"
  - "【限制 3】"

quality_check:
  - "最终请让整套幻灯片看起来【最终质感要求】"
```

## YAML Writing Notes

When assembling the final YAML:

- prefer readable Chinese or the user's language inside values
- do not over-nest
- keep field names stable
- use lists for visual rules and avoid rules
- make the YAML feel copyable, not academic

## Quality Bar

A good final prompt should feel like:

- directly usable
- visually opinionated
- constrained enough to reduce randomness
- broad enough that NotebookLM can still generate varied slides
- structured enough that users can tweak single sections later
