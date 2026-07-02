# Responsive Layout Validation Guidelines

Always validate all layout and design changes using the following reference viewports:

## Target Viewports
- **Mobile**
  - Android: 360 × 800 px
  - iPhone: 390 × 844 px
- **Tablet**
  - 768 × 1024 px
- **Desktop**
  - Notebook (Primary Base): 1366 × 768 px
  - Desktop Full HD: 1920 × 1080 px

## Validation Requirements
- Use **1366 × 768 px** as the primary design reference for notebook bases.
- Ensure browser viewport variations (interface overlays, address bars) are accounted for.
- The composition must remain consistent across all viewports, strictly avoiding:
  - Image cropping/clipping issues.
  - Text and image overlapping.
  - Horizontal scrolling (overflow-x).
  - Sudden or jarring proportion shifts.
  - Typographic hierarchy degradation.

## Stacking & Scaling Philosophy
- Prioritize **1366 × 768 px (Notebook)** as the primary design layout base, especially for the Hero composition.
- All other breakpoints must adapt from this base structure dynamically, without breaking the visual narrative or hierarchy.
- Avoid single-breakpoint specific fixes (e.g., ad-hoc adjustments only for 1920px or only for iPad) unless absolutely necessary.
- Rely on responsive, fluid math (e.g., clamp, percentages, aspect-ratio, vw/vh) to ensure a single, clean layout engine scales consistently across Desktop, Tablet, and Mobile.

## Composition & Code Integrity Guidelines
- **Composition Over Exact Position**: Focus on maintaining visual hierarchy, balance (text vs. space vs. imagery), and reading flow rather than absolute pixel matching across different screens.
- **D.R.Y. CSS (Don't Repeat Yourself)**: Before writing new CSS rules or media queries, inspect existing stylesheets for rules that can be reused, refactored, or slightly adjusted. Avoid duplicate style declarations and redundant overrides.
- **Clean & Scalable Code**: Prioritize clean, readable, and highly maintainable stylesheets with logical naming conventions.
