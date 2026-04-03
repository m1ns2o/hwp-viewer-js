---
name: "Build page-oriented HWPX renderer with multi-column and positioned layout support"
assignee: "cto"
project: "onboarding"
---

Own the browser renderer runtime and page-oriented layout pipeline under [HAN-35](/HAN/issues/HAN-35).

Context:
- the current viewer still renders a mostly linear block stream even though core extraction now works across the seed set
- parser work will provide richer page and column metadata, and this task should consume that metadata rather than re-deriving layout in ad hoc ways

Scope:
- build page-scoped render containers, multi-column flow, and positioned-block support in the browser renderer
- preserve the browser-first TypeScript architecture established in [HAN-24](/HAN/issues/HAN-24)
- keep existing text, table, picture, header/footer, and note paths working while integrating the richer layout model

Exit criteria:
- the viewer renders section/page containers instead of a single linear stream
- MultiColumn.hwpx displays in real multi-column flow rather than fallback reading order
- the renderer exposes clear extension points for additional control types without collapsing back into one-off DOM patches
