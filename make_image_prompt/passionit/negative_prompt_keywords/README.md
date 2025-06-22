# 부정 프롬프트 사용 가이드

부정 프롬프트를 효과적으로 사용하기 위한 종합 가이드입니다.

## 📋 카테고리별 파일 목록

1. **[해상도_및_품질_관련.md](./해상도_및_품질_관련.md)** - 저화질, 압축 오류, 선명도 부족 방지
2. **[인체_왜곡_및_해부학_오류.md](./인체_왜곡_및_해부학_오류.md)** - 손, 팔, 다리, 얼굴 등의 해부학적 오류 방지
3. **[컴포지션_구도_오류.md](./컴포지션_구도_오류.md)** - 구도, 프레이밍, 포커스 오류 방지
4. **[시각적_방해_요소.md](./시각적_방해_요소.md)** - 텍스트, 워터마크, 렌더 오류 방지
5. **[배경_및_소품_오류.md](./배경_및_소품_오류.md)** - 배경 왜곡, 의미 없는 요소 방지
6. **[스타일_오류_원하지않는_시각적_스타일.md](./스타일_오류_원하지않는_시각적_스타일.md)** - 특정 아트 스타일 제외
7. **[감정_표현_인물_표정_오류.md](./감정_표현_인물_표정_오류.md)** - 인물 표정 오류 방지
8. **[기타_특수_부정_요소.md](./기타_특수_부정_요소.md)** - 기타 특수 상황 대응

## ✅ 부정 프롬프트 작성 팁

### 1. 적정 개수 유지
- **핵심 요소 5~15개 정도**로 구성하는 것이 이상적
- 너무 많은 부정 키워드는 오히려 품질 저하나 혼란 발생 가능

### 2. 목적에 맞는 선택적 조합
- 프롬프트 목적에 맞게 카테고리별로 선택적으로 조합
- 예: 인물 사진 → 해부학 오류 + 품질 관련 중점

### 3. 우선순위 설정
1. **필수**: 해상도 및 품질 관련
2. **인물 이미지 시**: 인체 왜곡 및 해부학 오류
3. **상황별**: 나머지 카테고리에서 선택

## 🧩 상황별 추천 부정 프롬프트 조합

### 고품질 인물 사진
```
low quality, blurry, bad anatomy, deformed hands, extra fingers, bad hands, missing fingers, asymmetrical face, watermark, text, cropped, out of frame, jpeg artifacts
```

### 배경이 포함된 풍경 사진
```
low quality, blurry, pixelated, weird background, random object, cluttered background, text, watermark, bad perspective, compression artifacts
```

### 캐릭터 일러스트
```
low quality, bad anatomy, deformed hands, extra fingers, asymmetrical face, blurry, text, cropped, duplicate body, merged body parts
```

### 제품 사진
```
low quality, blurry, bad perspective, cluttered background, text, watermark, random object, floating item, compression artifacts
```

## 🔧 플랫폼별 고려사항

### Stable Diffusion 계열
- 기술적 키워드가 효과적
- 세부적인 해부학 키워드 활용 권장

### GPT-4o 등 자연어 기반
- 의미 중심의 설명적 키워드 효과적
- 자연스러운 문장 형태로도 가능

### 기타 AI 도구
- 각 도구의 특성에 맞게 조합 조정
- 실험을 통한 최적화 필요

## ⚠️ 주의사항

1. **과도한 사용 금지**: 너무 많은 부정 키워드는 역효과
2. **상황별 조정**: 원하는 결과에 따라 키워드 선택 조정
3. **플랫폼 정책 준수**: 성적/폭력적 키워드 사용 시 정책 확인
4. **지속적 실험**: 최적의 조합 찾기 위한 테스트 필요

## 📚 참고자료

- 각 카테고리별 상세 설명은 개별 마크다운 파일 참조
- 실제 사용 시에는 목적에 맞게 선택적으로 조합하여 사용
