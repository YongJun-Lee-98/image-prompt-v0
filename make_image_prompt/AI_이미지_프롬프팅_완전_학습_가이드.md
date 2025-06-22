# AI 이미지 프롬프팅 완전 학습 가이드

## 📚 학습 개요

이 가이드는 AI 이미지 생성(특히 DALL·E 3, Midjourney 등)에서 고품질 이미지를 만들기 위한 체계적인 프롬프팅 방법을 단계별로 학습할 수 있도록 구성되었습니다.

---

## 🎯 핵심 원리: 사진 디테일의 5가지 요소

AI 이미지 생성에서 고려해야 할 핵심 요소들:

1. **구도, 동작, 배경, 심도**
2. **조명(광제어), 광원 색조 분리, 색상 대비** 
3. **카메라 세팅(조리개, 색온도, 필터)**
4. **질감, 입자 효과**
5. **감정/표정 디테일**

---

## 📖 단계별 학습 과정

### 1단계: 동작과 포즈 지정하기

**목적**: 원하는 자세와 동작을 정확히 표현하기

**방법**:
- 구체적인 포즈 설명 사용
- 참고 이미지가 있다면 "posemy.art" 같은 도구로 포즈를 텍스트로 변환
- 신체 부위별 위치 명시

**실습 예시**:
```
❌ 나쁜 예: "여자가 춤추고 있다"
✅ 좋은 예: "젊은 여성이 오른팔을 위로 올리고 왼쪽 다리를 구부린 채 발레 아라베스크 자세를 취하고 있다"
```

### 2단계: Positive/Negative 프롬프트 활용

**목적**: 원하지 않는 요소 제거하고 원하는 요소 강화

**핵심 개념**:
- **Positive**: 그리고 싶은 요소들
- **Negative**: 그리지 말아야 할 요소들 (단어로 명시)

**프롬프트 템플릿**:
```
#상황
다음 프롬프트 기반으로 그림을 그리려 합니다. GPT 4O 기반 그림 생성에 최적화된 프롬프트로 변경해 주세요.

#지시
- Negative Prompt를 명시할 것
- 세부적인 빛 조건이나 비율 크기 지정
```

**실습 예시**:
```
Positive: "beautiful woman, elegant dress, natural lighting"
Negative: "blurry, low quality, distorted face, extra limbs, bad anatomy"
```

### 3단계: 옷과 재질의 디테일 설정

**목적**: 의상과 소재의 현실감 향상

**핵심 기법**:
- 구체적인 재료 비율 명시
- 빛 반사 특성 고려

**실습 예시**:
```
❌ 나쁜 예: "가죽 재킷"
✅ 좋은 예: "built from 35% leather, 30% Kevlar, 15% spandex, 10% carbon fiber, and 10% mesh로 제작된 미래적 재킷"
```

### 4단계: 고급 조명 및 카메라 설정

**목적**: 전문적인 사진 품질 달성

**설정 가능한 요소들**:
- 초점거리, 화각, 조리개
- 조명구성, 컬러온도
- 백라이트, 셔터속도, ISO 감도
- 배경 깊이

**카메라 설정 표**:

| 스타일 | 조리개 | 초점거리 | 조명 | 컬러온도 | 특징 |
|--------|--------|----------|------|----------|------|
| 인물 포트레이트 | f/1.4-2.8 | 85-135mm | 소프트박스 | 5600K | 얕은 심도, 부드러운 배경 흐림 |
| 풍경 사진 | f/8-11 | 14-35mm | 자연광 | 5200-6500K | 선명한 전체 초점 |
| 제품 사진 | f/8-16 | 50-100mm | 링라이트 | 5000K | 균등한 조명, 그림자 최소화 |
| 드라마틱 | f/2.8-4 | 24-70mm | 강한 측광 | 3200K | 강한 대비, 분위기 있는 그림자 |
| 매크로 | f/8-16 | 100mm+ | 디퓨저 | 5600K | 극도의 세부 묘사 |

**고급 조명 제어 프롬프트**:
```
#목적
이 제품을 세부설정을 통해 최고급으로 보이게 하고 싶습니다. 제어할 수 있는 파라미터들로 자세히 구성하고 최고급 3D 피규어 느낌이 나도록 만들어주세요.

#지시
- 상황별 적절한 프롬프트 3개 추천과 이유를 아래따로 작성
- 최고급 피규어에서 조명 스타일만 다르게 해서 프롬프트 5개 생성해
```

### 5단계: 투시와 앵글 제어

**목적**: 공간감과 역동성 있는 구도 연출

**투시의 핵심 개념**:
- **1점 투시**: 중앙 집중형 구도 (복도, 길 등)
- **2점 투시**: 건물이나 도시 풍경
- **3점 투시**: 극적인 앵글 (고층 빌딩을 아래서 위로)

**중요 키워드들**:
- `vanishing point` (소실점)
- `horizon line` (지평선)
- `low angle view` (로우 앵글)
- `high angle view` (하이 앵글)
- `wide-angle lens` (광각)
- `telephoto lens` (망원)

**추천 투시 세트**:
1. `"one-point perspective, centered composition, corridor, vanishing point at center"`
2. `"two-point perspective, urban street, horizon line at eye level, buildings"`
3. `"three-point perspective, low angle view, skyscrapers, dramatic perspective"`
4. `"high angle view, top-down cityscape, wide-angle lens, detailed environment"`
5. `"telephoto lens effect, compressed depth, distant mountains, soft background blur"`

---

## 🚀 실전 프롬프트 작성 워크플로우

### Step 1: 기본 아이디어 정의
```
주제: 무엇을 그릴 것인가?
인물/객체: 누구 또는 무엇을?
장소/배경: 어디서?
```

### Step 2: 디테일 레이어 추가
```
동작/포즈: 어떤 자세?
의상/재질: 어떤 옷과 소재?
표정/감정: 어떤 기분?
```

### Step 3: 기술적 설정
```
카메라: 앵글, 렌즈, 조리개
조명: 광원, 색온도, 분위기
투시: 1점/2점/3점, 시점
```

### Step 4: 품질 및 스타일
```
화질: 4K, 8K, photorealistic
스타일: 사진, 회화, 일러스트
네거티브: 제외할 요소들
```

---

## 📝 실습 예제: 완성된 프롬프트

### 예제 1: 인물 포트레이트
```
**Positive Prompt:**
A 25-year-old elegant woman with long flowing auburn hair, wearing a dress built from 40% silk, 30% satin, 20% lace, 10% chiffon, sitting gracefully on a vintage velvet armchair, soft smile with contemplative eyes looking slightly to the left, shot with 85mm lens, f/1.8 aperture, natural window lighting from the right side, color temperature 5600K, shallow depth of field, one-point perspective, photorealistic, 4K quality

**Negative Prompt:**
blurry, low quality, distorted face, extra limbs, bad anatomy, overexposed, harsh shadows, artificial lighting, plastic skin, cartoon
```

### 예제 2: 제품 사진
```
**Positive Prompt:**
Luxury watch made from 60% titanium, 25% sapphire crystal, 15% ceramic, floating above black marble surface, dramatic three-point lighting setup, key light from top-left, fill light from right, rim light from behind, color temperature 5000K, shot with 100mm macro lens, f/11 aperture, two-point perspective, highly detailed textures, reflective surfaces, premium commercial photography style, 8K resolution

**Negative Prompt:**
cheap, plastic, blurry, poor lighting, flat, dull, low resolution, amateur photography
```

---

## 🎓 고급 팁과 기법

### DALL·E 3 특화 기법
- **대화형 수정**: "고양이의 눈을 더 파랗게 해줘", "배경에 나무를 추가해줘"
- **구체적 묘사**: 개수, 위치, 색상, 질감, 분위기, 관계 등 상세 명시
- **맥락적 설명**: 단순 나열이 아닌 스토리텔링 방식 활용

### 프롬프트 최적화 체크리스트
- [ ] 주요 객체가 명확히 정의되었는가?
- [ ] 원하지 않는 요소가 네거티브로 지정되었는가?
- [ ] 조명과 카메라 설정이 포함되었는가?
- [ ] 재질과 질감이 구체적으로 명시되었는가?
- [ ] 투시와 구도가 의도에 맞게 설정되었는가?

### 자주 하는 실수들
❌ **피해야 할 것들**:
- 모호한 표현 ("예쁜", "멋진" 등)
- 문장으로 된 네거티브 프롬프트
- 과도한 키워드 나열
- 상충되는 설정 (실내인데 자연광 등)

✅ **권장사항**:
- 구체적이고 측정 가능한 설명
- 단어 기반 네거티브 프롬프트
- 논리적으로 일관된 설정
- 단계적 세밀화 과정

---

## 🔄 반복 학습을 위한 연습 과제

### 초급 과제
1. 같은 인물을 5가지 다른 포즈로 생성
2. 하나의 객체를 3가지 다른 조명으로 촬영
3. 동일한 장면을 다른 투시점으로 표현

### 중급 과제
1. 복잡한 재질 조합으로 의상 디자인
2. 전문 사진 스타일 모방 (패션, 제품, 풍경)
3. 네거티브 프롬프트만으로 문제 해결

### 고급 과제
1. 영화 같은 씬 연출 (조명, 구도, 분위기 통합)
2. 브랜드 콘셉트에 맞는 제품 사진 시리즈
3. 예술 작품 스타일과 사실적 표현의 결합

---

이 가이드를 통해 체계적으로 학습하면 AI 이미지 생성에서 전문적인 결과물을 얻을 수 있습니다. 각 단계를 차근차근 연습하며 자신만의 프롬프팅 스타일을 개발해보세요!