# gcp_proxy

# 🚀 GCP API Proxy Manager

![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=FastAPI&logoColor=white)

## 📝 프로젝트 개요

**GCP API Proxy Manager**는 Google Cloud Platform의 여러 API 서비스들을 하나의 통합된 엔드포인트로 관리할 수 있는 프록시 서버입니다. 

### 🎯 주요 목적
- **API 통합 관리**: 분산된 GCP API들을 단일 인터페이스로 제공
- **인증 중앙화**: GCP 서비스 계정 인증을 중앙에서 관리
- **요청 라우팅**: 클라이언트 요청을 적절한 GCP API로 자동 라우팅
- **모니터링 & 로깅**: API 호출 패턴 및 성능 모니터링

---

## 🏗️ 아키텍처 (예정)

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Client Apps   │───▶│  Proxy Server   │───▶│   GCP APIs      │
│                 │    │                 │    │                 │
│ • Web Apps      │    │ • Authentication│    │ • Compute API   │
│ • Mobile Apps   │    │ • Request Router│    │ • Storage API   │
│ • CLI Tools     │    │ • Rate Limiting │    │ • BigQuery API  │
│ • ML Pipelines  │    │ • Monitoring    │    │ • Vertex AI API │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

---
<!-- 
## 🚀 주요 기능

### 🔐 **인증 및 보안**
- GCP Service Account 기반 인증
- JWT 토큰 관리
- API Key 검증
- Rate Limiting

### 🔄 **API 라우팅**
- RESTful API 프록시
- GraphQL 쿼리 변환
- 요청/응답 변환
- 에러 핸들링

### 📊 **모니터링**
- 실시간 API 사용량 추적
- 성능 메트릭 수집
- 로그 중앙화
- 알람 및 알림

### ⚡ **성능 최적화**
- 응답 캐싱
- 커넥션 풀링
- 비동기 처리
- 부하 분산

---

## 🛠️ 기술 스택

### **Backend**
- **Python 3.11+**: 메인 개발 언어
- **FastAPI**: 고성능 웹 프레임워크
- **Uvicorn**: ASGI 서버
- **Pydantic**: 데이터 검증

### **GCP 서비스**
- **Cloud Run**: 서버리스 배포
- **Cloud Load Balancer**: 부하 분산
- **Cloud Monitoring**: 모니터링
- **Cloud Logging**: 로깅

### **데이터베이스**
- **Cloud Firestore**: 메타데이터 저장
- **Cloud Memorystore (Redis)**: 캐싱

### **DevOps**
- **Docker**: 컨테이너화
- **Cloud Build**: CI/CD
- **Terraform**: Infrastructure as Code -->

---

## 📋 지원 예정 GCP API

### **Compute & Infrastructure**
- `Compute Engine API`
- `Kubernetes Engine API`
- `Cloud Run API`

### **Data & Analytics**
- `BigQuery API`
- `Cloud Storage API`
- `Dataflow API`

### **AI & Machine Learning**
- `Vertex AI API`
- `AutoML API`
- `Vision AI API`
- `Natural Language AI API`

### **Security & Identity**
- `Identity and Access Management API`
- `Secret Manager API`
- `Security Command Center API`

---

## 🚦 프로젝트 상태

| 구성 요소 | 상태 | 진행률 |
|-----------|------|--------|
| 프로젝트 설정 | 🟡 진행중 | 20% |
| 기본 프록시 서버 | 🔴 미시작 | 0% |
| GCP 인증 모듈 | 🔴 미시작 | 0% |
| API 라우터 | 🔴 미시작 | 0% |
| 모니터링 시스템 | 🔴 미시작 | 0% |
| 문서화 | 🟡 진행중 | 15% |

---

## 📦 설치 및 실행

### **환경 요구사항**
- Python 3.11+
- Google Cloud SDK
- Docker (선택사항)
<!--
### **로컬 개발 환경 설정**
```bash
# 저장소 클론
git clone https://github.com/elfinLily/gcp_proxy.git

# Anaconda 가상환경 생성
conda create -n gcp-proxy-manager python=3.11 -y
conda activate gcp-proxy-manager

# 의존성 설치
pip install -r requirements.txt

# 환경변수 설정
cp .env.example .env
# .env 파일에 GCP 크리덴셜 정보 입력

# 개발 서버 실행
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

---

## 📚 API 문서

서버 실행 후 다음 URL에서 자동 생성된 API 문서를 확인할 수 있습니다:

- **Swagger UI**: `http://localhost:8000/docs`
- **ReDoc**: `http://localhost:8000/redoc`

---

## 🤝 기여하기

1. 이 저장소를 Fork합니다
2. 기능 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add amazing feature'`)
4. 브랜치에 Push합니다 (`git push origin feature/amazing-feature`)
5. Pull Request를 생성합니다

---

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

---

## 👨‍💻 개발자

**공부하는 인간의 연구 프로젝트**

- 이메일: wndms0224@gmail.com

---

## 🔗 관련 링크

- [Google Cloud Platform](https://cloud.google.com/)
- [FastAPI Documentation](https://fastapi.tiangolo.com/)
- [GCP API Reference](https://cloud.google.com/apis/docs/overview)

---

<div align="center">

**⭐ 이 프로젝트가 도움이 되셨다면 스타를 눌러주세요! ⭐**

</div>

 -->