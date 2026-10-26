<div align="center">

<img src=".github/assets/profile-banner.svg" alt="Giselle Da Costa, Cloud Architect and DevOps Lead" width="100%">

<br><br>

![Azure](https://img.shields.io/badge/Azure-0b1f4d?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEzLjA1IDQuMjQgNi41NiAxOC4wNWw1LjAxLS4wMiAxLjAzLTIuMTloNC45bC0xLjYtMi44M2gtMi4wNGwyLjU1LTUuNTV6TTUuMiAxOS42SDFMOC42NSA0LjRoMy4zeiIvPjwvc3ZnPg%3D%3D&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-14306b?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgZD0iTTMgMTRjNSA0IDEzIDQgMTggMCIvPjxwYXRoIGZpbGw9IiNmZmYiIGQ9Ik0xNyAxMi41bDQuNSAxLjItMS42IDQuM3oiLz48dGV4dCB4PSIxMiIgeT0iMTAiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSI4IiBmb250LXdlaWdodD0iNzAwIiBmaWxsPSIjZmZmIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIj5hd3M8L3RleHQ%2BPC9zdmc%2B&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-1d3f8a?style=for-the-badge&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-2456c8?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2f6fe0?style=for-the-badge&logo=githubactions&logoColor=white)
![Python](https://img.shields.io/badge/Python-4a86f0?style=for-the-badge&logo=python&logoColor=white)

</div>

## In numbers

| 15+ | 14 | 7 | 4 |
| :---: | :---: | :---: | :---: |
| years in infrastructure and cloud | public platform repositories | core cloud and Kubernetes certifications | working languages |

## What I do

I build the cloud platforms other teams build on. Landing zones, Terraform modules, GitOps pipelines and Kubernetes platforms that are secure by default and quiet to operate. My work sits where infrastructure, data and AI meet, in industries where reliability and compliance are not optional.

## The platform, end to end

```mermaid
flowchart LR
    subgraph FOUNDATION["fa:fa-layer-group Foundation"]
        LZ["Landing zones<br/>hub and spoke"]
        POL["Policy as code"]
        VEND["Subscription vending"]
    end
    subgraph DELIVERY["fa:fa-code-branch Delivery"]
        GHA["GitHub Actions<br/>OIDC, no secrets"]
        DRIFT["Drift detection"]
    end
    subgraph RUNTIME["fa:fa-cubes Runtime"]
        AKS["AKS and EKS"]
        FLUX["Flux GitOps"]
        GK["Gatekeeper policies"]
    end
    subgraph INSIGHT["fa:fa-chart-line Insight"]
        OBS["Observability<br/>SLOs"]
        FIN["FinOps"]
    end
    VEND --> LZ --> POL
    GHA --> LZ
    GHA --> AKS
    DRIFT --> GHA
    FLUX --> AKS --> GK
    AKS --> OBS
    LZ --> FIN

    classDef found fill:#0b1f4d,stroke:#7fb2ff,stroke-width:2px,color:#ffffff
    classDef deliv fill:#14306b,stroke:#7fb2ff,stroke-width:2px,color:#ffffff
    classDef run fill:#1d3f8a,stroke:#7fb2ff,stroke-width:2px,color:#ffffff
    classDef ins fill:#2456c8,stroke:#cfe0ff,stroke-width:2px,color:#ffffff
    class LZ,POL,VEND found
    class GHA,DRIFT deliv
    class AKS,FLUX,GK run
    class OBS,FIN ins
```

## Repositories

| Repository | What it shows | Stack |
| --- | --- | --- |
| [secure-genai-platform-azure](https://github.com/marlyngiselle/secure-genai-platform-azure) | Enterprise GenAI on Azure behind a private AI gateway: token quotas, managed identity, content safety and full traceability | ![Azure OpenAI](https://img.shields.io/badge/Azure%20OpenAI-0b1f4d?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEzLjA1IDQuMjQgNi41NiAxOC4wNWw1LjAxLS4wMiAxLjAzLTIuMTloNC45bC0xLjYtMi44M2gtMi4wNGwyLjU1LTUuNTV6TTUuMiAxOS42SDFMOC42NSA0LjRoMy4zeiIvPjwvc3ZnPg%3D%3D&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-2456c8?style=flat-square&logo=fastapi&logoColor=white) |
| [databricks-lakehouse-terraform](https://github.com/marlyngiselle/databricks-lakehouse-terraform) | A governed lakehouse: VNet-injected Databricks, Unity Catalog per environment, medallion pipelines shipped as bundles | ![Databricks](https://img.shields.io/badge/Databricks-14306b?style=flat-square&logo=databricks&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-1d3f8a?style=flat-square&logo=terraform&logoColor=white) |
| [fabric-realtime-intelligence](https://github.com/marlyngiselle/fabric-realtime-intelligence) | Real-time industrial telemetry on Microsoft Fabric: Event Hubs, Eventhouse and KQL with anomaly detection, health scores and alert rules | ![Python](https://img.shields.io/badge/Python-4a86f0?style=flat-square&logo=python&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-1d3f8a?style=flat-square&logo=terraform&logoColor=white) |
| [databricks-fabric-lakehouse-bridge](https://github.com/marlyngiselle/databricks-fabric-lakehouse-bridge) | Databricks produces, Fabric consumes: Unity Catalog gold tables exposed through OneLake, governed by data contracts with a breaking-change gate in CI | ![Databricks](https://img.shields.io/badge/Databricks-14306b?style=flat-square&logo=databricks&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-1d3f8a?style=flat-square&logo=terraform&logoColor=white) |
| [enterprise-rag-platform](https://github.com/marlyngiselle/enterprise-rag-platform) | Retrieval-augmented generation the enterprise way: hybrid search with document-level security, grounded answers with citations and an evaluation gate | ![Python](https://img.shields.io/badge/Python-4a86f0?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-2456c8?style=flat-square&logo=fastapi&logoColor=white) |
| [mlops-predictive-maintenance](https://github.com/marlyngiselle/mlops-predictive-maintenance) | From notebook to governed production: MLflow on Databricks, Unity Catalog registry, a champion and challenger gate, Azure ML serving and drift monitoring | ![MLflow](https://img.shields.io/badge/MLflow-14306b?style=flat-square&logo=mlflow&logoColor=white) ![Databricks](https://img.shields.io/badge/Databricks-1d3f8a?style=flat-square&logo=databricks&logoColor=white) |
| [governed-mcp-gateway](https://github.com/marlyngiselle/governed-mcp-gateway) | Safe, governed access for AI assistants to operations tools: role policies, JWT auth, redaction, rate limits and audit logging on MCP | ![Python](https://img.shields.io/badge/Python-4a86f0?style=flat-square&logo=python&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-2456c8?style=flat-square&logo=modelcontextprotocol&logoColor=white) |
| [azure-landing-zone-terraform](https://github.com/marlyngiselle/azure-landing-zone-terraform) | A modular Azure landing zone with hub-and-spoke networking, policy as code and self-service subscription vending | ![Terraform](https://img.shields.io/badge/Terraform-1d3f8a?style=flat-square&logo=terraform&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0b1f4d?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEzLjA1IDQuMjQgNi41NiAxOC4wNWw1LjAxLS4wMiAxLjAzLTIuMTloNC45bC0xLjYtMi44M2gtMi4wNGwyLjU1LTUuNTV6TTUuMiAxOS42SDFMOC42NSA0LjRoMy4zeiIvPjwvc3ZnPg%3D%3D&logoColor=white) |
| [aks-gitops-platform](https://github.com/marlyngiselle/aks-gitops-platform) | An AKS platform run by Flux: ingress, certificates, observability, Gatekeeper policies and namespace-as-a-service | ![Kubernetes](https://img.shields.io/badge/Kubernetes-2456c8?style=flat-square&logo=kubernetes&logoColor=white) ![Flux](https://img.shields.io/badge/Flux-1d3f8a?style=flat-square&logo=flux&logoColor=white) |
| [terraform-github-actions-oidc](https://github.com/marlyngiselle/terraform-github-actions-oidc) | Reusable plan, apply and drift-detection workflows for Azure and AWS, with OIDC and no long-lived secrets | ![Actions](https://img.shields.io/badge/Actions-2f6fe0?style=flat-square&logo=githubactions&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-14306b?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgZD0iTTMgMTRjNSA0IDEzIDQgMTggMCIvPjxwYXRoIGZpbGw9IiNmZmYiIGQ9Ik0xNyAxMi41bDQuNSAxLjItMS42IDQuM3oiLz48dGV4dCB4PSIxMiIgeT0iMTAiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSI4IiBmb250LXdlaWdodD0iNzAwIiBmaWxsPSIjZmZmIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIj5hd3M8L3RleHQ%2BPC9zdmc%2B&logoColor=white) |
| [secure-supply-chain](https://github.com/marlyngiselle/secure-supply-chain) | Signed, scanned and attested containers from commit to cluster, with admission policies that reject anything unverified | ![Sigstore](https://img.shields.io/badge/Sigstore-14306b?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEyIDIgNCA1djZjMCA1IDMuNCA5LjQgOCAxMSA0LjYtMS42IDgtNiA4LTExVjV6Ii8%2BPHBhdGggZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMTQzMDZiIiBzdHJva2Utd2lkdGg9IjIiIGQ9Im04LjUgMTIgMi41IDIuNSA0LjUtNSIvPjwvc3ZnPg%3D%3D&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2456c8?style=flat-square&logo=docker&logoColor=white) |
| [slo-observability-kit](https://github.com/marlyngiselle/slo-observability-kit) | SLOs as code that generate multi-window burn-rate alerts, Grafana dashboards and error-budget policies | ![Prometheus](https://img.shields.io/badge/Prometheus-1d3f8a?style=flat-square&logo=prometheus&logoColor=white) ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-2456c8?style=flat-square&logo=opentelemetry&logoColor=white) |
| [cloud-finops-toolkit](https://github.com/marlyngiselle/cloud-finops-toolkit) | A tested Python CLI that finds cloud waste: idle resources, tag gaps, rightsizing and shutdown schedules | ![Python](https://img.shields.io/badge/Python-4a86f0?style=flat-square&logo=python&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0b1f4d?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEzLjA1IDQuMjQgNi41NiAxOC4wNWw1LjAxLS4wMiAxLjAzLTIuMTloNC45bC0xLjYtMi44M2gtMi4wNGwyLjU1LTUuNTV6TTUuMiAxOS42SDFMOC42NSA0LjRoMy4zeiIvPjwvc3ZnPg%3D%3D&logoColor=white) |
| [platform-ops-toolkit](https://github.com/marlyngiselle/platform-ops-toolkit) | Day-to-day operations in Bash and PowerShell, safe by default, tested and documented | ![Bash](https://img.shields.io/badge/Bash-14306b?style=flat-square&logo=gnubash&logoColor=white) ![PowerShell](https://img.shields.io/badge/PowerShell-2456c8?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjIuNCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBkPSJNNSA2bDYgNi02IDZNMTMgMThoNyIvPjwvc3ZnPg%3D%3D&logoColor=white) |

## Fifteen years, one direction

```mermaid
timeline
    2010 : Banking operations
         : Windows, Linux and Active Directory under PCI DSS
    2013 : Telecom
         : 24/7 infrastructure, disaster recovery
    2015 : First cloud in a bank
         : Hybrid Azure and AWS, Terraform, first CI/CD
    2020 : Energy
         : Greenfield multi-account AWS platform
    2022 : Security at scale
         : Encryption and compliance as code across hundreds of accounts
    2023 : Global platform
         : Azure landing zones and self-service for thousands of developers
    2025 : Industrial data and AI
         : Data, ML and GenAI platforms across plants on four continents
```

## How I work

| Principle | In practice |
| --- | --- |
| Secure by default | Workload identity instead of secrets, private networking, policy enforced by the platform |
| Everything as code | If it can't be reviewed in a pull request, it isn't done |
| Self-service | The best platform request is the one nobody has to open |
| Cost is a feature | Tagging, rightsizing and schedules are designed in, not bolted on |
| Written first | Decision records and runbooks so the next engineer moves fast |

## Certifications

![Azure Solutions Architect Expert](https://img.shields.io/badge/Azure-Solutions%20Architect%20Expert-0b1f4d?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTEzLjA1IDQuMjQgNi41NiAxOC4wNWw1LjAxLS4wMiAxLjAzLTIuMTloNC45bC0xLjYtMi44M2gtMi4wNGwyLjU1LTUuNTV6TTUuMiAxOS42SDFMOC42NSA0LjRoMy4zeiIvPjwvc3ZnPg%3D%3D&logoColor=white)
![AWS Solutions Architect Professional](https://img.shields.io/badge/AWS-Solutions%20Architect%20Professional-14306b?style=flat-square&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgZD0iTTMgMTRjNSA0IDEzIDQgMTggMCIvPjxwYXRoIGZpbGw9IiNmZmYiIGQ9Ik0xNyAxMi41bDQuNSAxLjItMS42IDQuM3oiLz48dGV4dCB4PSIxMiIgeT0iMTAiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSI4IiBmb250LXdlaWdodD0iNzAwIiBmaWxsPSIjZmZmIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIj5hd3M8L3RleHQ%2BPC9zdmc%2B&logoColor=white)
![CKA](https://img.shields.io/badge/CNCF-CKA-1d3f8a?style=flat-square&logo=kubernetes&logoColor=white)
![CKAD](https://img.shields.io/badge/CNCF-CKAD-1d3f8a?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform Associate](https://img.shields.io/badge/HashiCorp-Terraform%20Associate-2456c8?style=flat-square&logo=terraform&logoColor=white)
![GitOps Certified Associate](https://img.shields.io/badge/CNCF-GitOps%20Associate-2f6fe0?style=flat-square&logo=git&logoColor=white)
![Argo Project Associate](https://img.shields.io/badge/CNCF-Argo%20Associate-2f6fe0?style=flat-square&logo=argo&logoColor=white)

<br>

<div align="center">

[LinkedIn](https://www.linkedin.com/in/giselledacosta) · French · English · Spanish · Portuguese

</div>
