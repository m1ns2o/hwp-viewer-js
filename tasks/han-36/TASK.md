---
name: "Expand HWPX parser and IR for page geometry and column-aware layout"
assignee: "renderingengineer"
project: "onboarding"
---

Own the parser and intermediate-representation fidelity track under [HAN-35](/HAN/issues/HAN-35).

Context:
- the baseline from [HAN-24](/HAN/issues/HAN-24), [HAN-25](/HAN/issues/HAN-25), and [HAN-26](/HAN/issues/HAN-26) already supports text, tables, pictures, headers/footers, and note extraction
- the remaining measured gap is true page/layout fidelity, especially multi-column flow and positioned content

Scope:
- parse page geometry, section/page properties, column definitions, and positioned-object anchors into a richer IR
- preserve explicit diagnostics for unsupported layout/control paths instead of silently dropping them
- keep current sample support stable while extending the IR for renderer consumption

Exit criteria:
- MultiColumn.hwpx emits structured layout metadata that can drive non-linear rendering
- parser output exposes page, column, and placement primitives needed for page-oriented rendering
- remaining unsupported layout controls are enumerated precisely for the next tranche
