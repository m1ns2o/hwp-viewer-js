---
name: "fidelity gate 판정 로직 보정 및 증적 기준 재정렬"
assignee: "qacorpusengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 후속 검증/도구 작업입니다.

배경:
- [HAN-45](/HAN/issues/HAN-45) 코멘트 기준 renderer는 일부 실질 개선이 들어갔지만, 현재 QA/fidelity 스크립트는 multi-column / positioned-layout을 정적 fail-side로 보는 구간이 남아 있습니다.
- [HAN-46](/HAN/issues/HAN-46) 결과도 gate가 여전히 `reject`임을 보여주지만, 이 수치가 실제 렌더 결함과 gate heuristic 한계를 얼마나 각각 반영하는지 분리할 필요가 있습니다.

구현 범위:
- `report:hwpx`, `report:qa` 판정 기준을 점검해 정적 fail-side 규칙과 실제 캡처/IR 기반 판단을 분리
- 현재 4개 blocker 각각에 대해 실제 렌더 미흡인지 gate 규칙 과보수인지 분류
- 향후 renderer 개선이 들어오면 gate 결과가 민감하게 반영되도록 기준을 보정

산출물:
- 갱신된 gate/QA 스크립트 또는 명시적 판정 로직 개선
- blocker 4건에 대한 원인 분류표
- 한국어 코멘트로 변경점과 남은 한계 설명

제약:
- 모든 코멘트는 한국어
- gate를 느슨하게 만드는 방향이 아니라, 실제 렌더 품질과 정합되도록 보정

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
