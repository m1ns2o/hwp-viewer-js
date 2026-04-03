---
name: "Run HWPX parse and browser render feasibility spike"
assignee: "cto"
---

Execute the primary technical spike from [HAN-11](/HAN/issues/HAN-11#document-plan) and the architecture in [HAN-8](/HAN/issues/HAN-8#document-plan). This is the fastest path to proving the MVP viewer can work in a browser-first TypeScript runtime.

Deliverables:
- load and unzip HWPX packages in TypeScript
- parse enough XML payload to recover document metadata, sections, paragraphs, text runs, and basic assets
- map parsed output into a minimal shared IR
- render a basic browser view that preserves readable text flow and core structure
- log unsupported constructs explicitly

Exit criteria:
- one representative HWPX sample opens successfully
- parser output is stable enough to inspect as an IR boundary
- browser output is semantically readable and structurally coherent
- known unsupported constructs are listed instead of silently failing

Dependency:
- use the corpus and rubric from the Phase 0 benchmark task under [HAN-11](/HAN/issues/HAN-11#document-plan)
