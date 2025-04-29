


# 한국史記꾼 (Hanguk Sagi-kkun)

AI 기반 **맞춤형 한국사 학습 플랫폼**  
**필기 이미지 → 요약 → 음성 → 문제 풀이 → 오답 복습까지 한 번에!**

---



![image](https://github.com/user-attachments/assets/d34d7d52-f9bb-4f1f-9431-76d6bf379066)





## 📌 프로젝트 개요

**한국史記꾼**은 한국사능력검정시험 수험생과 직장인 학습자를 위한  
AI 기반 한국사 학습 서비스입니다.

**출퇴근길이나 자투리 시간**에도  
**귀로 듣고, 문제를 풀고, 반복 학습할 수 있는 환경**을 제공하기 위해 개발되었습니다.

---

## 🎯 주요 기능

| 기능명 | 설명 |
|--------|------|
| 🧠 AI 요약 + 음성 변환 (TTS) | 필기 이미지 업로드 → 요약 → Azure TTS로 음성 생성 |
| 📝 AI 문제 생성 | 시대별 맞춤형 객관식 문제 자동 생성 및 해설 제공 |
| ❌ 오답노트 관리 | 틀린 문제 자동 저장 → 카테고리별 복습 지원 |
| 👤 오늘의 위인 | 매일 한국사 인물과 업적을 랜덤 팝업으로 제공 |

---

## 👥 주요 대상 사용자

- **직장인 학습자**: 이동 중 이어폰으로 한국사 요약 듣기  
- **수험생**: 다양한 문제 풀이와 오답노트 기반 효율적 복습

---

## 🧩 기술 스택

| 분류 | 기술 |
|------|------|
| 프론트엔드 | React, Gradio, SCSS, Creatie 디자인 툴 |
| 백엔드 | FastAPI, Python, RESTful API |
| AI 서비스 | Azure AI Search (RAG), Azure OpenAI GPT-4o, Azure TTS |
| 데이터 저장 | Azure MySQL, Azure Blob Storage |
| 배포/자동화 | GitHub Actions + Azure Web App (CI/CD) |

---

## 🗂️ 프로젝트 구조 (프론트엔드 기준)

```
my-app/
├── public/
├── src/
│   ├── API/                 # API 호출 관리
│   ├── components/          # 탭별 UI 구성
│   ├── styles/              # SCSS/CSS 스타일
│   └── index.js             # 진입점
```

---

## 🚀 설치 및 실행

```bash
# 1. 클론
git clone https://github.com/your-org/hanguk-sagikkun.git
cd hanguk-sagikkun/my-app

# 2. 패키지 설치
npm install

# 3. 개발 서버 실행
npm start
```

---


![image](https://github.com/user-attachments/assets/3125fb28-ef8e-4a19-bd3e-e892216d0c6c)




## 📊 성능 평가 요약


![image](https://github.com/user-attachments/assets/8e6ece50-af80-4f4e-bea4-286e1f8a617a)


- **요약 모델 (ROUGE-L F1)**: 평균 0.68  
- **문제 생성 정확도 (정답 일치율)**: 약 70%  
- **TTS 안정성**: 전 테스트 케이스에서 정상 작동

---

## 🧭 책임 있는 AI 적용 전략

| 항목 | 실천 내용 |
|------|-----------|
| **투명성** | RAG 기반 출처 명시, API/DB 기록 추적 |
| **공정성** | EBS 및 교육 콘텐츠 기반 데이터 구성 |
| **책임성** | 사용자 피드백 기반 기능 개선 및 반복 테스트 |
| **포용성** | TTS 속도/음성 스타일 선택 기능 제공 |
| **보안 및 개인정보 보호** | Azure MySQL 최소 정보만 저장, 서버 내 처리 |

---

## 🌱 향후 발전 방향

- **TTS 고도화** 및 **음성 명령 기반 UI 도입**
- **PWA + WebView 기반 모바일 앱** 개발
- **요약 내용 시각화**, **AI 학습 플래너** 기능 추가
- **오답노트 + 메모/태그 기능** 확장
- **지속 가능한 교육 플랫폼**으로의 발전

---

## 📬 팀 정보

| 이름 | 역할 |
|------|------|
| 김용휘 | 팀장 / ML 설계 / 전체 총괄 |
| [이름] | 프론트엔드 개발 |
| [이름] | AI 요약 모델 구축 |
| [이름] | TTS 및 UI 연동 |
| [이름] | 데이터 수집 및 정제 |
| … | … |

---

## 📝 참고사항

- 본 프로젝트는 **Microsoft AI School** 교육 과정 내 팀 프로젝트로 제작되었습니다.
- 비상업적 목적의 교육/연구용으로만 활용됩니다.

---
