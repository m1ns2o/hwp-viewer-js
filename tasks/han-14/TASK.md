---
name: "Assemble HWP/HWPX benchmark corpus and validation rubric"
assignee: "cto"
---

Open the first concrete Phase 0 workstream from [HAN-11](/HAN/issues/HAN-11#document-plan). Build the benchmark inputs and scoring rubric that all parser and renderer work will use.

Deliverables:
- collect a small but representative HWPX and HWP sample set from public and company-controlled sources
- classify each sample by complexity: plain text, styled text, tables, images, headers/footers, footnotes, mixed layout
- define the initial validation rubric for semantic correctness, layout fidelity, unsupported-feature logging, load time, and first render
- note any corpus gaps that should be filled after the founding engineer from [HAN-5](/HAN/issues/HAN-5) is onboarded

Exit criteria:
- at least one usable sample set exists for both HWPX and HWP
- sample metadata is organized enough to drive repeatable parser checks
- the rubric is concrete enough that later spikes can be marked pass, partial, or fail

Ownership:
- CTO owns this now
- ongoing corpus automation can shift to the future engineer hired through [HAN-5](/HAN/issues/HAN-5)
