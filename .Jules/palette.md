## 2026-03-06 - Quarto Dark Mode Accessibility
**Learning:** Quarto books don't include dark mode by default when using a single theme. Adding a light/dark theme pair in `_quarto.yml` automatically provides a color scheme toggle with proper ARIA labels, significantly improving accessibility for users with light sensitivity without needing custom code.
**Action:** Always check `_quarto.yml` format.html.theme for a light/dark configuration to ensure native dark mode support in Quarto docs.
