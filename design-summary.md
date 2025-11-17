# Portfolio Page - Design & CSS Summary

## Layout Architecture
- **Flexbox-based structure** with nested containers
- Parent container (`.fullProject`): Column layout for vertical stacking
- Child container (`.projects`): Row layout for horizontal card arrangement
- Two-tier flex system for organized content hierarchy

## Spacing Strategy
- **Inter-card spacing:** 2rem (32px) gap between cards
  - Creates visual separation without feeling cramped
  - Consistent in all directions (horizontal & vertical when wrapped)
- **Page margins:** 2rem padding on main container
  - Prevents content from touching viewport edges
  - Maintains breathing room across all screen sizes

## Alignment & Centering
- **Horizontal centering:** `justify-content: center` on cards container
  - Cards centered regardless of quantity or screen size
  - Works for both single-row and multi-row layouts
- Content naturally flows from center outward

## Responsive Behavior
- **`flex-wrap: wrap`** enables mobile-friendly layout
  - Cards stack vertically on narrow screens
  - Automatically adjusts to available width
  - Maintains center alignment during reflow
- No media queries needed - fluid by default

## CSS Approach
- **Bare CSS** for layout logic (flex, gap, padding, justify-content)
- **DaisyUI classes** for component styling (card, btn, shadow)
- **Tailwind utilities** for quick styling (w-48, bg-base-100)
- Hybrid approach: structural CSS + utility classes

## Component Design
- **DaisyUI cards** with consistent 192px width (w-48)
- Card structure: figure + body + actions
- Subtle shadows for depth (shadow-sm)
- Primary color button for CTAs

## Color & Theming
- Aqua background on main container
- DaisyUI base colors (bg-base-100) for cards
- Semantic color system via DaisyUI themes

## Technical Decisions
- CDN delivery for zero build setup
- Browser-based Tailwind processing (v4)
- Inline + style tag CSS for simplicity
- rem units for scalable, accessible spacing
