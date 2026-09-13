# 안녕하세요, Cloud & DevOps 엔지니어 이성규입니다.

> **"인프라를 코드로 정의(IaC)하고, 고가용성과 비용 효율성(FinOps), 관측 가능성(Observability)을 갖춘 클라우드 아키텍처를 설계합니다."**  
> 모놀리식 환경의 3-Tier 분리 리팩토링, EKS 기반 차세대 Gateway API 도입, Karpenter 및 KEDA를 통한 지능형 오토스케일링 경험을 보유하고 있습니다.

<br/>

<p align="left">
  <a href="mailto:leesk000107@naver.com"><img src="https://img.shields.io/badge/Email-leesk000107@naver.com-181717?style=flat-square&logo=naver&logoColor=white"/></a>
  <a href="https://github.com/leesk0007"><img src="https://img.shields.io/badge/GitHub-leesk0007-181717?style=flat-square&logo=github&logoColor=white"/></a>
</p>

---

### 🛠 Cloud & DevOps Toolchain

| Category | Technologies |
| :--- | :--- |
| **Cloud & Infrastructure** | <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/> <img src="https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white"/> <img src="https://img.shields.io/badge/Amazon_EKS-FF9900?style=flat-square&logo=amazon-aws&logoColor=white"/> <img src="https://img.shields.io/badge/Amazon_VPC-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/> |
| **IaC & Automation** | <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white"/> <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white"/> <img src="https://img.shields.io/badge/Atlantis-1E88E5?style=flat-square&logo=terraform&logoColor=white"/> <img src="https://img.shields.io/badge/Shell_Script-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white"/> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> |
| **Container & Orchestration** | <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white"/> <img src="https://img.shields.io/badge/Gateway_API-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/> |
| **Autoscaling & FinOps** | <img src="https://img.shields.io/badge/Karpenter-FF9900?style=flat-square&logo=amazon-aws&logoColor=white"/> <img src="https://img.shields.io/badge/KEDA-D62246?style=flat-square&logo=kubernetes&logoColor=white"/> <img src="https://img.shields.io/badge/Infracost-0D1117?style=flat-square&logo=infracost&logoColor=white"/> <img src="https://img.shields.io/badge/AWS_Spot_Instances-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/> |
| **CI/CD & GitOps** | <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/> |
| **Observability & Testing** | <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white"/> <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white"/> <img src="https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white"/> |
| **Database & Cache** | <img src="https://img.shields.io/badge/PostgreSQL_(CNPG)-4169E1?style=flat-square&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/> |

---

### 🏛 Featured Cloud Architecture Projects

#### 1. [Fundit] 라이브 커머스 리워드 펀딩 인프라 & GitOps 파이프라인
* 트래픽 변동성이 큰 라이브 커머스를 위한 AWS EKS 기반 인프라 구축 및 ArgoCD·Helm 무중단 GitOps 배포 환경을 설계했습니다.
* Terraform & Atlantis로 PR 기반 인프라 자동화 체계를 확립하고, 차세대 Gateway API를 도입해 ALB-파드 직결 라우팅으로 지연 시간을 최적화했습니다.
* **Tech Stack**: `AWS EKS`, `Terraform`, `Atlantis`, `ArgoCD`, `Helm`, `Gateway API`, `Docker`
* **Links**: [Infra Repository](https://github.com/KT-Cloud-Tech-Up-team6/Fundit-Infra) | [GitOps Repository](https://github.com/KT-Cloud-Tech-Up-team6/Fundit-GitOps)

<br/>

#### 2. [MGPZZ] EKS 3-Tier 아키텍처 리팩토링 & 지능형 스케일링
* 모놀리식 구조를 App/Infra/GitOps 3-Tier로 완전 분리하고, Karpenter와 KEDA를 통한 이벤트 기반 지능형 스케일링 환경을 구축했습니다.
* `aws sts` 기반 동적 S3/DynamoDB Lock 모듈화로 상태 충돌을 방지하고, Karpenter Spot 우선 할당 정책을 적용해 컴퓨팅 인프라 비용을 최적화했습니다.
* **Tech Stack**: `AWS EKS`, `Terraform`, `Karpenter`, `KEDA`, `Redis`, `Prometheus`, `Grafana`, `k6`
* **Links**: [Infra Repository](https://github.com/MGPZZ/Infra) | [GitOps Repository](https://github.com/MGPZZ/GitOps)

<br/>

#### 3. [InfraBoys] AIOps 선제적 장애 대응 & FinOps 인프라 파이프라인
* 온프레미스 제어 노드와 퍼블릭 클라우드를 연결하는 하이브리드 아키텍처 환경에서 AIOps 기반 자율형 인프라를 구축했습니다.
* Prometheus 예측 함수를 활용한 선제적 오토스케일링을 구현하고, CI 파이프라인에 Infracost를 연동하여 사전 인프라 예산 산출(FinOps)을 달성했습니다.
* **Tech Stack**: `AWS`, `Terraform`, `Ansible`, `FastAPI`, `Prometheus`, `Infracost`, `AIOps`
* **Links**: [GitHub Repository](https://github.com/leesk0007/InfraBoys)

<br/>


#### 4. [p01_dream_team] 클라우드 인프라 자동화 & 모니터링
* Terraform, Ansible, GitHub Actions를 결합하여 AWS 인프라 자동 프로비저닝 및 FastAPI 무중단 자동 배포 파이프라인을 구축했습니다.
* Prometheus와 Grafana 기반의 메트릭 수집 및 Alert Rule을 구성하고, WAS AMI 이미지 최적화 및 트래픽 부하 대응 오토스케일링 정책을 설계했습니다.
* **Tech Stack**: `AWS`, `Terraform`, `Ansible`, `GitHub Actions`, `Prometheus`, `Grafana`
* **Links**: [GitHub Repository](https://github.com/leesk0007/p01_dream_team)

<br/>

---

### 📈 GitHub Activity

<p align="left">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api?username=leesk0007&show_icons=true&theme=tokyonight&hide_border=true" height="150" alt="GitHub Stats" />
  <img src="https://streak-stats.demolab.com?user=leesk0007&theme=tokyonight&hide_border=true" height="150" alt="GitHub Streak" />
</p>
<p align="left">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=leesk0007&layout=compact&theme=tokyonight&hide_border=true" height="140" alt="Top Langs" />
</p>
