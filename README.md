# MasJeong

개발자 도구와 자동화 런타임 안정성에 관심이 많은 엔지니어입니다.

운영 중에도 이해 가능한 구조, 재현 가능한 버그 수정, 테스트로 검증되는 변경을 중요하게 생각합니다. 최근에는 CLI, tmux 기반 세션 오케스트레이션, 자동화 도구의 런타임 안정성에 관심을 두고 있습니다.

## 오픈소스 기여

최근 머지된 기여:

- [Yeachan-Heo/oh-my-codex #2738](https://github.com/Yeachan-Heo/oh-my-codex/pull/2738) - team worker 실행 중 tmux HUD 소유권 환경변수가 잘못 전달되어 HUD pane이 중복 생성되던 문제를 수정했습니다.
- [Yeachan-Heo/oh-my-codex #2739](https://github.com/Yeachan-Heo/oh-my-codex/pull/2739) - worker startup script 경로에서도 HUD 소유권 환경변수가 상속되지 않도록 후속 처리를 추가했습니다.

두 PR은 리뷰를 거쳐 원 저장소의 `dev` 브랜치에 머지되었고, 필요한 CI checks가 통과했습니다.

## 엔지니어링 관심 영역

- CLI 도구와 자동화 런타임
- 재현 가능한 버그 수정과 회귀 테스트
- 프로세스/런타임 환경 격리
- 멀티 에이전트 개발 도구
- 안정적인 tmux/session 오케스트레이션
- 실패 원인을 숨기지 않는 자동화와 실용적인 관측 가능성
