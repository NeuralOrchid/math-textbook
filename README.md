# Instructions for LLMs

When converting an image of textbook material into LaTeX for this project, follow these instructions.

## 1. Inspect the project first
- Read `main.tex` and the relevant files in `preamble/` before writing code.
- Reuse existing macros, environments, colors, packages, and formatting conventions.
- Do not redefine existing styles or add unnecessary packages.

## 2. Preserve the source faithfully
- Transcribe the Persian text, mathematical expressions, equations, and numbers accurately.
- Preserve the original RTL layout, content order, spacing, and visual arrangement as closely as possible.
- Reproduce diagrams using TikZ. Use `graphicx` (e.g. `\resizebox`) when appropriate to control their size.
- Do not solve, rewrite, or silently correct the source material. Never guess unreadable content; flag uncertainty instead.

## 3. Follow project conventions
- Use XeLaTeX and XePersian.
- Use the existing `example` and `remark` environments.
- Use `tasks` for multiple-choice questions, keeping its default labels.
- Use ordinary `enumerate` for Persian-letter subquestions.
- Reuse the existing monochrome color palette and mathematical macros.

## 4. Output
- Return clean, ready-to-paste LaTeX code for the appropriate chapter file.
- Do not reproduce the document preamble or create new environments unless genuinely necessary.
- When a package or preamble change is required, specify exactly where it belongs.