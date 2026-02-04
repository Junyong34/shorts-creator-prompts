# AGENTS.md

이 문서는 LLM(에이전트)이 이 저장소에서 작업할 때 따라야 하는 공통 규칙을 정의합니다.

## 프로젝트 목적
- AI 숏츠 제작 프롬프트를 테마별로 관리한다.
- 검증 전/후 상태를 분리해 품질을 안정적으로 유지한다.

## 핵심 구조
- `prompts/drafts/` : 검증 전 또는 개선 중인 프롬프트
- `prompts/final/` : 검증 완료 및 재사용 가능한 최종 프롬프트
- `templates/` : 표준 프롬프트 템플릿

## 작업 규칙
- 프롬프트는 `templates/prompt-template.md`를 기반으로 작성한다.
- 초안은 `prompts/drafts/<theme>/`에만 저장한다.
- 검증 완료 후 `prompts/final/<theme>/`로 이동한다.
- 파일명 규칙 `YYYYMMDD-주제-버전.md`를 준수한다.
- 테마 추가는 `misc`에서 시작하고 합의되면 전용 폴더를 만든다.

## 테마 목록
- `product-promo`
- `story`
- `travel-scenery`
- `kids`
- `kitchen`
- `tips`
- `misc`

## 협업 및 검증 흐름
- 초안 작성 → 검증 → 최종 승격의 순서를 따른다.
- 최종 승격 시 버전 증가 또는 상태 변경 기록을 남긴다.

## 참고 문서
- `README.md`
- `docs/commit-guidelines.md`
- `templates/prompt-template.md`
