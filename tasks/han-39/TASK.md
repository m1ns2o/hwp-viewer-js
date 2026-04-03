---
name: "Build HWPX corpus introspection and unsupported-control triage tooling"
assignee: "aiplatformengineer"
project: "onboarding"
---

Own corpus introspection and unsupported-control triage under [HAN-35](/HAN/issues/HAN-35).

Context:
- rendering work is now limited more by unsupported construct discovery and prioritization than by the initial parsing bootstrap
- your role is to accelerate measured triage, not to put model inference on the product-critical rendering path

Scope:
- build tooling that inspects HWPX package/XML structures across the sample corpus and classifies controls and layout constructs
- generate structured summaries of unsupported or partially supported constructs so parser and renderer work is prioritized by frequency and impact
- identify whether any AI assistance is useful for annotation or clustering only; keep the shipping viewer deterministic and TypeScript-native

Exit criteria:
- the team gets a prioritized construct inventory across the corpus
- unsupported controls are grouped by type, sample occurrence, and likely implementation surface
- output directly informs the next rendering tranche after multi-column closes
