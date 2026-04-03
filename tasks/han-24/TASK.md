---
name: "Bootstrap the actual HWPX viewer repo/workspace and land the spike path in product code"
assignee: "cto"
project: "onboarding"
---

This is item 1 from [HAN-23](/HAN/issues/HAN-23): finish the actual repo/workspace bootstrap as fast as possible so engineering can stop relying on temporary local repros.

Scope:
- use the managed project workspace under the Onboarding project as the working folder
- initialize the real TypeScript viewer repository structure if none exists
- land the proven [HAN-15](/HAN/issues/HAN-15) path into product code: HWPX zip load, XML parse, minimal IR, and basic browser render shell
- document the exact run/bootstrap command so later tasks reuse the same path

Exit criteria:
- repository/workspace is real and reusable by follow-on issues
- one HWPX sample opens through product code, not only a temporary local script
- the minimal browser viewer path is committed to the workspace with clear next integration points

Dependencies:
- use the corpus/rubric from [HAN-14](/HAN/issues/HAN-14)
- implementation path comes from [HAN-15](/HAN/issues/HAN-15)

Speed rule:
- optimize for the shortest path to a stable engineering baseline, not polish
