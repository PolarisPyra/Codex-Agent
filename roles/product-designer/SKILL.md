---
name: product-designer
description: "Implement high-fidelity dark UI (Obsidian Void) and enforce design system standards."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Product Designer Skill

## When to Use
Use this skill when you need to:
- Build premium dark UI components based on the Obsidian Void aesthetic.
- Define or update design tokens (colors, typography, spacing).
- Ensure visual consistency and "backlit" depth across the application.
- Implement responsive layouts and glassmorphism effects.

## Core Design Tokens

### 1. Colors (The Void Palette)
- **Void Black**: `#040506` (Canvas ground state)
- **Deep Charcoal**: `#07080a` (Primary surface)
- **Graphite 700**: `#111214` (Raised surface)
- **Graphite 600**: `#1b1c1e` (Overlay surface/badges)
- **Ash 50**: `#e6e6e6` (Primary CTA background)
- **Snow**: `#ffffff` (Primary text/strokes)
- **Ember Red**: `#ff6363` (Status/Logo accent only)

### 2. Typography (Inter & GeistMono)
- **Display Headlines**: 56px–64px, negative tracking (-0.11em to -0.13em), line-height 1.0.
- **Body Text**: 16px, line-height 1.5, tracking 0.1px.
- **Micro Labels/Badges**: 11px–12px, positive tracking (+0.04em to +0.073em).
- **Code/Monospace**: GeistMono 10px–14px, tracking +0.017em to +0.05em.

### 3. Elevation & Shadows
- **Physically Pressable (Key Shadow)**: `rgba(0,0,0,0.4) 0px 1.5px 0.5px 2.5px, rgb(0,0,0) 0px 0px 0.5px 1px, rgba(0,0,0,0.25) 0px 2px 1px 1px inset, rgba(255,255,255,0.2) 0px 1px 1px 1px inset`.
- **Glass Panel**: `rgba(0,0,0,0.28) 0px 1.189px 2.377px 0px` with `backdrop-filter: blur(36px)`.

### 4. Spacing & Shapes
- **Base Unit**: 8px.
- **Card Radius**: 11px.
- **Modal Radius**: 16px.
- **Button Radius**: 8px.
- **Page Max-width**: 1200px.

## Component Specifications

- **Primary CTA**: Background `#e6e6e6`, text `#2f3031`, 8px radius. High contrast without pure white aggression.
- **Ghost Nav**: Transparent background, text `#9c9c9d`, hover to `#ffffff`. Recedes until interaction.
- **Feature Card**: Transparent background, 16px radius, 1px solid `#222225` border or layered inset shadows.
- **Atmosphere Backdrop**: Per-section `radial-gradient` at top-center (blue core `#043f96` or violet core `#523091`) at 0.7 opacity core.

## Do's and Don'ts
- **DO**: Use `#040506` for the page ground.
- **DO**: Maintain density through negative tracking on large type.
- **DO**: Use radial gradients for section transitions instead of flat dividers.
- **DON'T**: Use colored backgrounds for containers; stay within the neutral charcoal stack.
- **DON'T**: Use border-radius above 20px for non-circular elements.
- **DON'T**: Use chroma-heavy colors (red/blue) as primary fill colors.

## Prerequisites
- Familiarity with the "Obsidian Void" design language.
- CSS/Tailwind proficiency.

## Common commands
- `view_file DESIGN.md`

## Limitations
- Visual design is subjective; always verify with the user via `generate_image` or mockups.
- Avoid breaking the established "precision instrument" aesthetic with overly rounded forms.
