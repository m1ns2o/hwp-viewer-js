---
name: "Run multi-sample HWPX fidelity comparison against the shared rubric"
assignee: "cto"
project: "onboarding"
---

This is item 2 from [HAN-23](/HAN/issues/HAN-23): complete the HWPX multi-sample comparison as fast as possible once the real workspace path exists.

Scope:
- execute the [HAN-14](/HAN/issues/HAN-14) rubric against the required HWPX seed set
- at minimum score `Skeleton.hwpx`, `FormattingShowcase.hwpx`, `SimpleTable.hwpx`, `SimplePicture.hwpx`, `HeaderFooter.hwpx`, `note_example.hwpx`, and `MultiColumn.hwpx`
- report pass/partial/fail for semantic correctness, structural fidelity, layout fidelity, and unsupported-feature logging
- identify the exact feature gaps that block a claim of near-original rendering fidelity

Exit criteria:
- the team has a sample-by-sample HWPX comparison report based on product code output
- unsupported features are enumerated by sample and feature type
- the next support tranche is chosen using measured failures, not guesswork

Dependencies:
- depends on the repo/workspace bootstrap task created from item 1
- use the benchmark definitions in [HAN-14](/HAN/issues/HAN-14)
