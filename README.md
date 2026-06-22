## 오픈소스 기여

최근 Codex CLI를 위한 워크플로우 레이어인 oh-my-codex의 tmux 기반 멀티 에이전트 런타임 환경에서 Team worker/HUD pane ownership과 shared-session shutdown 안정성 문제를 재현하고 수정했습니다.

릴리즈 반영:

- [oh-my-codex v0.18.10](https://github.com/Yeachan-Heo/oh-my-codex/releases/tag/v0.18.10) - HUD pane 중복 생성 방지 개선 반영
- [oh-my-codex v0.18.14](https://github.com/Yeachan-Heo/oh-my-codex/releases/tag/v0.18.14) - HUD pane ownership 보존 개선 반영

주요 기여:

- [Yeachan-Heo/oh-my-codex #2738](https://github.com/Yeachan-Heo/oh-my-codex/pull/2738), [#2739](https://github.com/Yeachan-Heo/oh-my-codex/pull/2739) - team worker 실행 시 부모 pane의 HUD ownership context가 worker 실행 환경에 전달되어 HUD pane이 중복 생성되는 문제를 발견하였고 worker 실행 전 HUD 소유권 관련 환경변수를 제거하도록 개선했으며 worker 실행 경로별 재현 테스트를 통해 HUD pane이 중복 생성되지 않는 것을 검증했습니다.

- [Yeachan-Heo/oh-my-codex #2828](https://github.com/Yeachan-Heo/oh-my-codex/pull/2828) - shared-session Team shutdown 시 종료 대상 Tmux pane 판별되지 않아 사용자 소유 tmux pane이 종료되고 HUD가 잘못된 pane에 연결될 수 있는 문제를 마주하였습니다. 실행 중인 tmux worker pane 정보를 기준으로 Team 소유 worker/HUD pane만 종료 대상으로 제한하도록 개선하고 리더 pane·개인 pane·standalone HUD pane 보존 여부를 테스트로 검증하였습니다.

## 관심 영역

- AI Agent Engineering
- AI Agent 기반 개발 워크플로우
- 개발 환경 개선과 반복 업무 자동화
- 백엔드 아키텍처 설계
