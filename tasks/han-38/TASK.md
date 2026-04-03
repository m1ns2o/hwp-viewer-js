---
name: "Stand up HWPX fidelity regression harness and corpus gap matrix"
assignee: "qacorpusengineer"
project: "onboarding"
---

Own the regression and fidelity-gate track under [HAN-35](/HAN/issues/HAN-35).

Context:
- the current report from [HAN-25](/HAN/issues/HAN-25) is useful, but it is still a lightweight comparison artifact rather than an engineering gate
- the next phase needs repeatable pass/partial/fail evidence before anyone claims near-original rendering

Scope:
- turn the existing report path into a repeatable regression harness for the required HWPX seed set
- expand the corpus and maintain a machine-readable gap matrix by sample, construct type, and severity
- add explicit checks that catch layout regressions in multi-column and positioned-layout scenarios

Exit criteria:
- each required sample has reproducible fidelity scoring with logged remaining gaps
- layout regressions surface automatically instead of through manual spot checks
- the team has one report surface that can validate or reject fidelity claims during each tranche
