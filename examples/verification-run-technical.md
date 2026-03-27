# Verification Run: Technical Precision Scenario

This file records one manual verification pass using the skill workflow against `evals/evals.json` case 1.

## Input

User request:

> 我有3张工业蓝图风和拆解图风格的参考图，想做一个关于智能制造产线改造的 NotebookLM 幻灯片。受众是工厂负责人和技术团队。我偏好深蓝、白色和一点橙色。请帮我直接产出可贴到 NotebookLM 的成品提示词。

Mode:

- quick

## Reference Read

- 参考图大概率偏技术制图和结构拆解感
- 画面重点应是组件关系、流程逻辑、结构清晰度
- 深蓝和白色适合做主基调，少量橙色适合做节点和强调
- 这类项目更适合“结构 / 精确”方向，而不是强营销或强情绪化方向

## Recommended Directions

1. 蓝图主导
   适合强调总规划感、技术秩序和工程逻辑。
2. 爆炸图主导
   适合解释产线模块、部件关系和改造前后结构差异。
3. 极简技术数据混合
   适合需要同时呈现流程、指标和实施阶段的版本。

Default choice:

蓝图主导，融合少量爆炸图式结构表达。

## Final NotebookLM Prompt

```yaml
role: "你是一位资深工业演示设计师兼信息设计顾问"

presentation:
  objective: "清楚说明智能制造产线改造的现状、关键模块、改造逻辑、实施路径和预期效果"
  audience: "工厂负责人和技术团队，他们既关心整体规划，也关心系统结构和执行可行性"
  format: "16:9 widescreen"
  language: "zh-CN"

style:
  direction: "工业蓝图风为主，融合少量爆炸图式结构表达"
  reference_family: "工程制图感、结构拆解感、技术秩序感、清晰的系统关系表达"
  priority: "精确、清楚、可信、便于理解，而不是营销感或装饰感"
  mood: "理性、冷静、工程化、专业"

  color_palette:
    background:
      - "深蓝"
      - "深青蓝"
    text:
      - "高对比白色"
      - "浅灰"
    accent:
      - "少量橙色，用于关键节点、步骤和重要标注"

  typography:
    headline: "简短直接，像工程章节标题或改造步骤标题"
    body: "短句化、模块化，避免长段叙述"
    text_density: "short blocks, avoid long paragraphs"

layout:
  composition:
    - "每页只表达一个核心信息"
    - "优先使用左右分栏、流程分段、模块拆解和关系图布局"
    - "保持强结构感和清晰阅读路径，尽量从左到右或从上到下组织信息"
    - "当页面用于展示系统结构时，可采用主体偏左或主体偏右的横向构图，另一侧留作说明区域"
  reading_flow: "left to right or top to bottom"
  overlay_space: "上方或右侧预留标题与简短说明区"

visuals:
  preferred:
    - "蓝图线稿"
    - "结构分层图"
    - "模块拆解图"
    - "流程箭头"
    - "简洁技术图标"
  diagrams: "图示应服务于解释系统关系、模块组成和改造路径，不要只做装饰"
  image_treatment: "如需表现设备、产线或系统，请保持正投影、低透视、清晰边界和工程制图气质"

rules:
  - "尽量减少大段文字，更多使用流程、分层结构、关键参数和模块说明"
  - "如果画面中需要出现文字，请控制在极短标签内，不依赖图像里生成长文本"
  - "数据和指标页面可以加入极简图表，但整体风格要和蓝图逻辑保持一致"

avoid:
  - "避免杂乱背景、花哨纹理和无意义装饰"
  - "避免夸张 3D 景深、强透视变形和炫技式发光"
  - "避免做成通用科技营销页，要更像真正的工程改造方案说明"
  - "避免一页塞太多流程和太多模块，保持重点清楚"

quality_check:
  - "最终请让整套幻灯片看起来像经过设计的工业技术汇报材料，兼顾工程准确感、结构清晰度和实际可读性"
```

## Verification Notes

- Contains 3 recommended directions before final output
- Uses default narrowing without forcing more questions
- Produces a single paste-ready YAML NotebookLM prompt
- Includes 16:9 composition, text handling, image rules, and negative constraints
- In real use, this scenario should usually skip extra contrast and go straight to output because the user already asked for a direct result
