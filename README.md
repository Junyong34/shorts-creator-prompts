# AI 숏츠 프롬프트 저장소

AI 숏츠 제작용 프롬프트를 테마별로 관리하고, 검증 상태에 따라 초안과 최종본을 분리해 운영하는 저장소입니다.

**목적**
- 테마별 숏츠 제작 프롬프트의 체계적 관리
- 검증 전/후 상태 구분으로 품질 확보
- 3인 협업 시 충돌 최소화 및 기록성 유지

**디렉토리 구조**
```text
prompts/
  drafts/
    product-promo/
    story/
    travel-scenery/
    kids/
    kitchen/
    tips/
    misc/
  final/
    product-promo/
    story/
    travel-scenery/
    kids/
    kitchen/
    tips/
    misc/
templates/
  prompt-template.md
```

**drafts vs final 의미**
- `prompts/drafts/` : 검증 전 또는 개선 중인 프롬프트
- `prompts/final/` : 검증 완료 및 재사용 가능한 최종 프롬프트

**테마 폴더 설명**
- `product-promo` : 제품홍보
- `story` : 스토리 있는 테마
- `travel-scenery` : 여행 풍경 관련
- `kids` : 아동
- `kitchen` : 주방
- `tips` : 꿀팁 사용
- `misc` : 기타/추가 테마

**프롬프트 작성 규칙**
- `templates/prompt-template.md` 템플릿을 복사해 작성한다.
- 제목, 훅, 스크립트, 비주얼 구성, CTA를 빠짐없이 기입한다.
- 검증 상태는 `초안`, `검증중`, `완료` 중 하나로 표기한다.

**파일 네이밍 규칙**
- 기본 포맷: `YYYYMMDD-주제-버전.md`
- 예시: `20260204-airfryer-v1.md`
- 버전은 `v1`, `v2` 형식으로 증가한다.

**협업 규칙 (3인 작업 기준)**
- 동일 프롬프트 수정 시 새 버전으로 저장한다.
- 최종본 승격 시 `drafts`에서 `final`로 이동하며, 버전을 증가하거나 상태 변경 기록을 남긴다.
- 테마 신설 시 `misc`에 먼저 추가 후 합의되면 전용 폴더를 만든다.

**검증/승격 흐름**
- 초안은 `prompts/drafts/<theme>/`에 저장한다.
- 검증 완료 후 `prompts/final/<theme>/`로 이동한다.
- 이동 시 버전 증가 또는 상태 변경 기록을 남긴다.
