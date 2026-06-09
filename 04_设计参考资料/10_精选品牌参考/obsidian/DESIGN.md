# DESIGN.md

Name: Obsidian-inspired Knowledge UI
Status: Community reconstructed (not official)
Source: Public pages from obsidian.md and brand assets

## 1) Visual Theme & Atmosphere
- Product type: PKM / knowledge base / notes workflow
- Overall mood: calm, focused, private, low-noise
- Design direction: soft-dark surfaces with clear reading hierarchy
- Density: medium for app UI, relaxed for long-form content

## 2) Color Palette & Roles
Primary:
- Obsidian Purple 500: #A88BFA
- Obsidian Purple 700: #6C31E3

Neutrals:
- Background Dark: #111827
- Surface Dark: #1F2937
- Surface Subtle: #374151
- Border Dark: #4B5563
- Text Primary: #F3F4F6
- Text Secondary: #D1D5DB
- Text Muted: #9CA3AF

Semantic:
- Success: #22C55E
- Success Deep: #16A34A
- Warning: #FEBC2E
- Danger: #DC2626

Guidelines:
- Purple is accent, not flood-fill.
- Keep large reading areas low contrast but text high contrast.
- Use semantic colors only for state communication.

## 3) Typography Rules
- Primary font: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial
- Mono font: ui-monospace, SFMono-Regular, Menlo, Consolas, monospace

Scale:
- H1: 32/700/1.2
- H2: 24/650/1.25
- H3: 20/600/1.3
- Body L: 16/400/1.7
- Body M: 14/400/1.65
- Caption: 12/500/1.5
- Code Inline: 13/500/1.5 (mono)

## 4) Component Stylings
Buttons:
- Primary: purple fill, white text, radius 10
- Secondary: subtle dark surface, border 1px, muted text
- Ghost: transparent, hover tint only

Inputs:
- Background dark-surface
- Border 1px neutral
- Focus ring: 2px purple glow
- Error: red border + helper text

Cards / Note blocks:
- Surface dark + thin border
- Radius 12
- Optional subtle shadow only when elevated actions appear

Navigation:
- Left sidebar, collapsed/expanded states
- Active item: purple left indicator + stronger text
- Hover: subtle background tint

## 5) Layout Principles
- Layout: sidebar + content + optional right context pane
- Content width: 720-840 for reading mode
- Spacing scale: 4, 8, 12, 16, 24, 32, 48
- Rhythm: larger gaps between sections, tighter gaps inside cards

## 6) Depth & Elevation
- Level 0: flat reading canvas
- Level 1: panel borders only
- Level 2: modal and command palette with soft shadow
- Avoid heavy blur and oversized shadow stacks

## 7) Do / Don't
Do:
- Prioritize readability and note-flow continuity
- Keep accent color sparse and meaningful
- Use keyboard-first affordances in tool-heavy views

Don't:
- Overuse gradients in content areas
- Mix many accent colors in one screen
- Make navigation visually louder than note content

## 8) Responsive Behavior
- Mobile first for capture and quick edit
- Breakpoints:
  - < 768: single column, sidebar as drawer
  - 768-1200: sidebar + content
  - > 1200: add right context panel
- Touch targets: minimum 40x40

## 9) Agent Prompt Guide
Quick prompt:
- Build a knowledge app UI in an Obsidian-inspired style.
- Use soft dark surfaces, sparse purple accents, high readability, and sidebar-first navigation.
- Keep typography comfortable for long-form reading.

Strict prompt:
- Follow DESIGN.md tokens exactly.
- No extra accent colors.
- Prioritize note content over decorative visuals.
- Implement full component states for buttons, inputs, and nav items.
