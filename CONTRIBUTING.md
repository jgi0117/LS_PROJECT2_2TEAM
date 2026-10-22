# 협업 규칙

## 브랜치 전략

- `main`: 마지막 배포·제출만 반영합니다. 기능 브랜치에서 직접 머지하지 않습니다.
- `dev`: 모든 기능과 문서를 먼저 합치는 통합 브랜치입니다.
- `feature/<기능>`: 새 기능
- `fix/<문제>`: 버그 수정
- `docs/<문서>`: 문서 작업

## 작업 흐름

```bash
git switch dev
git pull origin dev
git switch -c feature/기능이름

# 작업 후
git add .
git commit -m "feat: 기능 설명"
git push -u origin feature/기능이름
```

1. GitHub에서 `feature/*` → `dev` Pull Request를 엽니다.
2. 팀원 한 명 이상이 확인한 뒤 `dev`에 머지합니다.
3. 머지 후 각 팀원은 최신 `dev`를 다시 받습니다.
4. 최종 QA가 끝났을 때만 `dev` → `main` Pull Request를 머지합니다.

## PR 확인

- 맡은 기능이 처음부터 끝까지 동작하는가
- 키, 비밀번호, 실명 연락처가 커밋되지 않았는가
- 관련 문서와 시험 데이터가 함께 갱신되었는가
- 권한, 빈 값, API 실패 상황을 확인했는가
- 충돌을 해결한 뒤 최신 `dev` 기준으로 다시 확인했는가

