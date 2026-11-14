
## 📂 GitHub Actions 실습 디렉터리 구조

GitHub Actions의 기본 문법부터 Workflow 자동화, 조건부 실행, Job 간 데이터 전달 및 GitHub API 활용까지 실습한 내용을 날짜별로 정리하였습니다.

```text
.github/
└── workflows/
    │
    ├── Nov06_Practice/                  # 11월 6일 | GitHub Actions 기초 실습
    │   ├── hello.yml                    # Push 이벤트 및 Hello World 출력
    │   ├── shell-command.yml            # Shell 명령어 실행 및 환경변수 활용
    │   ├── workflow-error.yml           # Workflow 구조 오류 확인
    │   ├── yaml-error.yml               # YAML 문법 오류 확인
    │   ├── context.yaml                  # GitHub 및 Runner Context 활용
    │   ├── env.yaml                      # 환경변수 선언 및 범위 확인
    │   ├── env_ref.yaml                  # 환경변수 참조 실습
    │   ├── inter_env_ref.yaml            # 환경변수 간 참조 실습
    │   ├── val_ref.yaml                  # 변수 및 값 참조 실습
    │   ├── secret_ref.yaml               # GitHub Secrets 참조 실습
    │   ├── manual.yaml                   # 수동 실행 이벤트 실습
    │   └── run_time_error.yaml           # Workflow 실행 중 오류 확인
    │
    ├── Nov13_Practice/                  # 11월 13일 | GitHub Actions 심화 실습
    │   ├── run-name.yaml                # Workflow 실행 이름 동적 설정
    │   ├── literal.yaml                 # 리터럴 자료형 및 표현식 사용
    │   ├── operator.yaml                # 논리·비교 연산자 실습
    │   ├── object-filter.yaml           # 객체 필터를 이용한 데이터 추출
    │   ├── string-function.yaml         # 문자열 조건 함수 활용
    │   ├── string-create.yaml           # 문자열 생성 및 결합 함수 활용
    │   ├── json-function.yaml           # JSON 데이터 변환 함수 활용
    │   ├── hash.yaml                    # hashFiles()를 이용한 파일 해시 계산
    │   ├── hash-experiment.yaml         # 파일 생성·수정에 따른 해시값 변화 추가 실험
    │   ├── condition.yaml               # if 조건에 따른 Step 실행 제어
    │   ├── condition-workflow.yaml       # Job 조건 및 needs 의존성 실습
    │   ├── status-check.yaml            # success·failure·always 등 상태 함수 실습
    │   ├── job-status.yaml              # Job 성공·실패에 따른 조건부 실행
    │   ├── var.yaml                     # GITHUB_ENV 및 GITHUB_OUTPUT 활용
    │   ├── job-output.yaml              # Job 간 출력값 전달
    │   └── issue-comment.yaml           # Issue 생성 시 댓글 자동 작성
    │
    └── assignment-issue.yaml            # 별도 과제 | Push 이벤트 발생 시 Issue 자동 생성
```

### 📝 실습 내용

- 11월 6일 — GitHub Actions의 기본 구조, 이벤트, Runner, Context, 환경변수, Secrets 및 오류 처리 실습
- 11월 13일 — 표현식, 연산자, 문자열·JSON 함수, 조건부 실행, Job 의존성, 상태 함수 및 출력값 전달 실습
- 추가 실험 — 파일 해시값 변화와 Workflow 실행 조건에 따른 결과 비교
- **별도 과제** — Push 이벤트 발생 시 GitHub API를 활용하여 Issue를 자동 생성하는 Workflow 구현

> 날짜별 디렉터리는 실습 파일 보관용이며, 실제 실행되는 Workflow 파일은 `.github/workflows/` 최상위 경로에 별도로 유지하였습니다.
