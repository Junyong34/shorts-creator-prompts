# 커밋 규칙 가이드

이 문서는 팀 내 커밋 메시지 규칙을 통일하기 위한 가이드입니다.

## 메시지 형식
```
type(scope): summary
```

## 허용 type
- feat
- fix
- docs
- chore
- refactor
- test
- build
- ci
- perf
- revert

## scope 권장값
- prompts
- templates
- docs
- repo

## summary 규칙
- 한글로 작성한다.
- 현재형/명령형으로 작성한다.
- 72자 이내로 작성한다.
- 문장 끝 마침표는 생략한다.

## 본문 규칙 (선택)
- 한 줄 띄우고 본문을 작성한다.
- 변경 이유, 영향 범위, 검증 내용을 포함한다.

## 예시
```
docs(repo): add commit guidelines
feat(prompts): add initial product promo draft
fix(templates): refine CTA section wording
chore(docs): move verified prompts to final
```

## 참고 사항
- `prompts/drafts`에서 `prompts/final`로 이동할 때는 버전을 증가하거나 상태 변경 기록을 남긴다.
- 이 문서는 `README.md`의 규칙과 충돌하지 않도록 유지한다.
