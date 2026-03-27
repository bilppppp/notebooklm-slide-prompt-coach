# Style Map

Use this file to decide what direction fits the project best before generating the final NotebookLM prompt.

## 1. Read Reference Images First

Before naming a style, extract these signals from the references:

### Palette

- light neutral
- dark premium
- saturated campaign
- earth tone
- neon tech

### Contrast

- low contrast and calm
- medium contrast and professional
- high contrast and forceful

### Density

- spacious and editorial
- balanced and businesslike
- dense and dashboard-like

### Image Language

- photography-led
- diagram-led
- icon-led
- illustration-led
- texture-led

### Tone

- explanatory
- precise
- visionary
- human
- aggressive

### Composition

- asymmetric editorial
- left visual / right text
- right visual / left text
- centered hero
- modular grid
- timeline or process flow

## 2. Fast Selection Rules

If the user only wants a quick decision, use these defaults.

### A. Explain / Train

Use when the goal is:

- teaching
- onboarding
- training
- simplifying a complex topic

Prefer:

- blackboard
- whiteboard
- sketch note
- minimal 2D visual explanation

Default output tendency:

- easy to follow
- lighter terminology
- simple diagrams
- obvious reading flow

### B. Structure / Precision

Use when the goal is:

- technical explanation
- architecture
- data logic
- process clarity

Prefer:

- exploded view
- blueprint
- minimal 2D data viz
- high-contrast monospace
- swiss structure

Default output tendency:

- strong hierarchy
- diagram-first pages
- restrained colors
- less emotional imagery

### C. Vision / Strategy

Use when the goal is:

- roadmap
- executive communication
- digital transformation
- future positioning

Prefer:

- strategic infographic
- executive dashboard
- professional future
- glassmorphism UI
- swiss editorial

Default output tendency:

- confident framing
- cleaner summaries
- stronger hero pages
- polished strategic feel

### D. Human / Approachable

Use when the goal is:

- team story
- change management
- HR
- culture
- workshop summary

Prefer:

- sketch note
- corporate memphis
- paper craft
- kawaii
- tactile 3D

Default output tendency:

- friendlier diagrams
- more people presence
- softer color decisions
- less intimidating pages

### E. Impact / Campaign

Use when the goal is:

- launch
- promotion
- recruiting campaign
- high-energy storytelling

Prefer:

- pop art
- risograph
- retro print
- brutalism
- cyberpunk

Default output tendency:

- higher contrast
- bigger headlines
- more stylized rhythm
- less conservative layouts

## 3. Strategic Pair Decisions

Use these pairings when the user seems torn between similar options.

### Technical Data

- exploded view: best when explaining how parts fit together
- high-contrast monospace: best when the authority of the data itself matters more than the mechanism

### Data Authority

- minimal 2D data visualization: best for direct, clean, undeniable statistics
- executive dashboard: best for dense summary, control-room, live-overview feeling

### Corporate Tone

- swiss design: more stable, mature, safe
- glassmorphism UI: more next-generation, premium, disruptive

### Human Connection

- sketch note: more personal, live, workshop-like
- corporate memphis: more scalable, professional, team-communication friendly

### Emotional Depth

- graphite / charcoal: more solemn, historic, reflective
- watercolor: more atmospheric, fluid, artistic

### Future Feeling

- professional future: best for realistic high-end transformation
- cyberpunk: best for aggressive, sharp, disruptive future energy

### Brand Impact

- retro print: classic, archival, editorial
- risograph: trendier, more modern, more saturated artistic punch

## 4. Color Override Rules

Most directions can absorb brand colors without losing the style.

When rewriting the final prompt, think in three layers:

### Base

Main background color.

Example:

- deep navy background
- warm off-white background
- charcoal gray background

### Accents

One or two emphasis colors.

Example:

- electric gold and teal accents
- terracotta and sage accents
- neon orange linework

### Lighting / Temperature

The emotional light direction of the deck.

Example:

- warm amber lighting
- cool daylight blue
- soft neutral studio light

If the user has a strong brand color, preserve the style structure but rewrite the color system around that brand color.

## 5. Widescreen and Overlay Rules

NotebookLM slides are usually 16:9 widescreen.

If the intended slides need room for titles or labels, the final prompt should include ideas like:

- 16:9 widescreen aspect ratio
- cinematic horizontal composition
- main subject on the far left, leaving empty whitespace on the right for text overlay
- main subject on the far right, leaving empty whitespace on the left for text overlay

## 6. Text Handling Rules

Generated images often fail on long text.

Default recommendation:

- use visuals, icons, and shape language first
- let NotebookLM handle headings and real text
- if text must appear visually, keep it very short

## 7. Negative Constraints

Use when the references are clean or when outputs may become too “AI-like.”

### Clean Style Negatives

- avoid cluttered backgrounds
- avoid photo-realistic stock imagery
- avoid muddy textures
- avoid excessive gradients
- avoid decorative ornaments that do not support the message

### Technical Style Negatives

- avoid perspective distortion
- avoid dramatic 3D depth of field
- avoid ornamental shadow effects
- avoid unnecessary glossy surfaces

## 8. Recommendation Formula

When recommending three directions, use this order:

1. one direction that matches the references most closely
2. one direction that improves communication clarity
3. one direction that adds more brand or emotional force

This keeps the user from getting trapped in only one kind of recommendation.
