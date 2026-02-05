# AI Tools 사전 조사 TODO

프롬프트 작성 전에 3명이 분담하여 사전 조사를 진행한다.

## 담당자
- 숏츠/동영상 제작 AI Tools: **Mango**
- 자막 및 자동 번역 AI Tools: **Orbit**
- 음성 생성 AI Tools: **Raven**

## 진행 상태
- 상태: `미시작 / 진행중 / 완료`
- 마감일: `TBD`

---

## 공통 평가 항목 체크리스트
- [ ] 가격/구독: 월/연 비용, 과금 방식(크레딧/분당/좌석)
- [ ] 무료 체험/환불: 체험 기간, 제한, 환불 정책
- [ ] 사용 편의성: UI 난이도, 학습 곡선, 템플릿 제공 여부
- [ ] 다국어 지원: 지원 언어 수, 한글 품질
- [ ] 품질: 결과물 자연스러움, 아티팩트 여부
- [ ] 생성 가능 시간: 최대 길이, 동시 생성 한도, 큐 대기
- [ ] 출력/포맷: 해상도, 포맷, 자막 파일 지원 여부
- [ ] 워터마크/라이선스: 워터마크 유무, 상업적 사용 가능 여부
- [ ] 속도/성능: 평균 생성 시간, 안정성
- [ ] API/연동: API 제공 여부, Zapier/플러그인
- [ ] 팀 협업: 공유/코멘트/버전 관리
- [ ] 지역/결제: 결제 가능 국가, 한글 UI 지원
- [ ] 보안/데이터: 학습 사용 여부, 데이터 보관 정책

---

## 1) 숏츠/동영상 제작 AI Tools 

### TODO
- [ ] 후보 도구 3~5개 리스트업
- [ ] 공통 체크리스트 항목 조사
- [ ] 비교표 작성
- [ ] 최종 추천 1~2개와 이유 정리

### 비교표
| Tool | Price/Plan | Trial | Ease | Languages | Quality | Max Duration | Export/Format | Watermark/License | API/Integration | Notes | Score(1-5) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Google Veo (Veo3)** | Vertex AI ($0.75/s), AI Pro($19.99) | Cloud Credit ($300) | Mid/High | Multi (Gemini) | High (4K, Cinematic) | 8s+ (Extendable) | MP4 (1080p+) | SynthID (Invisible) | Yes (Vertex AI) | Google DeepMind 최신 모델, Native Audio 지원 | 4.9 |
| **Nanobanana** | Credit ($9.99/mo~), ~1-2c/sec | Free w/ limit | High | Eng | Mid/High | 5s~Continuous | MP4 | Yes (Free) | Limited | Google Gemini/Veo 기반 Wrapper 추정, 이미지-비디오 강점 | 3.8 |
| **Google Flow (VideoFX)** | Google AI Premium ($19.99/mo) | Labs Access | High | Eng/Multi | High (Veo 기반) | Short clips (Loop/Extend) | MP4 | Yes (SynthID) | No (Consumer) | Veo/Imagen 모델 사용 가능한 일반 사용자용 UI Tools | 4.7 |
| **Higgsfield AI** | Free ($0), Basic (~$9), Pro (~$29), Ultimate (~$49) | Free w/ limit | High | multi | High (Cinematic) | 5s+ | MP4 (up to 720p) | Yes (Free) | Yes (Creator Plan) | Cinematic motion control 강점, Kling/Sora/Veo 등 다양한 모델 통합 | 4.6 |


---


**주요 도구별 개별 특징**

- **Google Veo (모델 엔진)**
    - Google DeepMind의 최첨단 영상 생성 모델로, 텍스트와 이미지로부터 고화질(4K급) 시네마틱 영상을 생성합니다.
    - 영상 내 물리 법칙, 조명, 질감을 정교하게 이해하며 자연스러운 움직임을 구현하는 데 집중합니다.
    - 주로 API나 Vertex AI를 통해 제공되며, 전문적인 영상 생성 기술의 근간이 됩니다.

- **Google Flow (제작 플랫폼)**
    - 일반 사용자와 크리에이터가 웹상에서 직관적으로 영상을 제작할 수 있도록 설계된 인터페이스 도구입니다.
    - 단순히 영상을 만드는 것을 넘어 여러 장면을 연결하고, 등장인물(캐릭터)의 일관성을 유지하며 시퀀스를 구성하는 워크플로우를 제공합니다.
    - Google Labs(VideoFX) 환경에서 대화형 인터페이스를 통해 복잡한 설정 없이 창의적인 비디오를 쉽고 빠르게 제작할 수 있게 돕습니다.

- **Nanobanana (이미지-비디오 특화)**
    - Google의 Gemini/Veo 기술을 기반으로 구축된 것으로 추정되는 서비스로, 특히 이미지 내의 캐릭터나 스타일을 유지한 채 비디오로 변환하는 데 강점이 있습니다.
    - 사용자 친화적인 UI를 통해 비교적 저렴한 크레딧 방식으로 쉽고 빠르게 비디오 콘텐츠를 생산할 수 있는 것이 특징입니다.

- **Higgsfield AI (시네마틱 컨트롤 특화)**
    - 70개 이상의 전문 카메라 워킹(Dolly, Whip Pan, Drone 등)을 제공하여 영화 같은 연출이 가능한 AI 영상 제작 플랫폼입니다.
    - Kling 2.6, Sora 2, Veo 3.1 등 시장의 주요 SOTA 모델들을 하나의 구독으로 이용할 수 있는 '멀티 모델 통합'이 핵심 강점입니다.
    - 'Cinema Studio' 기능을 통해 조명, 앵글, 모션을 세밀하게 조정할 수 있어, 단순 생성을 넘어 '디렉팅'이 가능한 환경을 제공합니다.



## 2) 자막 및 자동 번역 AI Tools 

### TODO
- [ ] 후보 도구 3~5개 리스트업
- [ ] 공통 체크리스트 항목 조사
- [ ] 비교표 작성
- [ ] 최종 추천 1~2개와 이유 정리

### 비교표
| Tool | Price/Plan | Trial | Ease | Languages | Quality | Max Duration | Export/Format | Watermark/License | API/Integration | Notes | Score(1-5) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Google Cloud STT** | Usage-based | $300 Credit | Mid/High | 125+ | High | Unlimited | SRT, VTT, JSON | Custom | Yes (API) | 동영상 자막 추출 및 번역 최적화, 최신 Chirp 모델 지원 | 4.8 |
| **Vertex AI Studio** | Usage-based | $300 Credit | Mid | Multi | High | File size limit | SRT, Text | Custom | Yes | Gemini 모델을 활용한 비디오 분석 및 자막 생성 가능 | 4.5 |

**자막 및 번역 도구별 개별 특징**

- **Google Cloud STT (Speech-to-Text)**
    - 전문적인 오디오 전사 도구로, 동영상 파일에서 음성을 추출하여 SRT, VTT 등 표준 자막 파일로 변환하는 데 최적화되어 있습니다.
    - 최신 Chirp 모델을 통해 배경 소음이 있는 환경에서도 높은 정확도를 유지하며, 125개 이상의 언어를 지원합니다.

- **Vertex AI Studio (비디오 분석형 자막)**
    - Gemini 모델의 멀티모달 능력을 활용하여 영상의 시각적 맥락과 음성을 동시에 분석, 단순 전사보다 정확한 문맥 기반 자막을 생성합니다.
    - 별도의 복잡한 API 연동 없이 Google Cloud 콘솔에서 비디오 파일을 직접 업로드하여 자막 결과물을 뽑아낼 수 있습니다.


---

## 3) 음성 생성 AI Tools

### TODO
- [ ] 후보 도구 3~5개 리스트업
- [ ] 공통 체크리스트 항목 조사
- [ ] 비교표 작성
- [ ] 최종 추천 1~2개와 이유 정리

### 비교표
| Tool | Price/Plan | Trial | Ease | Languages | Quality | Max Duration | Export/Format | Watermark/License | API/Integration | Notes | Score(1-5) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Google Cloud TTS** | Usage-based | $300 Credit | Mid | 75+ (380+ voices) | Very High | 1M+ chars | MP3, WAV, OGG | Custom | Yes (API) | Gemini-TTS, Chirp 3 등 인간에 가까운 감정 표현 가능 | 4.9 |
| **Gemini API (TTS)** | Usage-based | Free tier avail. | High | Multi | High | Short/Long | Audio stream | Custom | Yes | 자연어 프롬프트로 억양, 속도, 톤 미세 조정 가능 | 4.7 |

**음성 생성 도구별 개별 특징**

- **Google Cloud TTS (Text-to-Speech)**
    - 380개 이상의 풍부한 보이스를 제공하며, 특히 'Chirp 3' 모델은 웃음소리, 머뭇거림 등 인간 특유의 비언어적 표현까지 자연스럽게 구현합니다.
    - 대규모 텍스트 전사 및 전문적인 성우 오디오 제작에 적합하며, SSML 지원을 통해 발음을 정밀하게 교정할 수 있습니다.

- **Gemini API (멀티모달 음성)**
    - "부끄러운 듯이 말해줘", "기쁜 목소리로 속도를 높여줘"와 같은 일상적인 명령어로 음성의 톤과 감정을 조절할 수 있습니다.
    - 최신 멀티모달 기술이 적용되어 단순 낭독을 넘어 대화의 맥락에 맞는 가장 자연스러운 감정선을 스스로 찾아 음성을 생성합니다.


---

## 결과 요약
- 숏츠/동영상 제작 도구 최종 추천:
- 자막/번역 도구 최종 추천:
- 음성 생성 도구 최종 추천:

## 프롬프트 작성 반영 메모
- 
