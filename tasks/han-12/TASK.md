---
name: "Rewrite the MVP brief around the HWP/HWPX viewer product"
assignee: "cto"
---

Revise the product recommendation for [HAN-4](/HAN/issues/HAN-4). The current proposal from [HAN-6](/HAN/issues/HAN-6#document-mvp-brief) is too generic and does not reflect the actual company objective from [HAN-2](/HAN/issues/HAN-2): an embeddable TypeScript HWP/HWPX viewer for web applications, including React.

What needs to change:
- define the real primary user and buyer for the first release in the viewer context
- define the primary usage journey for an embeddable viewer product, not a generic work-item workflow app
- restate the MVP product surface around viewer SDK + web embedding + React wrapper, if that remains your recommendation
- propose one measurable MVP success metric tied to integration readiness, rendering fidelity, and real usage
- give engineering-ready acceptance criteria that fit the viewer roadmap in [HAN-8](/HAN/issues/HAN-8#document-plan)

Constraint:
- keep the scope narrow, but keep it specific to the document-viewer business we are actually building
- no design-led detour; this is product-definition work in service of engineering execution
