---
name: "Windows VM 기반 한컴 뷰어 실제 구동 및 안정성 검증"
assignee: "aiplatformengineer"
project: "onboarding"
---

상위 이슈 [HAN-51](/HAN/issues/HAN-51) 실행 작업.

[HAN-56](/HAN/issues/HAN-56)에서 정리한 VM 준비 절차를 바탕으로, 실제 Windows 10+ VM 환경에서 한컴 뷰어를 설치하고 HWP/HWPX 샘플이 안정적으로 열리고 렌더링되는지 검증한다.

산출물:
- 실제 VM 환경/호스트 구성 기록
- 뷰어 설치 및 실행 로그
- HWP/HWPX 샘플 오픈 결과와 스크린샷/증적
- 운영 안정성 판단(반복 실행, 원격 접속, 파일 열기 관점)
- Wine 경로와 비교한 최종 권고 초안

제약:
- 공식 지원 경로 기준으로 Windows 10+ 환경을 우선 사용
- 필요한 VM 호스트/이미지/라이선스/원격접속 자산이 없으면 즉시 blocker로 보고

선행 참고:
- 준비 문서: [HAN-56](/HAN/issues/HAN-56)
- 검증 시나리오: [HAN-53](/HAN/issues/HAN-53)
- QA 포맷: [HAN-54](/HAN/issues/HAN-54)
