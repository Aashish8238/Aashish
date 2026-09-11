---
name: Obsidian Engineering Console
colors:
  surface: '#10141a'
  surface-dim: '#10141a'
  surface-bright: '#353940'
  surface-container-lowest: '#0a0e14'
  surface-container-low: '#181c22'
  surface-container: '#1c2026'
  surface-container-high: '#262a31'
  surface-container-highest: '#31353c'
  on-surface: '#dfe2eb'
  on-surface-variant: '#bcc9cd'
  inverse-surface: '#dfe2eb'
  inverse-on-surface: '#2d3137'
  outline: '#869397'
  outline-variant: '#3d494c'
  surface-tint: '#4cd7f6'
  primary: '#4cd7f6'
  on-primary: '#003640'
  primary-container: '#06b6d4'
  on-primary-container: '#00424f'
  inverse-primary: '#00687a'
  secondary: '#4edea3'
  on-secondary: '#003824'
  secondary-container: '#00a572'
  on-secondary-container: '#00311f'
  tertiary: '#7bd0ff'
  on-tertiary: '#00354a'
  tertiary-container: '#23b2ec'
  on-tertiary-container: '#00415a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#acedff'
  primary-fixed-dim: '#4cd7f6'
  on-primary-fixed: '#001f26'
  on-primary-fixed-variant: '#004e5c'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#c4e7ff'
  tertiary-fixed-dim: '#7bd0ff'
  on-tertiary-fixed: '#001e2c'
  on-tertiary-fixed-variant: '#004c69'
  background: '#10141a'
  on-background: '#dfe2eb'
  surface-variant: '#31353c'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '600'
    lineHeight: 44px
    letterSpacing: -0.025em
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 26px
    letterSpacing: -0.015em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: -0.005em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: 0em
  code-md:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: -0.01em
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0em
  badge-label:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.04em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  px: 1px
  xs: 0.25rem
  sm: 0.5rem
  md: 0.75rem
  base: 1rem
  lg: 1.5rem
  xl: 2rem
  2xl: 3rem
  gutter: 1rem
  margin-mobile: 1rem
  margin-desktop: 1.5rem
---

## Brand & Style
This design system embodies a high-performance, developer-first aesthetic inspired by elite engineering environments like Vercel and GitHub. The visual tone is precise, utilitarian, and focused. It prioritizes information density, crisp functional contrast, and low optical fatigue for prolonged technical workflows. 

The aesthetic is anchored in modern minimalist-technical styling: deep obsidian and charcoal layers, hairline borders, and targeted luminescent accents. Visual noise is aggressively eliminated, allowing real-time metrics, deployment logs, and syntax structures to take absolute visual priority.

## Colors
The palette relies on deep architectural dark tones structured to provide clear container hierarchy without harsh contrast jumps:
- **Canvas Base:** `#0a0c10` (Primary application backdrop)
- **Surface Level 1:** `#0d1117` (Cards, sidebars, panel containers)
- **Surface Level 2:** `#161b22` (Sub-cards, tables, nested modules, interactive elements)
- **Surface Level 3 / Hover:** `#21262d` (Active states, elevated popovers)
- **Structural Outlines:** `#30363d` (Hairline perimeter strokes and divider rules)

Accents are strictly functional:
- **Primary Accent (`#06b6d4`):** Focused states, primary triggers, and core interactive workflows.
- **Success / Healthy Accent (`#10b981`):** Operational deployment indicators, successful run outputs, and healthy telemetry.
- **Info / Analytics Accent (`#38bdf8`):** Network metrics, streaming data, and real-time logs.
- **Text & Foreground Hierarchy:** Pure White (`#f0f6fc`) for active headers, muted slate (`#8b949e`) for secondary annotations, and dark muted (`#484f58`) for disabled or trailing indicators.

## Typography
Typographic scale uses `Inter` for functional narrative readability and UI layout control, paired with `JetBrains Mono` for data tables, metrics, inline terminal outputs, and metadata chips. 

- Headings use tight negative letter-spacing for high-density modern impact.
- Body copy maintains disciplined vertical line rhythm aligned with code height standards.
- All numbers, performance metrics, commit hashes, and status chips strictly use monospace numerals (`tabular-nums` via `JetBrains Mono`) to avoid layout jitter during real-time streaming updates.

## Layout & Spacing
The layout follows a fluid-responsive grid system designed for data density:
- **Structure:** 12-column grid layout with nested dashboard split-views (collapsible left-hand navigation, flexible telemetry body, contextual right-hand inspector panel).
- **Margins & Gutters:** 16px margins on mobile/tablet expanding to 24px on desktop; uniform 16px gutters between data panels.
- **Reflow Rules:**
  - **Desktop (>= 1280px):** 3-column architecture (Navigation: 240px fixed, Main Console: fluid, Telemetry/Inspector: 360px fixed).
  - **Tablet (768px - 1279px):** Inspector collapses to an off-canvas drawer; main grid compresses to single or dual-column blocks.
  - **Mobile (< 768px):** Navigation collapses to a top command-bar drawer; all metric and log panels stack vertically into a single-column flow with full-bleed touch targets.

## Elevation & Depth
Depth in this design system is engineered via tonal stacking and hairline borders rather than heavy diffuse drop-shadows.

- **Surface Tiers:** Level 0 (`#0a0c10`) functions as the base canvas. Floating panels and dashboard sections sit at Level 1 (`#0d1117`), while inner controls, table headers, and modules rest at Level 2 (`#161b22`).
- **Hairline Borders:** All structural boundaries use a clean 1px border (`#30363d`), creating high-definition definition without visual bulk.
- **Micro Ambient Lighting:** Popovers, contextual menus, and floating modals use a subtle, directional drop-shadow tinted with base charcoal: `0 8px 24px rgba(1, 4, 9, 0.85)`, enclosed with a brightened hairline border (`#38424d`).
- **Active Glow:** Focused inputs and active terminal buffers project an intentional, tight neon perimeter bleed (`0 0 0 1px #06b6d4, 0 0 12px rgba(6, 182, 212, 0.2)`).

## Shapes
The system relies on crisp, compact corner radii to preserve an engineered, instrumentation-grade feel:
- Base inputs, buttons, and status tags apply `rounded` (4px / 0.25rem).
- Metric modules, cards, and modal dialogs use `rounded-lg` (8px / 0.5rem).
- Status pulse indicators and avatar nodes use fully rounded circular geometries (`rounded-full`).
- Pill shapes are strictly avoided for actionable buttons to maintain an architectural, technical precision across the viewport.

## Components

### Buttons
- **Primary:** Background `#06b6d4`, foreground `#0a0c10`, font `Inter` semibold 13px. Hover: `#22d3ee`. Active: scale 0.98.
- **Secondary / Ghost:** Background `#21262d`, border 1px solid `#30363d`, foreground `#f0f6fc`. Hover: background `#30363d`, border `#8b949e`.
- **Destructive:** Background `rgba(248, 81, 73, 0.1)`, border 1px solid `rgba(248, 81, 73, 0.4)`, text `#f85149`.

### Chips & Badges
- Built exclusively with `JetBrains Mono` at 10px uppercase with `0.04em` letter-spacing.
- Height: 20px, inline padding: 6px.
- **Success Chip:** Background `rgba(16, 185, 129, 0.12)`, border 1px solid `rgba(16, 185, 129, 0.35)`, text `#10b981`. Features a 6px static or pulsing circle icon.
- **Metric Chip:** Background `#161b22`, border 1px solid `#30363d`, text `#8b949e`.

### Inputs & Terminal Command Fields
- Background `#0a0c10`, border 1px solid `#30363d`, text `#f0f6fc`.
- Padding: 8px 12px. Font: `JetBrains Mono` 13px.
- Focus state: border `#06b6d4`, subtle cyan rim shadow (`0 0 0 1px #06b6d4`).

### Cards & Telemetry Panels
- Surface `#0d1117`, border 1px solid `#30363d`, corner radius 8px.
- Card headers feature an explicit bottom divider stroke (`#21262d`) with uppercase tracking labels.
- Interactive cards feature an edge-highlight hover state transitioning border color to `#484f58`.

### Lists & Data Tables
- Row height: 36px (compact) or 44px (default).
- Separators: 1px border-bottom `#21262d`.
- Table header: Font `JetBrains Mono` 11px uppercase, background `#161b22`, text `#8b949e`.
- Hover state: Background `#161b22` transition over 120ms ease.

### Checkboxes & Switches
- Checkboxes: 16x16px square, radius 3px, border 1px solid `#30363d`, background `#0a0c10`. Checked: background `#06b6d4` with dark vector checkmark.
- Switches: Track 32x18px, border 1px solid `#30363d`, thumb 12x12px solid `#f0f6fc`. Active track `#10b981`.

### Code Blocks & Console Drawers
- Embedded terminal panels utilizing `#05070a` absolute-dark canvas.
- Syntax elements tinted with Cyan (`#38bdf8`), Emerald (`#10b981`), Amber (`#fbbf24`), and Violet (`#a78bfa`).
- Integrated top metadata bar with branch name, commit sha chip, and one-click copy button.