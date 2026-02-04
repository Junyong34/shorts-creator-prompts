# 자막/텍스트 Safe Zone

**관련 가이드**
- [실전 프롬프트 예시](examples.md)
- [핵심 팁 모음](tips.md)
- [가이드 허브](README.md)

## Safe Zone 다이어그램

```
+------------------+
|   TOP SAFE ZONE  |  <- 상단 10-15% (플랫폼 UI 겹침 방지)
|                  |
|                  |
|  MAIN CONTENT    |  <- 중앙 70% (핵심 콘텐츠)
|  (Subject Here)  |
|                  |
|                  |
| BOTTOM SAFE ZONE |  <- 하단 15-20% (자막 영역)
+------------------+
```

## 프롬프트에 포함할 지시
- "Keep subject centered for vertical screen"
- "Leave bottom 20% clear for subtitles"
- "Maintain safe zones at top and bottom"

## 핵심 강조
- 하단 15-20%는 자막/텍스트 오버레이 영역으로 비워두기
