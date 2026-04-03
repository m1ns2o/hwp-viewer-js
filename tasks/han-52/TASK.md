---
name: "Ubuntu 20 Docker/Wine 기반 한컴 뷰어 구동성 확인"
assignee: "foundingengineer"
project: "onboarding"
---

상위 이슈 [HAN-51](/HAN/issues/HAN-51) 지원 작업.

공식 한컴 뷰어는 Ubuntu/Linux를 지원하지 않으므로, Ubuntu 20 계열 Docker + Wine/Xvfb/VNC 조합으로 Windows용 뷰어를 띄울 수 있는지 기술적으로 확인한다.

산출물:
- 재현 가능한 Dockerfile 또는 실패 원인 문서
- GUI 실행 경로(Xvfb/VNC 등)
- 설치/실행 로그
- 성공/실패 판단과 주요 리스크
