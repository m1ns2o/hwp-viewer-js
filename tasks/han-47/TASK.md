---
name: "float-wrap 및 positioned layout fidelity 3차 수정"
assignee: "renderingengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 후속 구현 작업입니다.

배경:
- [HAN-46](/HAN/issues/HAN-46) 재평가 결과 gate는 여전히 `reject`이며 blocker 4건이 유지됩니다. 핵심 잔여 결함은 `FormattingShowcase.hwpx`, `SimpleTable.hwpx`, `SimplePicture.hwpx`의 positioned-layout 미보존과 `MultiColumn.hwpx`의 multi-column 선형 fallback입니다.
- [HAN-45](/HAN/issues/HAN-45)에서 좌표 해석과 lane/page 판정은 개선됐지만, float가 본문 flow를 실제로 밀어내는 규칙과 wrap fidelity는 아직 빠져 있습니다.

구현 범위:
- floating table/picture가 body flow를 밀어내는 text wrap 규칙 구현
- `PARA`뿐 아니라 필요한 `COLUMN`/`PAPER` 기준에서도 wrap/anchor 동작을 일관되게 적용
- `MultiColumn.hwpx`가 더 이상 선형 fallback으로 판정되지 않도록 lane 분배와 page progression을 보강
- 우선 샘플: MultiColumn, FormattingShowcase, SimpleTable, SimplePicture

산출물:
- 코드 반영
- 샘플별로 어떤 blocker가 실제로 줄었는지 한국어 코멘트 요약
- `npm run build` 및 가능하면 `report:qa` 재실행 결과

제약:
- 모든 코멘트는 한국어
- ad hoc CSS patch가 아니라 renderer/layout 규칙 수준에서 정리

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
