---
name: Canary Operational Utility
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#4b4732'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#7d775f'
  outline-variant: '#cec7ab'
  surface-tint: '#6b5f00'
  primary: '#6b5f00'
  on-primary: '#ffffff'
  primary-container: '#fbe106'
  on-primary-container: '#706300'
  inverse-primary: '#dfc700'
  secondary: '#5f5e5f'
  on-secondary: '#ffffff'
  secondary-container: '#e2dfe0'
  on-secondary-container: '#636263'
  tertiary: '#00696d'
  on-tertiary: '#ffffff'
  tertiary-container: '#34f7ff'
  on-tertiary-container: '#006e72'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#fee40e'
  primary-fixed-dim: '#dfc700'
  on-primary-fixed: '#201c00'
  on-primary-fixed-variant: '#504700'
  secondary-fixed: '#e5e2e3'
  secondary-fixed-dim: '#c8c6c7'
  on-secondary-fixed: '#1b1b1c'
  on-secondary-fixed-variant: '#474647'
  tertiary-fixed: '#58f8ff'
  tertiary-fixed-dim: '#00dce3'
  on-tertiary-fixed: '#002021'
  on-tertiary-fixed-variant: '#004f52'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono-data:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 12px
  margin-safe: 24px
---

## Brand & Style
The design system is engineered for high-density, technical environments where speed of information processing is paramount. It follows a **Modern Corporate** aesthetic with a lean toward **Systematic Minimalism**. The brand personality is deterministic and operational, prioritizing utility over decoration.

The UI should evoke a sense of professional calm and precision. It avoids "marketing fluff," opting instead for a tool-like interface that feels like a natural extension of a developer or analyst's workflow. Visual depth is minimal, relying on subtle tonal shifts and precise borders rather than heavy shadows or gradients.

## Colors
The palette is centered around a "Canary" yellow, used strictly for primary actions, critical focus states, and specific warning indicators. 

- **Primary:** Canary Yellow (#FBE106) is high-visibility. Use it for the most important button on a screen or to highlight active tool states.
- **Neutrals:** A range of cool grays and off-whites provides the foundation. Surface colors use slight shifts in value to denote hierarchy.
- **Semantics:** Health and risk are conveyed through a robust three-tier system. Green signifies stable/healthy, Amber (distinct from Canary) for warnings, and Red for critical failures.
- **Contrast:** Text must maintain a minimum 4.5:1 ratio against backgrounds to ensure legibility in high-density data views.

## Typography
This design system utilizes **Inter** for its neutral, systematic clarity. A tight type scale is employed to maximize data density without sacrificing readability.

- **Data Presentation:** Use `mono-data` (JetBrains Mono) for all technical values, IDs, and timestamps to ensure character alignment and a technical feel.
- **Hierarchy:** Use `label-caps` for section headers within sidebars or small card titles to create clear structural anchors.
- **Weight:** Bold weights are reserved for interactive elements and primary headers; body text remains at regular weight to prevent visual clutter in dense tables.

## Layout & Spacing
The layout follows a **Fluid Grid** model designed for browser-based dashboards. It uses a 4px baseline grid to maintain rigorous alignment.

- **Density:** Components use "compact" padding (8px internal) by default.
- **Grid:** A 12-column layout is used for primary dashboard views, with 12px gutters.
- **Reflow:** On mobile devices, columns stack vertically, and horizontal margins reduce to 16px. Technical tables should transition to a "pinned column" or "card-list" format on smaller screens.
- **Containers:** Content is typically housed in bordered containers rather than floating freely, reinforcing the "instrument panel" aesthetic.

## Elevation & Depth
Depth is communicated through **Tonal Layers** and **Low-Contrast Outlines** rather than traditional shadows.

- **Levels:** The canvas is the lowest level (`#F8FAFC`). Surfaces like cards and sidebars sit on top (`#FFFFFF`).
- **Borders:** Every container must have a 1px solid border (`#E2E8F0`). 
- **Active State:** To show elevation or focus, use a 1px border of a darker gray or a subtle inner glow, rather than a drop shadow.
- **Overlays:** Modals or dropdowns use a very soft, high-diffusion shadow (0px 4px 12px rgba(0,0,0,0.05)) to separate them from the underlying data layer.

## Shapes
The design system uses a **Soft** shape language to balance professional rigidity with modern UI sensibilities.

- **Components:** Buttons, inputs, and small chips use a 4px (`0.25rem`) corner radius.
- **Containers:** Larger cards and panels use an 8px (`0.5rem`) corner radius.
- **Icons:** Use square-proportioned icons with a 1.5px or 2px stroke weight to match the technical aesthetic.

## Components

- **Buttons:** Primary buttons use Canary Yellow with black text. Secondary buttons use a white background with a gray border. Success/Error actions use their respective semantic colors but only for text/outlines unless the action is destructive.
- **Inputs:** Fields are rectangular with a 1px border. On focus, the border changes to a dark neutral (not yellow) to avoid visual fatigue, with a subtle yellow "tick" indicator.
- **Chips/Status:** Use "Status Dots" (small 8px circles) next to text labels to indicate health. Background tints for chips should be very desaturated (e.g., 10% opacity of the semantic color).
- **Data Tables:** High-density with 8px vertical cell padding. Header rows use a light gray background (`#F1F5F9`) and `label-caps` typography.
- **Cards:** White background, 1px border, no shadow. Headers within cards should be separated by a 1px horizontal rule.
- **Monochromatic Icons:** Icons should be a single color (Neutral-600). Use color only to denote a change in status (e.g., a "Sync" icon turning green when successful).