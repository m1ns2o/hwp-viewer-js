---
name: "SimpleTable positioned anchor 증거 보강 및 실제 layout blocker 해소"
assignee: "renderingengineer"
project: "onboarding"
---

[HAN-37](/HAN/issues/HAN-37) 후속 구현 작업입니다.

배경:
- [HAN-48](/HAN/issues/HAN-48) 기준 legacy 4-blocker 중 실제 render gap으로 남은 것은 `SimpleTable.hwpx` 1건뿐입니다.
- 현재 문제는 `positioned-layout`과 anchor evidence가 아직 충분히 해소되지 않아 gate가 `reject`를 유지하는 것입니다.

구현 범위:
- `SimpleTable.hwpx`의 positioned table anchor 근거를 parser/IR/renderer에서 끝까지 추적
- 현재 unresolved로 남은 anchor evidence를 구체적으로 없애고, table placement가 gate 기준에서도 실제 반영되도록 수정
- 필요하면 최소 범위의 parser 보강을 포함하되, 목표는 `SimpleTable.hwpx` blocker 제거에 집중

산출물:
- 코드 반영
- 왜 `SimpleTable.hwpx`가 막혔는지와 무엇을 바꿨는지 한국어 코멘트 설명
- `npm run build`와 관련 리포트 재실행 결과

제약:
- 모든 코멘트는 한국어
- 범위를 다시 넓히지 말고 `SimpleTable.hwpx` 단일 blocker 해소에 집중

상위 이슈: [HAN-37](/HAN/issues/HAN-37)
연계 이슈: [HAN-47](/HAN/issues/HAN-47), [HAN-48](/HAN/issues/HAN-48)
