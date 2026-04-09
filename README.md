# ALICE (All-In-one Consultant Agent)
정부 R&D 사업계획서 작성을 위한 AI 기반 초격차 컨설팅 에이전트 
<img width="1901" height="1060" alt="image" src="https://github.com/user-attachments/assets/9960653d-18d5-4566-9c56-4ab9181d8242" />

## 1. 프로젝트 개요

기획 의도: 아이디어는 있지만 문서화(제안서 작성)에서 막히는 기획자 및 창업자 혹은 직장인들을 위해 AI가 컨설팅과 초안 작성을 도움.

핵심 가치: 단순 텍스트 생성이 아닌, 분석-생성-검증으로 이어지는 체계적인 멀티 에이전트 시스템 제공.



프로젝트 기간 2025.09.11 ~ 2024.11.11 (14주)

주요 기능 <br>
복잡한 정부 공고문과 양식을 Vision API와 RAG 기술로 정밀 분석하여,
연구자가 행정 업무 대신 연구 본연의 가치에 집중할 수 있도록 돕는 AI 에이전트 서비스입니다

## 2. 시스템 구조 및 아키텍쳐

### ERD 설계
<img width="1802" height="908" alt="image" src="https://github.com/user-attachments/assets/4ad33b3e-38dc-4a14-9a83-340f4cbda7aa" />

### 에이전트 아키텍쳐
<img width="1761" height="979" alt="image" src="https://github.com/user-attachments/assets/2ab0904d-ba8a-4fd0-b8e6-60e5d4173211" />

## 3. 주요 기능 및 시연

### 맞춤형분석
<img width="1665" height="833" alt="image" src="https://github.com/user-attachments/assets/9e9d1eb2-35f0-4472-a405-3b872c7c2d1d" />


### 규격 기반생성
<img width="1737" height="819" alt="image" src="https://github.com/user-attachments/assets/2afa83e8-6740-4ce6-952a-2cf775c5fe08" />


### 정량/정성 검증
<img width="1829" height="907" alt="image" src="https://github.com/user-attachments/assets/358fefe7-26b9-4ee8-863a-c7b024703a06" />

### 화면구성
<img width="1782" height="909" alt="image" src="https://github.com/user-attachments/assets/bd8f6f79-0ea2-4711-a6d0-656ca3f3a589" />



## 4. 문제 해결 및 학습 내용 (Troubleshooting)

| 항목 | 내용 |
| :--- | :--- |
| **문제 상황** | **AI 학습용 정량적 데이터(정답 셋) 부족** <br> 정부 제안서의 경우 우수 사례 데이터가 공개되지 않거나 보안상 수집이 어려워 학습 데이터가 절대적으로 부족함 |
| **원인 분석** | 단순 데이터 학습(Fine-tuning)만으로는 정부 지원 사업 특유의 엄격한 규격과 법률적 요건을 충족하는 고품질 제안서 생성이 불가능함 확인 |
| **해결 방법** | **데이터 부족을 '분석-생성-검증' 아키텍처로 극복** <br> 1. 공고문의 세부 요건을 극도로 상세하게 분석하는 프로세스 구축 <br> 2. 분석 결과를 바탕으로 공고문과 관계법령에 어긋남이 없는지 자가 검증하는 멀티 에이전트 워크플로우 설계 |
| **최종 검증** | **실무 전문가 검증 완료** <br> 시스템이 도출한 결과물을 바탕으로 **인간 전문가(현업 종사자)를 방문하여 자문 및 검증 진행**, 실무에서 즉시 활용 가능한 수준의 논리 구조와 품질을 갖췄음을 확인 |
| **배운 점** | 데이터의 양적 한계를 **정교한 아키텍처 설계**와 **현장 기반의 피드백**을 통해 극복하는 실무적 해결 능력을 배양함 |



### 5. 차별성 및 기대효과

데이터 확장성 (RAG): 우수 사례를 직접 입력하여 즉시 학습 참조 자료로 활용 가능

정밀한 법적 검토: Vision API를 통한 공고문 밀착 분석으로 행정적 결격 사유 방지

80% 시간 절감: 1~2주 소요되던 기획 업무를 수 시간 내로 단축하여 효율 극대화

전문가 검증 완료: 현업 컨설턴트 자문을 통해 실무 활용 가능성 및 논리 구조 검증

차별성 ( vs LLM)
<img width="1024" height="531" alt="image" src="https://github.com/user-attachments/assets/a1420eef-7662-456c-b1a1-21125a94881b" />
<img width="1023" height="525" alt="image" src="https://github.com/user-attachments/assets/2b3df9ac-9a8b-4a1d-9cd6-5040dae49cf9" />


추후계획
<img width="1024" height="500" alt="image" src="https://github.com/user-attachments/assets/688e1815-4ced-4b9b-a87e-685155a4b9fa" />
<img width="1024" height="519" alt="image" src="https://github.com/user-attachments/assets/97c174c5-16b6-4eef-9cf9-cc122aa323a5" />



### 기술스택

| 구분 | 내용 |
| :--- | :--- |
| **사용 언어** | ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) |
| **프레임워크** | ![Spring Boot](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) |
| **AI 에이전트** | ![LangGraph](https://img.shields.io/badge/LangGraph-FF6F00?style=for-the-badge&logo=chainlink&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white) ![OpenAI](https://img.shields.io/badge/GPT--4o_Vision-412991?style=for-the-badge&logo=openai&logoColor=white) |
| **데이터베이스** | ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white) ![ChromaDB](https://img.shields.io/badge/ChromaDB-5233EA?style=for-the-badge&logo=googlecloud&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white) |
| **개발 및 협업** | ![MyBatis](https://img.shields.io/badge/MyBatis-black?style=for-the-badge) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white) |

### 팀원 소개

| <img src="이미지주소" width="100"> | <img src="이미지주소" width="100"> | <img src="이미지주소" width="100"> | <img src="이미지주소" width="100"> |
| :---: | :---: | :---: | :---: |
| **김태준** | **이민지** | **조수연** | **문준현** |
| UI, Frontend, AI | Frontend, AI | Backend, AI | Backend, DB, AI |
| [![github](https://img.shields.io/badge/github-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/jakemoti0n) | [![github](https://img.shields.io/badge/github-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/깃허브ID) | [![github](https://img.shields.io/badge/github-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/깃허브ID) | [![github](https://img.shields.io/badge/github-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/깃허브ID) |

