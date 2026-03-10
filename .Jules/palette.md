## 2026-03-06 - Quarto Dark Mode Accessibility
**Learning:** Quarto books don't include dark mode by default when using a single theme. Adding a light/dark theme pair in `_quarto.yml` automatically provides a color scheme toggle with proper ARIA labels, significantly improving accessibility for users with light sensitivity without needing custom code.
**Action:** Always check `_quarto.yml` format.html.theme for a light/dark configuration to ensure native dark mode support in Quarto docs.

## 2026-03-08 - Quarto Reader Mode and Back-to-Top Navigation
**Learning:** Quarto offers native reader-mode and back-to-top-navigation features. Enabling `reader-mode: true` and `back-to-top-navigation: true` in `_quarto.yml` significantly improves reading experience and accessibility without needing any custom code or new dependencies.
**Action:** Enable these properties in Quarto projects to provide an accessible, low-cognitive-load reading interface.

## 2026-03-09 - Exposing Quarto Formats for Accessibility
**Learning:** Quarto books may configure alternative accessible formats (like `epub`) without exposing them to users in the UI by default. EPubs offer superior accessibility for screen readers and customized reading experiences compared to PDFs or standard web pages.
**Action:** When a Quarto project has alternative formats like `epub` configured under `format:`, explicitly add them to the `downloads` array under the `book:` section in `_quarto.yml` (e.g., `downloads: [pdf, epub]`) so users can easily access and download these formats directly from the sidebar.

## 2026-03-10 - Explicit Document Language
**Learning:** Quarto builds default to omitting an explicit language definition if `lang` is not specified at the top level of `_quarto.yml`. This causes the generated `<html>` tags to lack a proper `lang` attribute, creating a WCAG accessibility issue for screen reader pronunciation mapping.
**Action:** Always verify `lang: <language-code>` is present in the root level of `_quarto.yml` files for improved screen reader support.
