# MasJeong

Spring Boot/Java 기반 업무 시스템을 개발하는 백엔드 엔지니어입니다.

외부 연계 API, 조회 성능, 트랜잭션 경계, JPA/QueryDSL 기반 쿼리 구조처럼 운영 중 문제가 될 수 있는 지점을 분석하고 개선하는 데 관심이 있습니다.  
반복되는 확인 작업과 품질 리스크를 자동화 가능한 문제로 바라보며, Claude Code, MCP, 기능 계약서, pre-commit hook 등을 활용해 개발 흐름을 더 안정적으로 만드는 작업을 이어가고 있습니다.

최근에는 오픈소스 자동화 도구인 oh-my-codex에 기여하며, tmux 기반 멀티 에이전트 런타임에서 HUD pane이 중복 생성되던 문제를 재현하고 수정했습니다.

## 오픈소스 기여

최근 머지된 기여:

- [Yeachan-Heo/oh-my-codex #2738](https://github.com/Yeachan-Heo/oh-my-codex/pull/2738) - team worker 실행 중 tmux HUD 소유권 환경변수가 잘못 전달되어 HUD pane이 중복 생성되던 문제를 수정했습니다.
- [Yeachan-Heo/oh-my-codex #2739](https://github.com/Yeachan-Heo/oh-my-codex/pull/2739) - worker startup script 경로에서도 HUD 소유권 환경변수가 상속되지 않도록 후속 처리를 추가했습니다.

두 PR은 리뷰를 거쳐 원 저장소의 `dev` 브랜치에 머지되었고, 필요한 CI checks가 통과했습니다.

## 관심 영역

- Spring Boot 기반 백엔드 설계와 구현
- JPA/QueryDSL 기반 조회 성능 개선
- 외부 연계 API와 트랜잭션 경계 설계
- 개발 프로세스 자동화와 품질 게이트
- AI Agent 기반 개발 워크플로우
- 재현 가능한 버그 수정과 회귀 방지
