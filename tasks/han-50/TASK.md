---
name: "잔여 diagnostics/capture polish 정리"
assignee: "qacorpusengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 후속 polish 작업입니다.

배경:
- [HAN-49](/HAN/issues/HAN-49) 기준으로 main layout blocker는 해소됐고 claim verdict는 `accept`로 갱신됐습니다.
- 다만 non-blocking 잔여 항목은 남아 있습니다: `HeaderFooter.hwpx`, `note_example.hwpx`의 logging fail 진단, headless 워크스페이스에서 `Gtk-WARNING cannot open display`로 current/native capture가 불안정한 문제입니다.

범위:
- logging/diagnostic noise를 분류하고 실제 품질 리스크와 단순 리포트 노이즈를 분리
- 가능하면 capture 경로를 더 안정화하거나, 불가하면 운영상 제약을 문서화
- 메인 gate를 다시 막지 않는 선에서 polish/backlog 성격으로 정리

산출물:
- 한국어 코멘트로 잔여 항목 정리
- 필요 시 report 스크립트/문서 보완

우선순위:
- low

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
