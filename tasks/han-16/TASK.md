---
name: "Run HWP binary extraction feasibility spike"
assignee: "cto"
---

[HAN-11](/HAN/issues/HAN-11#document-plan)에서 2차 Phase 0 스파이크를 실행합니다: HWPX-first MVP 시퀀스의 안정성을 해치지 않으면서 이진 HWP 경로가 어디까지 진행될 수 있는지 확인합니다.

산출물:

* TypeScript에서 HWP OLE/CFB 컨테이너 구조를 검사하기
* 텍스트 및 구조 복원에 필요한 주요 스트림과 메타데이터를 파악한다
* 대표적인 HWP 샘플 하나 이상에서 기본 텍스트와 단락 또는 섹션 경계를 복원한다
* 참고 자료를 바탕으로 바이너리 형식의 미확인 항목, 지원되지 않을 가능성이 높은 영역 및 라이선스 제한 사항을 기록한다
* HWP가 MVP 핵심 일정에 그대로 남아야 하는지, 아니면 HWPX-first 마일스톤 이후에 강화 단계로 넘어가야 하는지에 대한 의견을 남겨 주세요.

종료 기준:

* 대표적인 HWP 샘플 하나를 통해 기본 텍스트 또는 구조를 추출할 수 있다
* 위험 지역이 구체적으로 명시되어 있다
* 팀은 MVP 단계별 순서에 대해 명확한 진행/중단 권고안을 제시하고 있습니다

제약 조건:

* 이 급증으로 인해 [HAN-11](/HAN/issues/HAN-11#document-plan)에 정의된 주요 HWPX 경로의 처리가 지연되지 않도록 하십시오
