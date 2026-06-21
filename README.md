## 오픈소스 기여

최근 Codex CLI를 위한 워크플로우 레이어인 oh-my-codex의 tmux 기반 멀티 에이전트 런타임 환경에서 Team worker/HUD pane ownership과 shared-session shutdown 안정성 문제를 재현하고 수정했습니다.

릴리즈 반영:

- [oh-my-codex v0.18.10](https://github.com/Yeachan-Heo/oh-my-codex/releases/tag/v0.18.10) - HUD pane 중복 생성 방지 개선 반영
- [oh-my-codex v0.18.14](https://github.com/Yeachan-Heo/oh-my-codex/releases/tag/v0.18.14) - HUD pane ownership 보존 개선 반영

주요 기여:

- [Yeachan-Heo/oh-my-codex #2738](https://github.com/Yeachan-Heo/oh-my-codex/pull/2738), [#2739](https://github.com/Yeachan-Heo/oh-my-codex/pull/2739) - team worker 실행 경로와 worker startup script 경로에서 HUD ownership context가 worker/prompt 실행 환경으로 누수되어 HUD pane이 중복 생성되던 문제를 함께 정리했습니다. HUD 소유권 환경변수를 명시적으로 제거하고, 중복 HUD pane 복구 로직·로컬 소스 기준 실행 경로·회귀 테스트를 보강했습니다.
- [Yeachan-Heo/oh-my-codex #2828](https://github.com/Yeachan-Heo/oh-my-codex/pull/2828) - shared-session Team shutdown 중 사용자 소유 tmux pane이 실수로 종료되거나 HUD가 잘못된 생존 pane에 연결될 수 있던 문제를 수정했습니다. Team 소유 worker/HUD pane만 제거하도록 live tmux worker evidence 기반으로 shutdown 대상을 좁히고, leader pane·무관한 user pane·sidecar pane·별도 HUD pane·복구된 standalone HUD pane을 보존하도록 회귀 테스트를 추가했습니다.


## 관심 영역

- 백엔드 아키텍처 설계
- AI Agent 기반 개발 워크플로우
- 개발 환경 개선과 반복 업무 자동화
