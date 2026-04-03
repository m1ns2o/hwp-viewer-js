---
name: "page/column/positioned layout renderer 2차 수정"
assignee: "renderingengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 후속 구현 작업입니다.

배경:
- [HAN-41](/HAN/issues/HAN-41), [HAN-42](/HAN/issues/HAN-42) 기준 현재 reject 게이트의 주 원인은 컬럼 흐름, positioned object 기준 좌표 변환, implicit page reset 처리입니다.
- [HAN-40](/HAN/issues/HAN-40), [HAN-43](/HAN/issues/HAN-43) 결과상 allinpdf는 안정적 oracle이 아니므로, XML/IR 근거와 현재 캡처를 바탕으로 renderer 정확도를 먼저 끌어올립니다.

구현 범위:
- placement basis별 좌표 변환(PARA/COLUMN/PAPER 등) 정리
- implicit page reset과 section/page container 흐름 보정
- multi-column flow를 현재 y 역전 + columnBreak 편향 로직에서 탈피시켜 재설계
- floating table/picture 배치를 page overlay 구조 안에서 일관되게 처리

산출물:
- 코드 반영
- 수정 전후 차이와 남은 known gap을 한국어 코멘트로 요약
- npm run build 및 가능하면 관련 리포트 재실행

제약:
- 모든 코멘트는 한국어
- 우선순위 샘플: MultiColumn, FormattingShowcase, SimplePicture, SimpleTable

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
