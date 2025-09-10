# 📖 한국사기꾼 (韓國史記꾼) - 맞춤형 한국사 AI 학습 서비스

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932" src="https://github.com/user-attachments/assets/24b435cd-30ed-41ef-9096-a4419bc995cb" />


'한국사기꾼'은 AI 기술을 활용하여 사용자 맞춤형 한국사 학습 경험을 제공하는 웹 애플리케이션입니다. 직접 필기한 노트를 업로드하면 AI가 핵심 내용을 요약하고 음성(TTS)으로 변환해주어, 언제 어디서든 쉽고 재미있게 학습할 수 있도록 돕습니다.


## ✨ 주요 기능 (Features)

### 🧠 AI 요약 및 TTS 변환
사용자가 직접 필기한 학습 노트를 이미지로 업로드하면, AI(OCR, RAG)가 내용을 인식하고 핵심만 요약하여 텍스트와 음성 파일(TTS)로 제공합니다.

### 📝 시대별 맞춤 문제 생성
원하는 한국사 시대를 선택하면, AI가 해당 범위 내에서 맞춤형 문제를 출제하여 실전 감각을 키울 수 있도록 돕습니다.

### ✅ 오답 노트 자동화
AI 문제 풀이에서 틀린 문제는 자동으로 '오답 노트'에 기록되어, 취약한 부분을 집중적으로 반복 학습할 수 있습니다.

### ⭐ 오늘의 위인
매일 접속 시 한국사의 중요 인물을 랜덤으로 소개해 학습 동기를 부여하고 역사 상식을 넓혀줍니다.

## 🛠️ 기술 스택 (Tech Stack)

### Frontend
- React.js
- CSS3/HTML5
- Responsive Design

### Backend & AI
- Python
- FastAPI
- OpenAI GPT API
- OCR (Optical Character Recognition)
- RAG (Retrieval-Augmented Generation)
- TTS (Text-to-Speech)

## ⚙️ 시스템 아키텍처 (System Architecture)

서비스의 전체 기술 구조와 AI 모델의 데이터 처리 흐름은 다음과 같습니다.

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_09" src="https://github.com/user-attachments/assets/dd590e24-a018-4b1e-af91-32007eedec60" />

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_10" src="https://github.com/user-attachments/assets/4e9357ac-837e-4449-b81c-7877677d0368" />


## 📊 모델 성능 평가 (Model Performance)

AI 요약 모델과 RAG 기반 문제 출제 모델의 성능을 객관적인 지표로 측정하여 서비스의 품질을 검증했습니다.

### 성능 측정 결과
<img width="1920" height="1080" alt="KakaoTalk_20250910_164058170" src="https://github.com/user-attachments/assets/78e0ee31-65bb-49c3-994e-fc0c906563ac" />


### 주요 성과 지표

#### AI 요약 구현 개요
- **ROUGE-L F1 Score**: 생성된 요약의 정답 요약과 얼마나 유사한지 수치화한 지표
  - Test 1: **0.667** - 높은 요약 정확도 달성
  - Test 2: **0.6957** - 지속적인 성능 개선 확인

#### 문제 출제 (RAG) 모델  
- **Precision@5**: 검색 결과 상위 5개 중 정답의 포함률 확률
  - Baseline: 0.9 → **Scored: 0.95** (5.6% 향상)
- **MRR (Mean Reciprocal Rank)**: 정답 문서가 검색 결과에서 얼마나 상위에 노출되는지 나타내는 지표
  - Baseline: 0.741 → **Scored: 0.787** (6.2% 향상)

### 핵심 성과
- **요약 품질**: ROUGE-L F1 점수 0.69 이상으로 높은 요약 정확도 확보
- **검색 정확도**: RAG 모델의 Precision@5가 95%로 우수한 문제 출제 품질 달성
- **랭킹 개선**: MRR 지표에서 베이스라인 대비 6.2% 성능 향상

> 📈 **Azure AI Search 기반 RAG 모델과 최적화된 요약 알고리즘을 통해 신뢰할 수 있는 학습 서비스를 구현했습니다.**



### 전체 시스템 아키텍처

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_08" src="https://github.com/user-attachments/assets/3b9054e1-964a-4105-8083-d23aeb353d3e" />


## 📱 서비스 화면 (Screenshots)

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_12" src="https://github.com/user-attachments/assets/25f27721-125e-4cde-9716-975aeefea035" />

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_413" src="https://github.com/user-attachments/assets/7d3d54dd-880f-4555-b41d-6c9bfe05a596" />

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_13" src="https://github.com/user-attachments/assets/35417648-8f14-4373-a37c-039fa908ee7e" />

<img width="1920" height="1080" alt="KakaoTalk_20250910_162352932_14" src="https://github.com/user-attachments/assets/615f2a3b-7db8-4133-96dd-2ce9c6000067" />



## 🎥 시연 영상 (Demo Video)

[![한국사기꾼 시연 영상](https://img.youtube.com/vi/21AjsP_mD0w/0.jpg)](https://youtube.com/shorts/21AjsP_mD0w)



## 🚀 향후 발전 방향 (Future Plans)

### 접근성 강화
- 음성 명령 기반 UI 도입
- 시각장애인 지원 기능 추가

### 서비스 확장
- 요약 내용 도식화 기능
- AI 학습 루틴 플래너 기능 도입

### 서비스 협업
- 타 과목(영어, 과학 등)으로 서비스 확장
- B2B 유료화 모델 모색

---

> 📚 **한국사기꾼**으로 더 스마트하고 효율적인 한국사 학습을 경험해보세요!
