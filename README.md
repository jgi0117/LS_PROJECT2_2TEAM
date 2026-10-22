# LS PROJECT 2 · 2TEAM

실시간 데이터와 회원 입력 데이터를 결합해 조회, 요청, 관리자 처리를 한 흐름으로 구현하는 팀 프로젝트입니다.

## 현재 상태

- `main`: 최종 제출·배포용 브랜치(초기에는 비어 있음)
- `dev`: 팀 통합 개발 브랜치(공통 문서와 디렉터리 뼈대)
- 서비스 주제와 기술 스택은 팀 합의 후 기록합니다.
- 배포 주소: 미정

## 시작하기

```bash
git clone https://github.com/jgi0117/LS_PROJECT2_2TEAM.git
cd LS_PROJECT2_2TEAM
git switch dev
git pull origin dev
git switch -c feature/기능이름
```

작업 및 PR 규칙은 [CONTRIBUTING.md](CONTRIBUTING.md)를 따릅니다.

## 디렉터리

```text
.
├─ .claude/skills/       팀 전용 스킬
├─ docs/                 기획, 설계, QA, 평가 문서
│  ├─ features/          기능별 구현 계획과 담당자
│  ├─ interviews/        인터뷰 원문
│  ├─ personas/          인터뷰용 페르소나
│  └─ references/        디자인·기능 참고 자료
├─ fixtures/             정상·경계값 시험 데이터
│  └─ broken/            빈 값·오류 시험 데이터
└─ 발표/                 3분 HTML 발표 자료
   └─ images/            직접 촬영한 화면 캡처
```

애플리케이션 디렉터리와 실행 명령은 기술 스택 확정 후 `dev`에서 추가합니다.

