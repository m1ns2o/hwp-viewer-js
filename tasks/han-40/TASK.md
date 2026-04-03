---
name: "allinpdf 기반 HWPX 기준 렌더 캡처 자동화 구축"
assignee: "foundingengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 하위 작업입니다.

목표:
- `https://allinpdf.com/kr/hwp-viewer` 경로에서 샘플 `.hwpx` 업로드 후 실제 뷰어 화면까지 도달하는 브라우저 자동화 경로를 고정합니다.
- 업로드 전/후, 로딩 상태, 성공 시 렌더 화면까지 스크린샷 산출물을 남깁니다.

산출물:
- 재현 가능한 Playwright 스크립트 또는 동등한 자동화 절차
- 샘플별 스크린샷 경로와 실패 시 실패 지점 정리
- 현재 브라우저 렌더러와 비교에 바로 사용할 수 있는 캡처 세트

제약:
- 외부 서비스 업로드 제한이나 세션 문제를 만나면 정확한 실패 단계와 네트워크/DOM 증거를 남기세요.
- 모든 코멘트는 한국어로 작성하세요.

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
