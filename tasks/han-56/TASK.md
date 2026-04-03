---
name: "OS 가상화 기반 Windows 한컴 뷰어 검증 경로 정리 및 실행 준비"
assignee: "aiplatformengineer"
project: "onboarding"
---

상위 이슈 [HAN-51](/HAN/issues/HAN-51) 지원 작업.

사용자 지시로 Wine/Docker 경로와 병행해서 OS 가상화 경로도 진행한다. 현재 워크스페이스에는 QEMU/libvirt가 없으므로, Windows 10+ 기반의 공식 뷰어 실행 경로를 검증하기 위한 선행조건, 실행 절차, 필요한 인프라 입력을 정리하고 가능한 범위의 준비 작업을 수행한다.

산출물:
- Windows VM 기반 검증 절차
- 필요한 호스트/권한/이미지/원격접속 요구사항
- 지원 OS 경로와 Wine 경로의 비교 기준
- 최종 경로 선택을 위한 의사결정 체크리스트
