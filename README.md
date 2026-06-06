# MasJeong

Spring Boot/Java 기반 백엔드를 개발하며, 구현 과정에서 개선할 수 있는 지점을 그냥 지나치지 않는 개발자입니다.

반복되는 확인 작업이나 헷갈리기 쉬운 개발 흐름을 발견하면, 문서·도구·자동화로 정리해보는 편입니다.  
최근에는 Claude Code, MCP, 기능 계약서, pre-commit hook 등을 활용해 요구사항 확인과 구현 검증 흐름을 더 안정적으로 만드는 작업을 이어가고 있습니다.

최근에는 OpenAI Codex CLI를 위한 워크플로우 레이어인 oh-my-codex에 기여하며, tmux 기반 멀티 에이전트 런타임에서 HUD pane이 중복 생성되던 문제를 재현하고 수정했습니다.

## 오픈소스 기여

최근 머지된 기여:

- [Yeachan-Heo/oh-my-codex #2738](https://github.com/Yeachan-Heo/oh-my-codex/pull/2738) - team worker 실행 중 tmux HUD 소유권 환경변수가 잘못 전달되어 HUD pane이 중복 생성되던 문제를 수정했습니다.
- [Yeachan-Heo/oh-my-codex #2739](https://github.com/Yeachan-Heo/oh-my-codex/pull/2739) - worker startup script 경로에서도 HUD 소유권 환경변수가 상속되지 않도록 후속 처리를 추가했습니다.

두 PR은 리뷰를 거쳐 원 저장소의 `dev` 브랜치에 머지되었고, 필요한 CI checks가 통과했습니다.

## 관심 영역

- Spring Boot/Java 기반 백엔드 개발
- 개발 흐름 개선과 자동화
- AI Agent 기반 개발 워크플로우
