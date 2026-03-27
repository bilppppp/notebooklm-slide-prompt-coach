# Extended Style Catalog

Use this file when the user wants a more specific visual family than the core five-direction map.

This catalog folds in ideas from the public repo `serenakeyitan/awesome-notebookLM-prompts` and turns them into selection guidance for this skill.

## 1. Editorial & Business

### Modern Newspaper

Best for:

- founder essays
- market commentary
- business analysis
- high-signal thought leadership

Traits:

- oversized headline hierarchy
- asymmetrical placement
- strong whitespace tension
- monochrome photography or cutout subjects
- yellow or red marker-like highlights

Good when the user wants:

- intellectual energy
- modern media feel
- editorial punch without chaos

### Sharp-edged Minimalism

Best for:

- company profiles
- product overviews
- architecture summaries
- executive decks that should feel expensive but calm

Traits:

- rigid grid
- thin lines
- monochrome palette
- top-left navigation cues
- quiet luxury whitespace

Good when the user wants:

- maturity
- restraint
- premium but safe structure

### Yellow × Black Editorial

Best for:

- bold brand explainers
- trend reports
- youth-facing business content

Traits:

- yellow field
- strong black typography
- fashion-magazine rhythm
- handwritten or sticker-like accents

Good when the user wants:

- loud but organized
- magazine energy
- strong visual memory

### Black × Orange Creative Agency

Best for:

- agency pitches
- product launches
- portfolio storytelling

Traits:

- white or light background
- black typography
- blood-orange accents
- dynamic simple photography
- stylish English labels

Good when the user wants:

- creative confidence
- agency polish
- modern commercial feel

### Seminar Use (Minimal Text)

Best for:

- conference speaking
- training sessions
- workshops

Traits:

- fewer words
- bolder visual beats
- large supporting graphics

Good when the user wants:

- projection readability
- less dense pages

## 2. Pop, Youth, and Street

### Manga Style

Best for:

- educational explainers
- onboarding
- storytelling through scenes

Traits:

- comic framing
- narrative sequencing
- fun without becoming random

Good when the user wants:

- better memorability
- more engagement

### Magazine Style

Best for:

- lifestyle content
- feminine or trend-led decks
- social-first brand storytelling

Traits:

- cutout subjects
- numbered snippets
- trim-mark accents
- side labels
- editorial pink or muted palettes

Good when the user wants:

- polished magazine layout
- soft but intentional style

### Pink Street-style

Best for:

- youth campaigns
- creator decks
- playful launches

Traits:

- louder color use
- street-fashion rhythm
- expressive labels

### Digital / Neo / Pop

Best for:

- startup tools
- builder culture
- AI product explainers

Traits:

- modular blocks
- thick outlines
- pixel or dev-ish icon language
- hot pink / yellow / cyan systems

Good when the user wants:

- anti-corporate builder energy
- expressive system diagrams

## 3. Typography-led

### Mincho × Handwritten Mix

Best for:

- reflective essays
- cultural decks
- emotional but designed communication

Traits:

- serif + handwritten contrast
- literary feeling
- personal voice

Good when the user wants:

- softer humanity
- less corporate tone

## 4. Artistic & Avant-garde

### Deformed Flat Persona

Best for:

- concept storytelling
- art-driven presentations
- identity-heavy decks

### Royal Blue × Red Watercolor

Best for:

- visionary narratives
- culture or brand stories
- emotional interpretation

Traits:

- painterly texture
- controlled color drama

### Classic / Pop (Sculpture × Vaporwave)

Best for:

- experimental brand decks
- creative campaigns

### Tech / Art / Neon

Best for:

- edgy AI showcases
- art-tech launches
- visually aggressive future storytelling

Traits:

- neon glow
- dark stage
- high contrast

Use with caution:

- powerful for impact
- weak for sober enterprise clarity

## 5. Professional / Product / Premium

### Studio / Mockup / Premium

Best for:

- premium product decks
- SaaS positioning
- polished product marketing

Traits:

- glossy restraint
- high-end mockup feeling
- product-centered hero images

## 6. Sports & High-energy

### Sports / Athletic / Energy

Best for:

- campaign launches
- motivational decks
- performance storytelling

Traits:

- diagonal motion
- strong contrast
- headline-first pacing

## 7. How to Use This Catalog

When recommending three directions:

1. pick one from the core map that best serves the content goal
2. if useful, refine it with one of the style families in this file
3. keep the final recommendation understandable in plain language

Example:

- not just “Sharp-edged Minimalism”
- instead: “偏高端极简的网格式商业风，接近 sharp-edged minimalism”

## 8. YAML Translation Advice

Many styles in the public prompt library already lean YAML-like.

When converting one of these styles into the final output:

- keep the style family name in a human-readable field
- translate visual traits into reusable YAML keys
- do not dump a raw copied prompt
- rewrite it to fit the user's content, audience, and colors

Good fields to fill:

- `style.direction`
- `style.reference_family`
- `style.mood`
- `style.color_palette`
- `layout.composition`
- `visuals.preferred`
- `rules`
- `avoid`
