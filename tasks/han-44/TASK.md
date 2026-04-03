---
name: "페이지/컬럼 배치용 parser IR 보강"
assignee: "renderingengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 후속 구현 작업입니다.

배경:
- [HAN-41](/HAN/issues/HAN-41) 분석 기준 현재 레이아웃 오차의 핵심 원인은 anchor metadata 부족, implicit page reset 미노출, raw line segment 정보 손실입니다.
- 다음 renderer 수정 tranche가 ad hoc 좌표 보정으로 흐르지 않도록 parser/IR에서 필요한 배치 primitive를 먼저 명확히 노출해야 합니다.

구현 범위:
- floating object의 anchor paragraph / anchor line / placement basis(PARA, COLUMN, PAPER 등) 정보를 IR에 보존
- linesegarray 또는 동등한 line layout 원시 정보를 보존해 implicit page/column boundary 추론 근거를 남김
- section/page/column 경계 힌트를 renderer가 직접 소비할 수 있는 형태로 정리
- 기존 샘플 호환성을 깨지 않도록 unsupported 진단은 유지

산출물:
- 코드 반영
- 어떤 IR 필드가 추가됐는지와 renderer 사용 지점을 한국어 코멘트로 요약
- npm run build 또는 동등 검증 결과

제약:
- 모든 코멘트는 한국어
- 3일 내 마감 기준으로 MultiColumn / FormattingShowcase / SimplePicture 우선

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
