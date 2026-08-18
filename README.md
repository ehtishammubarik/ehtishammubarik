# Ehtisham Mubarik

**Senior Platform & AI Infrastructure Engineer** - Kubernetes, MLOps, and GPU systems in production.
CKA + CKAD certified · 7+ years building cloud and on-prem infrastructure for real-time, AI-native products.

[![Website](https://img.shields.io/badge/Website-ehtishammubarik.com-007AFF?style=flat&logo=google-chrome&logoColor=white)](https://ehtishammubarik.com)
[![Upwork](https://img.shields.io/badge/Upwork-Available%20for%20consulting-14A800?style=flat&logo=upwork&logoColor=white)](https://www.upwork.com/freelancers/ehtishammubarik)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ehtisham%20Mubarik-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ehtisham-mubarik)
[![Email](https://img.shields.io/badge/Email-ehtisham@eprecisio.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:ehtisham@eprecisio.com)

I build the platforms other engineers ship on: multi-tenant Kubernetes control planes, GPU and MLOps pipelines, observability, and the automation that keeps them reliable and cheap to run.

### What I work on

- **Kubernetes platforms** - multi-tenant control planes (Kamaji), GPU orchestration, MetalLB / K3s / Rancher, and bare-metal and air-gapped deployments for data-sovereign environments.
- **AI / MLOps infrastructure** - AWS Bedrock, Ray distributed training and inference, Kubeflow / MLflow / Airflow, model serving, and cost-aware routing.
- **LLM systems for operations** - an SRE harness that ingests alerts, correlates them against logs and metrics, summarizes the incident, and gates remediation behind approval, with token budgets on every run. Built on LangGraph and the Anthropic Claude Agent SDK.
- **Reliability & cost** - Prometheus / Grafana / Loki, SLOs, incident response, and FinOps. Cut AWS spend 60%+ on a real-time gaming platform.

### Selected background

- Senior DevOps across a real-time gaming/AI platform, a Kubernetes automation product for AI/ML teams, and multi-tenant AI platforms (Pulumi/Go modules with per-tenant provisioning and automated teardown).
- Team Lead on a HIPAA-aligned healthcare IoT platform - LoRaWAN device fleets on Kubernetes.
- MSCS; thesis on GPU Cluster Optimization for ML Workloads.

### Tech

![Kubernetes](https://img.shields.io/badge/Kubernetes-326ce5?style=flat&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-623CE4?style=flat&logo=terraform&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat&logo=helm&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat&logo=argo&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078d4?style=flat&logo=microsoft-azure&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat&logo=google-cloud&logoColor=white)

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![Ray](https://img.shields.io/badge/Ray-028cf0?style=flat&logo=ray&logoColor=white)
![Kubeflow](https://img.shields.io/badge/Kubeflow-326ce5?style=flat&logo=kubeflow&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apache-kafka&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangChain%20%2F%20LangGraph-1C3C3C?style=flat&logo=langchain&logoColor=white)

### Open source

Tools I built because I needed them, then made good enough to hand to someone else.

One argument runs through both: **the failure that costs you is the one nothing reported.** A corpus
that silently lost documents, a Terraform repo that passes `validate` and cannot `apply`. Both
projects are built so the pipeline tells you what it did and what it dropped, and both cores are
stdlib only, so they run in a locked-down container or an air-gapped build box.

**[websieve: turn a web crawl into an ML-ready dataset](https://github.com/ehtishammubarik/websieve)** [![PyPI](https://img.shields.io/pypi/v/websieve?color=3775A9&logo=pypi&logoColor=white)](https://pypi.org/project/websieve/) [![CI](https://github.com/ehtishammubarik/websieve/actions/workflows/ci.yml/badge.svg)](https://github.com/ehtishammubarik/websieve/actions/workflows/ci.yml)
> Boilerplate extraction, Gopher/C4 quality filtering, MinHash near-dedup, sharded output. The quality rules adapt to the writing system, so they do not silently reject Chinese, Japanese, Thai, and Korean the way English-derived rules do. Every drop is attributed to a rule, and the counts reconcile.
>
> [PyPI](https://pypi.org/project/websieve/) · [Quickstart](https://github.com/ehtishammubarik/websieve/blob/master/docs/quickstart.md) · [Benchmarks](https://github.com/ehtishammubarik/websieve/blob/master/docs/benchmarks.md) · [Roadmap](https://github.com/ehtishammubarik/websieve/blob/master/ROADMAP.md)

**[stackmason: Terraform repositories that are secure by default](https://github.com/ehtishammubarik/stackmason)** [![PyPI](https://img.shields.io/pypi/v/stackmason?color=3775A9&logo=pypi&logoColor=white)](https://pypi.org/project/stackmason/) [![CI](https://github.com/ehtishammubarik/stackmason/actions/workflows/ci.yml/badge.svg)](https://github.com/ehtishammubarik/stackmason/actions/workflows/ci.yml)
> Answer some questions, get a repository, not a snippet. It **refuses** to emit a data port open to `0.0.0.0/0`, a publicly accessible database, or a committed credential, and there will never be a flag that downgrades a refusal to a warning. A generator multiplies whatever it emits, so the defaults are the product.
>
> [PyPI](https://pypi.org/project/stackmason/) · [Guardrails](https://github.com/ehtishammubarik/stackmason#why-not-just-copy-a-blog-post) · [Roadmap](https://github.com/ehtishammubarik/stackmason/blob/master/ROADMAP.md) · [Contributing](https://github.com/ehtishammubarik/stackmason/blob/master/CONTRIBUTING.md)

Both take contributions. Issues labelled [`good first issue`](https://github.com/ehtishammubarik/websieve/labels/good%20first%20issue) are pre-scoped, and each repo's `CONTRIBUTING.md` says how to claim one so two people do not build it twice.

### Certifications

- Certified Kubernetes Administrator (CKA) - The Linux Foundation
- Certified Kubernetes Application Developer (CKAD) - The Linux Foundation

### Currently

Founder at Eprecisio Technologies. Open to hands-on senior, founding, and forward-deployed engineering roles involving difficult infrastructure problems.

📫 [ehtishammubarik.com](https://ehtishammubarik.com) · [Upwork](https://www.upwork.com/freelancers/ehtishammubarik) · [LinkedIn](https://www.linkedin.com/in/ehtisham-mubarik) · [ehtisham@eprecisio.com](mailto:ehtisham@eprecisio.com)

Eprecisio Technologies: [Website](https://eprecisio.com) · [LinkedIn](https://www.linkedin.com/company/eprecisio/) · [X](https://twitter.com/EprecisioTech) · [Instagram](https://www.instagram.com/eprecisiotech/) · [Facebook](https://www.facebook.com/EprecisioTechnologies)
