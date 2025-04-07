# RAG 서비스 Ddabong

<div style="display: flex; justify-content: center; gap: 10px;">
    <img src="https://github.com/user-attachments/assets/697c09ab-9f21-4a54-a346-42a97659562b" width="32%" alt="Image 1">
    <img src="https://github.com/user-attachments/assets/03221cb1-b0ec-4b14-9389-a5cf3a19bafe" width="32%" alt="Image 2">
    <img src="https://github.com/user-attachments/assets/92e66bbd-2a35-43ed-9504-2ee9efa6b9c9" width="32%" alt="Image 3">
</div>

https://youtu.be/z_AQmAX-8mE

## 프로젝트 소개

Ddabong은 최신 RAG(Retrieval-Augmented Generation) 기술을 활용한 고성능 챗봇 서비스입니다. 다양한 언어 모델과 임베딩 기술을 통합하여 사용자의 질문에 대해 정확하고 신속한 답변을 제공합니다.


### 핵심 특징

- 다중 LLM 모델 지원 및 실시간 스트리밍 응답
- 사용자 정의 가능한 임베딩 모델과 검색 파라미터
- 멀티 GPU 기반 분산 처리 및 로드밸런싱
- 실시간 문서 참조 하이라이팅
- 고성능 문서 파싱 및 처리

## 기술 스택

### Backend

- **언어**: TypeScript
- **프레임워크**: Nest.js
- **데이터베이스**: MongoDB

### Frontend

- **프레임워크**: React
- **상태 관리**: Zustand
- **스타일링**: SCSS Modules

### AI/ML 구성요소

- **LLM**:
  - GPT
  - Qwen
  - Gemma
  - Varco
  - NeMo
  - Eeve
- **임베딩 모델**:
  - BAAI/bge-m3
  - HIT-TMG/KaLM-embedding-multilingual-mini-instruct-v1
- **벡터 데이터베이스**: Chroma DB
- **모델 서빙**: vLLM

## 주요 기능

### Backend 기능

1. **채팅 로그 관리**
   - 대화 내용 기록 및 분석
   - 성능 개선을 위한 데이터 활용

2. **실시간 데이터 처리**
   - SSE(Server-Sent Events) 기반 실시간 통신
   - 임베딩 진행 상태 및 채팅 스트리밍

3. **보안 및 사용자 관리**
   - SHA-256 기반 API 키 암호화
   - IP/User Agent 기반 블랙리스트 관리
   - 중복 요청 방지 및 접근 제어

4. **RAG API**
   - 다양한 RAG 관련 요청 통합 관리
   - 임베딩, Retriever, Vector Store 관리

5. **LLM 스트리밍 핸들러**
   - 단일 API를 통한 다중 모델 요청 처리
   - 스트리밍 방식의 응답 처리

### Frontend 기능

1. **최적화된 사용자 경험**
   - 데스크톱 환경 최적화 설계
   - 실시간 스트리밍 응답 표시

2. **컴포넌트 기반 설계**
   - 재사용 가능한 UI 컴포넌트
   - SCSS 모듈화를 통한 스타일 관리

3. **상태 관리**
   - Zustand를 활용한 효율적인 상태 관리
   - 전역/로컬 상태의 명확한 구분

### AI/ML 기능

1. **문서 처리 및 검색**
   - 사용자 정의 가능한 청크 크기 및 오버랩
   - 맞춤형 검색 파라미터 설정
   - 앙상블 리트리버 옵션 지원

2. **하이라이트 기능**
   - 참조 문서 자동 하이라이팅
   - 답변 근거의 시각적 표시

## 시스템 아키텍처
<img width="1268" alt="process" src="https://github.com/user-attachments/assets/a8abcdeb-7d8a-45db-b073-24cd2ee07b3b" />

## 배포 환경

- On-premise GPU 서버
- Docker 기반 컨테이너화
- HTTPS 보안 적용
- Nginx 기반 로드밸런싱
- 멀티 GPU 분산 처리 시스템

## 프로젝트 해결 과제

1. **성능 최적화**
   - 멀티스레드 환경에서의 로드밸런싱 구현
   - 대규모 동시 접속 처리

2. **문서 처리 개선**
   - PDF 파싱 정확도 향상
   - 이미지 처리 최적화

## 향후 개선 계획

### Backend
- Monorepo 구조로의 마이그레이션
- 관리자용 통계 기능 구현
- 분산 처리 시스템 확장

### Frontend
- 모바일 환경 지원 확대
- 사용자 인터페이스 개선

### AI/ML
- 추가 언어 모델 통합
- 검색 알고리즘 최적화

## 문의

[연락처 정보 추가 필요.]
