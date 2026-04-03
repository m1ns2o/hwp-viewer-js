---
name: "Implement the first HWPX layout support tranche for near-original rendering"
assignee: "cto"
project: "onboarding"
---

This is item 3 from [HAN-23](/HAN/issues/HAN-23): complete the first layout-support expansion as fast as possible after measured comparison results arrive.

Scope:
- implement the first renderer support tranche driven by failures from the comparison task
- expected initial focus order: tables, images, header/footer, footnotes/endnotes, then multi-column fallback
- keep unsupported constructs explicitly logged instead of silently dropped
- preserve the browser-first TypeScript architecture defined in [HAN-8](/HAN/issues/HAN-8)

Exit criteria:
- the highest-value missing constructs from the comparison run are supported or deliberately deferred with logging
- fidelity materially improves on the benchmark set for the targeted constructs
- remaining blockers to near-original HWPX rendering are reduced to a smaller, explicit list

Dependencies:
- depends on item 2 comparison results
- should reuse the product code baseline from the item 1 bootstrap task
