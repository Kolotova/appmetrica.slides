---
name: Deep Space Metrics
colors:
  surface: '#11131a'
  surface-dim: '#11131a'
  surface-bright: '#373940'
  surface-container-lowest: '#0c0e14'
  surface-container-low: '#191b22'
  surface-container: '#1d1f26'
  surface-container-high: '#272a31'
  surface-container-highest: '#32353c'
  on-surface: '#e1e2eb'
  on-surface-variant: '#c2c6d5'
  inverse-surface: '#e1e2eb'
  inverse-on-surface: '#2e3037'
  outline: '#8c909f'
  outline-variant: '#424753'
  surface-tint: '#afc6ff'
  primary: '#afc6ff'
  on-primary: '#002d6c'
  primary-container: '#538dfd'
  on-primary-container: '#00275f'
  inverse-primary: '#0059c6'
  secondary: '#ffb0c9'
  on-secondary: '#650034'
  secondary-container: '#c2006a'
  on-secondary-container: '#ffd6e0'
  tertiary: '#d0bcff'
  on-tertiary: '#3c0091'
  tertiary-container: '#a078ff'
  on-tertiary-container: '#340080'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d9e2ff'
  primary-fixed-dim: '#afc6ff'
  on-primary-fixed: '#001a43'
  on-primary-fixed-variant: '#004398'
  secondary-fixed: '#ffd9e3'
  secondary-fixed-dim: '#ffb0c9'
  on-secondary-fixed: '#3e001e'
  on-secondary-fixed-variant: '#8e004c'
  tertiary-fixed: '#e9ddff'
  tertiary-fixed-dim: '#d0bcff'
  on-tertiary-fixed: '#23005c'
  on-tertiary-fixed-variant: '#5600ca'
  background: '#11131a'
  on-background: '#e1e2eb'
  surface-variant: '#32353c'
typography:
  display-xl:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: '800'
    lineHeight: 72px
    letterSpacing: -0.02em
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  number-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1440px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
  stack-xl: 64px
---

## Brand & Style

The brand personality is authoritative, technical, and high-end. It is designed for data analysts, product managers, and C-suite executives who require clarity in complex datasets. The UI evokes a sense of "command and control" through a dark, cinematic atmosphere.

The design style is **Corporate Modern** with **Minimalist** leanings. It prioritizes information density and structural clarity. The visual language is defined by large-scale containers, deep tonal layering, and vibrant accent pops that guide the eye toward key conversion points and data highlights. The aesthetic avoids all representational imagery (photos/emojis) in favor of abstract geometry and functional iconography.

## Colors

The palette is rooted in a "Deep Night" spectrum. The background uses a near-black navy to provide maximum contrast for text and vibrant accents. 

- **Backgrounds:** Use `#0E121A` for the main canvas.
- **Surfaces:** Use `#191E28` for primary content cards. Use `#202635` for interactive hover states or secondary nested containers.
- **Accents:** Use Blue for primary actions, Pink for secondary highlights or "Pro" features, and Purple for premium tiers or specialized data streams.
- **Functional:** Dividers must remain subtle at `#303849` to maintain the 16:9 layout structure without breaking the visual flow.

## Typography

The typography system relies on **Inter** for its neutral, technical precision. 

- **Headlines:** Use Extra-bold weights for display sizes to create a strong visual anchor.
- **Numerical Data:** All numbers must use **Tabular Figures** (`tnum`) to ensure columns of data align perfectly in dashboards and pricing tables.
- **Hierarchy:** Use secondary text colors (`#AEB7C8`) for body descriptions to maintain a clear visual dip between headings and supporting content.
- **Mobile Scaling:** For mobile devices, `display-xl` should scale down to `headline-lg` (32px) to ensure readability without excessive horizontal scrolling.

## Layout & Spacing

The system uses a **12-column fluid grid** with a fixed maximum width for desktop to maintain the 16:9 cinematic presentation feel. 

- **Rhythm:** A base-8 scale drives all spacing. 
- **Grid:** Desktop utilizes 24px gutters with 64px side margins to allow the content to "breathe." 
- **Reflow:** On Tablet (768px - 1024px), margins reduce to 32px. On Mobile, the grid collapses to 4 columns with 20px margins.
- **Containers:** Content is grouped into logical cards that span specific column counts (e.g., 3 cards spanning 4 columns each in a row).

## Elevation & Depth

Hierarchy is established through **Tonal Layering** and **Subtle Outlines** rather than traditional shadows.

- **Level 0:** Background (`#0E121A`) is the lowest point.
- **Level 1:** Content cards (`#191E28`) sit above the background. They do not use shadows; instead, they are defined by their contrast and a 1px border of `#303849` or a subtle inner glow.
- **Level 2:** Interactive elements like dropdowns and tooltips use the Secondary Surface (`#202635`) with a slight ambient shadow (0px 8px 24px rgba(0,0,0,0.4)) to separate them from the content layer.
- **Active States:** Elements being interacted with may use a 1px solid stroke of the Accent Blue to indicate focus.

## Shapes

The design system uses an exaggerated roundedness for large containers to soften the technical nature of the data. 

- **Primary Cards:** Use a radius of **32px** (variable between 28-36px depending on size).
- **Interactive Elements:** Buttons and inputs use a more functional **8px to 12px** radius to maintain a professional "tool" aesthetic.
- **Badges:** Small utility labels or badges use a fully rounded "pill" shape.

## Components

### Buttons
- **Primary:** Solid `#4D88F7` with white text. High-contrast.
- **Secondary:** Ghost style with `#303849` border and `#FFFFFF` text.
- **Tertiary:** Text-only with an trailing arrow icon.

### Cards
- Large `32px` radius. 
- Padding should be generous (typically 40px internal padding for display cards).
- Feature cards can use top-weighted accent gradients (Blue to Purple) for visual distinction.

### Inputs & Selects
- Background: `#191E28`.
- Border: 1px `#303849`.
- Font: Tabular figures for any numerical inputs.
- Icons: Use simple 2px stroke line icons centered vertically.

### Badges & Chips
- Muted background (`#8495C4` at 10-20% opacity).
- Text color matches the badge's respective accent (Blue, Pink, or Purple).

### Lists
- Use horizontal dividers (`#303849`) between items.
- Ensure 24px vertical padding per list item to maintain the "spacious" layout requirement.

### Iconography
- 24px bounding box.
- 2px stroke weight.
- Round caps and joins.
- Strict monochrome or single-accent usage.