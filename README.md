# 개발자 김창현
**빠른 실행**과 **유연한 계획 조정**으로 서비스를 만들어가는 개발자입니다.  
계획을 세우고 바로 실행하고, 막히면 방향을 바꾸는 것을 두려워하지 않습니다.  
할 일이 끝나면 다음 할 일을 이미 정해놓는 사람입니다.

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

---

## Projects

### Viva — 진료기록 기반 AI 생활습관 가이드 서비스
> 건강검진·진료기록·처방전을 기반으로 복약·식단·운동·수면 가이드를 자동 생성하는 반응형 웹 서비스

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

#### 주요 기능 목록
- 혈압·혈당·콜레스테롤·BMI 수치 조합으로 8개 위험군 분류 및 개인 맞춤 식단 플랜 매핑 엔진 직접 설계
- 식단·복약·수면 AI 가이드 자동 생성 구현 (임상진료지침 RAG 검색 → GPT-4o-mini 생성 → 파싱 → DB)
- CLOVA OCR 처방전 자동 인식 구현 (요양기관·환자명·진단코드·처방약 목록 등 14개 필드 추출, 텍스트·좌표 이중 검증)
- DUR 안전성 검사 5종 구현 (동일성분 중복·병용금기·회수약·1일 최대량 초과·효능군 중복, BLOCK/WARN/INFO 3단계)
- 건강검진·처방약·식단·수면 컨텍스트 기반 멀티턴 챗봇 (20턴 히스토리, OpenAI Web Search 연동)
- JWT + Google OAuth 2.0 인증 시스템 전체 구현 (Access 30분 / Refresh 14일)
- APScheduler + FCM 푸시 알림 기반 복약 알림 시스템 구현

**GitHub URL**: https://github.com/AI-HealthCare-03/AH_03_06

---

### 의료 진단 및 위치 기반 병원/의사 탐색 플랫폼

> 증상 입력으로 질병·진료과를 예측하고, 위치 기반으로 병원과 의사를 탐색하는 의료 정보 서비스

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

- 공개 의료 데이터의 한계로, 네이버 지식인 크롤링(54,570건)과 GPT-4o Zero-Shot 증강을 결합하여 학습 데이터를 직접 설계 및 구축 → KM-BERT 파인튜닝으로 Top-3 Accuracy 83% 달성
- Flask 예측 서버 신뢰 점수(score) 0.4 미만 시 GPT-4o로 자동 Fallback하는 이중 파이프라인 설계로 예측 커버리지 확보
- 일반 좌표 계산의 정확도 한계로, Hibernate Spatial + JTS 공간 인덱스를 도입하여 진료과·요일·운영시간·거리 복합 필터 검색 구현
- 주관적 리뷰 점수의 신뢰도 문제로, Times Higher Education 대학 순위 기반 학위·수련·직책 유형별 가중치를 결합한 의사 신뢰도 점수 산출 알고리즘 직접 설계

**GitHub**: https://github.com/orgs/cbnu-development-team-tuktak/repositories

---

### 개인 맞춤형 칼로리 소모량 예측 AI

> 신체 및 운동 데이터를 바탕으로 개인화된 칼로리 소모량을 산출하는 회귀 모델

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square)
![Optuna](https://img.shields.io/badge/Optuna-3B4EFF?style=flat-square)

- 단순 피처로는 칼로리 소모의 물리적 메커니즘을 충분히 설명하지 못해, Keytel 공식(BMR 기반 생리학 공식)을 베이스라인으로 설정하고 잔차(Residual)만 트리 모델이 학습하는 구조 설계
- 개인별 운동 패턴 차이를 반영하기 위해 K-Means 군집화로 운동 세션을 세분화하여 파생 변수로 활용
- Optuna 기반 XGBoost·LightGBM·CatBoost·RandomForest 동시 최적화 후 RidgeCV 메타 모델 스태킹으로 예측 오차 최소화

**GitHub**: https://github.com/Lunarian0928/calories-burned-prediction

---

### 심리/행동 데이터 기반 투표율 예측

> 심리·행동 데이터 및 인구통계 정보를 활용한 국가 선거 투표 여부 예측 AI

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Random Forest](https://img.shields.io/badge/Random_Forest-217346?style=flat-square)
![TabNet](https://img.shields.io/badge/TabNet-FF6B35?style=flat-square)

- 단순 응답 점수로는 개인의 점수 부여 편향을 상쇄하지 못해, 심리 문항 간 1:1 교차 비율(Pairwise Ratio) 235개를 파생 변수로 생성하여 상대적 성향 강도를 수치화
- 파생 변수 증가로 노이즈가 늘어남에 따라 RFECV 4-Seed 앙상블로 핵심 피처만 선별, Mach_score(마키아벨리즘 총점)가 압도적 1위 예측 근거로 확인
- 트리 모델의 구조적 사각지대를 보완하기 위해 5 Repeat × 7-Fold 35개 신경망 앙상블을 결합한 이종 앙상블 구조 설계 → 최종 AUC 0.7814 달성

**GitHub**: https://github.com/Lunarian0928/psychological-voting-prediction

---

### 건강검진 데이터 통계 분석 및 시각화

> 대규모 건강검진 데이터를 전처리하고 주요 질환 발병 요인을 EDA로 도출

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Scipy](https://img.shields.io/badge/Scipy-8CAAE6?style=flat-square&logo=scipy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat-square)

- 단순 시각화로는 변수 간 상관관계의 통계적 유의미성을 입증할 수 없어, 단측 검정(p<0.05)을 적용하여 흡연과 동맥경화 지수(AI) 간의 상관관계를 수치로 검증
- 흡연자 집단 내 동맥경화 위험군을 세분화하여 시각화, 집단별 위험도 차이를 명확히 도출

**GitHub**: https://github.com/Lunarian0928/smoking-health-analysis

---

## GitHub Stats

![Profile Summary](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Lunarian0928&theme=dark)

<div>
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Lunarian0928&theme=dark" width="48%"/>
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Lunarian0928&theme=dark" width="48%"/>
</div>

---

## Education & Certifications

- 충북대학교 소프트웨어학부 (2020.03 ~ 2026.02) | GPA 4.12 / 4.5
- 오즈코딩스쿨 AI 헬스케어 캠프 (2025.12 ~ 2026.06)
- 정보처리산업기사 (2024.09)
- 컴퓨터활용능력 2급 (2021.08)
- 워드프로세서 (2022.02)

---

## Contact

- Email: thanks092834@gmail.com
- GitHub: https://github.com/Lunarian0928
