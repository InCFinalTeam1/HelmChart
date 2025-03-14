# Final Project Helm Chart 저장소

신세계 I&C 클라우드 엔지니어 양성과정 최종 프로젝트 HelmChart

## 사용 가능한 차트

이 저장소에서는 다음과 같은 Helm 차트를 제공합니다:

| 차트 이름 | 버전 | 설명 |
|------------|---------|-------------|
| final-project-client | 0.1.0 | 인플루언서 클라이언트 애플리케이션 |
| final-project-insight | 0.1.0 | 데이터 분석 및 리포팅 서비스 |
| final-project-main | 0.1.0 | 핵심 애플리케이션 서비스 |
| final-project-user | 0.1.0 | 사용자 관리 및 인증 서비스 |

## 차트 사용 방법

### Helm 저장소 추가하기

```bash
helm repo add final-project https://incfinalteam1.github.io/HelmChart
helm repo update
```

### 차트 설치하기

```bash
# 클라이언트 애플리케이션 설치
helm install client final-project/final-project-client

# 인사이트 서비스 설치
helm install insight final-project/final-project-insight

# 메인 서비스 설치
helm install main final-project/final-project-main

# 사용자 서비스 설치
helm install user final-project/final-project-user
```

## 아키텍처 개요

우리의 마이크로서비스 아키텍처는 다음과 같이 구성되어 있습니다:
능
- **인사이트 서비스**: 분석 및 리포팅 기능
- **메인 서비스**: 핵심 비즈니스 로직 및 애플리케이션 기능
- **사용자 서비스**: 사용자 인증, 권한 부여 및 프로필 관리


