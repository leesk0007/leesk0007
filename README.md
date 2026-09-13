# 안녕하세요, Cloud & DevOps 엔지니어 이성규입니다. 👋

> **"인프라를 코드로 정의(IaC)하고, 고가용성과 비용 효율성(FinOps), 관측 가능성(Observability)을 갖춘 클라우드 아키텍처를 설계합니다."**  
> 모놀리식 환경의 3-Tier 분리 리팩토링, EKS 기반 차세대 Gateway API 도입, Karpenter 및 KEDA를 통한 지능형 오토스케일링 경험을 보유하고 있습니다.

<br/>

<p align="left">
  <a href="mailto:leesk000107@naver.com"><img src="https://img.shields.io/badge/Email-leesk000107@naver.com-181717?style=flat-square&logo=naver&logoColor=white"/></a>
  <a href="https://github.com/leesk0007"><img src="https://img.shields.io/badge/GitHub-leesk0007-181717?style=flat-square&logo=github&logoColor=white"/></a>
  <a href="https://linkedin.com"><img src="https://img.shields.io/badge/LinkedIn-Profile-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
</p>

---

### 🛠 Cloud & DevOps Toolchain

| Category | Technologies |
| :--- | :--- |
| **Cloud & Infrastructure** | <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/> <img src="https://img.shields.io/badge/Amazon_EKS-FF9900?style=flat-square&logo=amazon-aws&logoColor=white"/> <img src="https://img.shields.io/badge/Amazon_VPC-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/> |
| **IaC & Automation** | <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white"/> <img src="https://img.shields.io/badge/Atlantis-1E88E5?style=flat-square&logo=terraform&logoColor=white"/> <img src="https://img.shields.io/badge/Shell_Script-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white"/> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> |
| **Container & Orchestration** | <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white"/> <img src="https://img.shields.io/badge/Gateway_API-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/> |
| **Autoscaling & FinOps** | <img src="https://img.shields.io/badge/Karpenter-FF9900?style=flat-square&logo=amazon-aws&logoColor=white"/> <img src="https://img.shields.io/badge/KEDA-D62246?style=flat-square&logo=kubernetes&logoColor=white"/> <img src="https://img.shields.io/badge/AWS_Spot_Instances-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/> |
| **CI/CD & GitOps** | <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/> |
| **Observability & Testing** | <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white"/> <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white"/> <img src="https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white"/> |
| **Database & Cache** | <img src="https://img.shields.io/badge/PostgreSQL_(CNPG)-4169E1?style=flat-square&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/> |

---

### 🏛 Featured Cloud Architecture Projects

#### 1. [Fundit] 라이브 커머스 리워드 펀딩 플랫폼 인프라 & GitOps 파이프라인
> 대규모 동시 접속 및 트래픽 변동성이 큰 라이브 커머스 도메인을 위한 클라우드 인프라 구축 및 GitOps 파이프라인 설계

* **Architecture Highlights**:
  * **Terraform 모듈화 & Atlantis 워크플로우**: PR 기반의 Terraform Plan/Apply 자동화를 통해 팀 내 인프라 변경 이력 추적 및 협업 거버넌스 확립
  * **차세대 Kubernetes Gateway API 도입**: NGINX Ingress의 2단계 라우팅(인그레스 파드 거침) 병목을 해소하고, AWS ALB와 파드를 1단계로 직결하여 네트워크 지연 최소화
  * **ArgoCD 기반 GitOps 배포**: Helm Chart를 구조화하여 애플리케이션 및 인프라 매니페스트를 선언적으로 관리, 무중단 롤링 배포 실현
  * **클라우드 보안 및 거버넌스**: AWS Secrets Manager 비대칭 키(RSA) 기반 인증과 SAST/DAST 보안 점검 파이프라인 구성
* **Tech Stack**: `AWS EKS`, `Terraform`, `Atlantis`, `ArgoCD`, `Helm`, `Gateway API`, `Docker`, `Secrets Manager`
* **Repositories**:
  * [Infra Repository (Terraform)](https://github.com/KT-Cloud-Tech-Up-team6/Fundit-Infra)
  * [GitOps Repository (ArgoCD & Helm)](https://github.com/KT-Cloud-Tech-Up-team6/Fundit-GitOps)
  * [Security Repository (SAST/DAST)](https://github.com/KT-Cloud-Tech-Up-team6/Fundit-Security)

<br/>

#### 2. [MGPZZ] EKS 기반 3-Tier 아키텍처 리팩토링 & 지능형 오토스케일링
> 모놀리식 인프라 구조를 실무 표준 3-Tier (App / Infra / GitOps)로 완전 분리하고, Karpenter와 KEDA를 통한 지능형 스케일링 구축

* **Architecture Highlights**:
  * **3-Tier Git Architecture 리팩토링**: 비즈니스 애플리케이션(`app`), 테라폼 인프라(`infra`), 배포 매니페스트(`gitops`)의 완벽한 관심사 분리
  * **동적 S3 백엔드 프로비저닝**: `aws sts get-caller-identity`를 통해 실행 계정 ID 기반으로 S3 버킷 및 DynamoDB Lock을 동적으로 자동 생성하여 팀원 간 상태 파일 충돌 방지
  * **Karpenter 기반 FinOps 비용 절감**: Node 오토스케일링 시 `capacity-type: spot`을 1순위로 배치하여 인프라 컴퓨팅 비용 최적화 달성
  * **Redis 대기열 & KEDA 이벤트 기반 스케일링**: 대규모 트래픽 발생 시 서버 폭파를 방지하는 가상 대기실(Virtual Waiting Room)을 설계하고 큐 길이에 따른 파드 선제적 스케일아웃 연동
  * **모니터링 & 경보 체계 이원화**: Prometheus & Grafana를 통해 실시간 긴급 장애 알림과 KRR(Kubernetes Resource Report) 리소스 분석 보고 체계를 분리 운영
* **Tech Stack**: `AWS EKS`, `Terraform`, `Karpenter`, `KEDA`, `Redis`, `Prometheus`, `Grafana`, `k6`, `CNPG`
* **Repositories**:
  * [Infra Repository](https://github.com/MGPZZ/Infra)
  * [GitOps Repository](https://github.com/MGPZZ/GitOps)
  * [App Repository](https://github.com/MGPZZ/App)

<br/>

#### 3. [Runify] 러닝 코스 생성 플랫폼 인프라 자동화
> 사용자 그림 기반 러닝 경로 서비스의 AWS 인프라 자동화 프로비저닝 및 지속적 통합/배포 환경 구성
* **Tech Stack**: `AWS`, `Terraform`, `Docker`, `GitHub Actions`
* **Repository**: [Runify Infra](https://github.com/KozzilzzilE/Runify_infra)

---

### 📈 GitHub Activity

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=leesk0007&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="150" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=leesk0007&layout=compact&theme=tokyonight&hide_border=true" height="150" alt="Top Langs" />
</p>
