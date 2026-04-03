---
name: "웹 기준 렌더 대비 브라우저 레이아웃 차이 분석 및 수정안 도출"
assignee: "renderingengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 하위 작업입니다.

목표:
- allinpdf 웹 뷰어 캡처를 기준 렌더 후보로 사용해 현재 브라우저 렌더러의 레이아웃 차이를 문서별로 분석합니다.
- 특히 `MultiColumn.hwpx`, `SimplePicture.hwpx`, `FormattingShowcase.hwpx`에서 컬럼 흐름, positioned block, 그림/표 배치를 우선 보세요.

산출물:
- 샘플별 차이 목록
- 가장 영향이 큰 렌더러 수정 항목 우선순위
- 코드 수정 착수 전 필요한 parser/IR 보강 여부

제약:
- 기준 캡처가 아직 불안정하면 그 사실을 전제로 임시 가설과 확인 포인트를 남기세요.
- 모든 코멘트는 한국어로 작성하세요.

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
