## 2026-03-06 - Quarto Dark Mode Accessibility
**Learning:** Quarto books don't include dark mode by default when using a single theme. Adding a light/dark theme pair in `_quarto.yml` automatically provides a color scheme toggle with proper ARIA labels, significantly improving accessibility for users with light sensitivity without needing custom code.
**Action:** Always check `_quarto.yml` format.html.theme for a light/dark configuration to ensure native dark mode support in Quarto docs.

## 2026-03-08 - Quarto Reader Mode and Back-to-Top Navigation
**Learning:** Quarto offers native reader-mode and back-to-top-navigation features. Enabling `reader-mode: true` and `back-to-top-navigation: true` in `_quarto.yml` significantly improves reading experience and accessibility without needing any custom code or new dependencies.
**Action:** Enable these properties in Quarto projects to provide an accessible, low-cognitive-load reading interface.
