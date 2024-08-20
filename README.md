# 🏝️NLP_team1 - 법률 및 심리 상담 챗봇

## 1. 💡프로젝트 소개
### 🧑‍🤝‍🧑 **팀원**
- **비타민 13기 : 박소언, 서윤**
- **비타민 14기 : 김민율, 김선재, 정은지**

### 🗓️**시기**
- **2024년 여름방학**

### 📍**주제** - **약자를 위한 법률 및 심리 상담 챗봇 생성**
**- 주제선정 이유: 현대 사회에서는 법률과 심리 상담에 대한 필요성이 커지고 있지만, 비용, 접근성, 정보 부족 등의 이유로 사회적 약자들은 이러한 서비스에 접근하기 어렵습니다. 특히 경제적 어려움, 신체적 장애, 언어 장벽 등을 가진 사람들은 법적 보호와 심리적 지원을 받지 못할 위험이 큽니다. 이러한 문제를 해결하기 위해 접근성이 높은 디지털 도구를 통해 이들의 권리와 정신 건강을 보호할 수 있는 방안이 필요합니다.**

### 📍**목표** 
**- 사회적 약자들이 쉽게 접근할 수 있는 법률 및 심리 상담 서비스를 제공하여, 그들의 권리 보호와 심리적 안정을 돕는 것을 목표로 합니다. 이를 통해 정보 불균형을 해소하고, 사회적 안정과 통합에 기여하고자 합니다.**

## 📊2. 데이터 수집
**대화 데이터: 한국어 멀티세션 대화(AI-Hub)**
**심리 데이터: 웰니스 대화 스크립트 데이터셋(AI-Hub)**
**법률 데이터: easylaw_kr**

## 💻3. 모델 학습

**Fine-tuning**
-  

**RAG**
- csvloader활용하여 csv 파일 로드
- RecursiveCharacterTextSplitter 활용하여 텍스트 분할
- 텍스트 정수 벡터로 임베딩- 허깅페이스임베딩 모델 : jhgan/ko-sbert-nli
- FAISS (VECTORDB)에 임베딩 된 데이터 저장
- 유사도 기반 검색(RETRIEVER)


**prompt-engineering**
- AI 프롬프트 26가지 지침 (https://arxiv.org/abs/2312.16171) 참고
- 독자 특성 명시 + 특정 역할 부여
- few-shot
- 구조화 + 구분 기호 사용
- 자연스러운 답변 요구 : 대화체 유도


## 📈4. 주요 성과


## 🔍5. 향후 계획
- RAG에 초점을 맞춘 


## 🧹6. 참조
