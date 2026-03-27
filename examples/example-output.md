# Example Output

This is a worked example showing the standard of output expected from this skill.

## Scenario

- Reference images: clean dark SaaS dashboards, glassy UI cards, blue-cyan accents, strong whitespace
- Source material: internal AI transformation roadmap for a mid-sized company
- Audience: leadership team and department heads
- User preference: "你来决定，稳一点，但要有下一代科技感"
- Mode: normal

## Brief Recommendation

Recommended directions:

1. Professional Future
   Best fit for realistic digital transformation and premium enterprise credibility.
2. Executive Dashboard
   Best fit if the material is data-heavy and needs command-center summary energy.
3. Swiss + Glass Hybrid
   Best fit if the user wants a safer corporate structure with a subtle next-generation polish.

Default choice:

Professional Future with a restrained dashboard influence.

## Final NotebookLM Prompt

```yaml
role: "你是一位资深演示设计师兼信息设计顾问"

presentation:
  objective: "向管理层清楚说明 AI 转型路线图、关键阶段、资源重点和预期业务价值"
  audience: "公司管理层和各部门负责人，他们时间有限，需要快速看懂重点并建立信心"
  format: "16:9 widescreen"
  language: "zh-CN"

style:
  direction: "专业未来感为主，融合少量高管仪表盘式的信息组织方式"
  reference_family: "高端企业科技感、克制的玻璃拟态细节、清晰的战略表达"
  priority: "可信、清晰、下一代数字化升级感，而不是夸张的科幻感"
  mood: "冷静、专业、克制、高价值感"

  color_palette:
    background:
      - "深海军蓝"
      - "深炭灰"
    text:
      - "高对比白色"
      - "浅灰"
    accent:
      - "青蓝色"
      - "少量电光蓝"

  typography:
    headline: "简短有力，像战略页标题，而不是冗长说明句"
    body: "短句化、分组化，避免整段堆叠"
    text_density: "short blocks, avoid long paragraphs"

layout:
  composition:
    - "每页只表达一个核心信息"
    - "优先使用左右分栏、模块卡片、流程分段和高层摘要页"
    - "页面节奏保持留白充分、信息层级明确、重要数字或阶段一眼可见"
    - "封面和章节页可以使用更强的横向构图，主体偏左或偏右，另一侧保留明显留白"
  reading_flow: "left to right with strong modular grouping"
  overlay_space: "右侧或上方预留文字空白"

visuals:
  preferred:
    - "高端科技 UI 模块"
    - "流程节点"
    - "轻度玻璃感卡片"
    - "简洁图标和关系图"
  diagrams: "图示应服务于战略说明和阶段关系表达，不要只做装饰"
  image_treatment: "如出现抽象场景或技术背景，请保持克制、真实可落地的企业科技感"

rules:
  - "尽量减少长段文字，更多使用阶段分组、流程图、对比模块和关键数字"
  - "如果画面中需要出现文字，请控制在极短词组内，不要依赖图像里生成长文本"
  - "可以适当使用网络连接、平台模块、数据层级等视觉语言，但不要做成夸张赛博朋克"

avoid:
  - "避免杂乱背景和过多无意义发光效果"
  - "避免把每一页都做成同一种仪表盘"
  - "避免过强的 3D 景深、炫技式透视和泛滥渐变"
  - "避免看起来像通用 AI 模板，要更像经过设计的企业战略材料"

quality_check:
  - "最终请让整套幻灯片看起来清晰、有判断力、具有高端数字化品牌气质，同时保持真实可信和易读"
```

## Optional Follow-up

如果你要，我可以继续帮你收成更稳一点，或者更像高端极简商业风的一版。
