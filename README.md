## 오픈소스 기여

최근 OpenAI Codex CLI를 위한 워크플로우 레이어인 oh-my-codex에 기여하며, tmux 기반 멀티 에이전트 런타임에서 HUD pane이 중복 생성되던 문제를 재현하고 수정했습니다.

릴리즈 반영:

- [oh-my-codex v0.18.10](https://github.com/Yeachan-Heo/oh-my-codex/releases/tag/v0.18.10) - 해당 기여가 릴리즈에 반영되었고 릴리즈 노트에서 contributor로 확인할 수 있습니다.

최근 머지된 기여:

- [Yeachan-Heo/oh-my-codex #2738](https://github.com/Yeachan-Heo/oh-my-codex/pull/2738) - team worker 실행 시 HUD ownership context가 worker/prompt 실행 경로로 누수되어 HUD pane이 중복 생성되던 문제를 수정하고, 중복 HUD pane 복구 로직·로컬 소스 기준 실행 경로·회귀 테스트를 보강했습니다.
- [Yeachan-Heo/oh-my-codex #2739](https://github.com/Yeachan-Heo/oh-my-codex/pull/2739) - worker startup script 경로에서도 HUD 소유권 환경변수를 명시적으로 제거하도록 후속 보완하고 회귀 테스트를 추가했습니다.


## 관심 영역

- 백엔드 아키텍처 설계
- AI Agent 기반 개발 워크플로우
- 개발 환경 개선과 반복 업무 자동화
