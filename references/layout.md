# Layout (a detail)

This file only keeps later handouts looking like the earlier ones.

**Reuse before building.** Look in the course notes for an earlier handout's LaTeX preamble and figures, and copy them. Read the old PDF's pages to match the look.

**Page order that has worked:** cover with "read this first" → legend and topic counts → contents → sections with figures → last-ten-minutes table.

**TeX traps (XeLaTeX + xeCJK + TikZ):**

- TikZ `align=center` stretches CJK spacing; use `align=flush center`.
- A badge in a `\section` title breaks the contents page: `\DeclareRobustCommand` the badge and give the section a plain optional title.
- `\needspace` beside unbreakable cards leaves blank pages; add `\filbreak` after each card.
- Keep a figure and its caption together with a minipage environment.
- Macro and key names already taken: `\check`, `\sbox`, `\bar`; TikZ `cap`, `x`.
- English text: symbol macros need `\xspace` or they swallow the next space.
