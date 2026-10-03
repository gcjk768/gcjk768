### Hi, I'm James Koh 👋

**DevSecOps & MLOps engineer in Singapore.** I build the platforms that ship software and models safely: GitLab CI/CD, AWS and Kubernetes, with security and model-quality gates that run in the pipeline instead of in review.

AWS Certified Solutions Architect – Associate · CKA in progress · MTech Software Engineering, NUS-ISS

<a href="https://www.linkedin.com/in/kohguanchinjames/"><img src="https://img.shields.io/badge/LinkedIn-James%20Koh-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<img src="https://img.shields.io/badge/Open%20to-MLOps%20·%20Platform%20·%20DevSecOps%20roles-39D353?style=flat-square" alt="Open to MLOps, Platform and DevSecOps roles" />

## Start here

| Repo | What it shows |
|---|---|
| ⭐ [**careroute-mlops**](https://github.com/gcjk768/careroute-mlops) | The MLOps pipeline I built for a clinical triage model: data validation, a release gate (red-flag recall ≥ 0.95) shared by training and CI, MLflow registry, DVC lineage, Fairlearn and Evidently drift monitoring, canary promotion and drift-triggered retraining |
| ⭐ [**careroute-iac**](https://github.com/gcjk768/careroute-iac) | The infrastructure I built for the same system: Terraform and Terragrunt on AWS ECS Fargate, and a GitLab pipeline with tflint, Checkov, gitleaks and OPA policy gates, a push-only OIDC CI role, manual apply and a scheduled auto-destroy |
| [**careroute-ai**](https://github.com/gcjk768/careroute-ai) | The full system (NUS-ISS team project): multi-agent triage on AWS ECS Fargate, 16 Terraform modules with Terragrunt, and a GitLab DevSecOps/MLSecOps pipeline with 85 jobs |
| [**job-hunter**](https://github.com/gcjk768/job-hunter) | A self-hosted agent on my home NAS that scans 40+ job boards, has an LLM score each posting and drafts applications. A human always decides; it never applies |
| [**python-garminconnect**](https://github.com/gcjk768/python-garminconnect) | A family heart-rate monitor with LLM explanations and a rules fallback, 244 tests and nightly backups |

Every repo has an architecture diagram and a README that explains the design trade-offs.

## What I do at work (NCS, regulated enterprise)

- Own the path to production for a **300-repository, 50+ pipeline** estate: reusable GitLab CI templates, Terraform-managed AWS and zero-downtime EKS/ECS releases.
- Enforce **SonarQube, Fortify, OWASP dependency-check, Nexus IQ and Trivy** as pipeline gates rather than review steps.
- Instrumented all four **DORA metrics**; the data behind it drove a **~35% cut in mean time to deploy**.
- Built an **air-gapped, human-approved self-healing CI agent**: an LLM diagnoses a failed job and opens a draft fix MR, which a person must approve.

## Stack

AWS · Kubernetes (EKS) · Terraform / Terragrunt · GitLab CI · Docker · MLflow · DVC · Evidently · Fairlearn · scikit-learn · Prometheus / Grafana · Elasticsearch · Python · Node.js

<details>
<summary>More projects</summary>

- [ai-tech-news-bot](https://github.com/gcjk768/ai-tech-news-bot): local-first news triage with Ollama and a daily Claude digest
- [photography-sensei](https://github.com/gcjk768/photography-sensei): multi-agent photo critique with Claude Code subagents
- [sg-recipe-bot](https://github.com/gcjk768/sg-recipe-bot) · [sg-food-hunt](https://github.com/gcjk768/sg-food-hunt) · [sg-car-market-tracker](https://github.com/gcjk768/sg-car-market-tracker): scheduled data pipelines on a home NAS
- [wc2026-match-predictor](https://github.com/gcjk768/wc2026-match-predictor): a Poisson xG model with LLM explanations
- [Workout-Rotation](https://github.com/gcjk768/Workout-Rotation): a private Telegram gym coach on my NAS. Claude writes the weekly plans, every plan passes a shoulder-injury check, and Garmin recovery data shapes the day
- [Miles-Chase](https://github.com/gcjk768/Miles-Chase): a KrisFlyer miles tracker. Claude writes daily fare and monthly coach reports to a private Telegram channel
- [Burden-of-Proof](https://github.com/gcjk768/Burden-of-Proof): an agent that makes every Semgrep and Dependency-Check finding prove itself with file and line evidence before anyone triages it
- [SG-Property-Hunter](https://github.com/gcjk768/SG-Property-Hunter): watches the Singapore property market, with all money maths in code and Claude only writing the words
- [Huat-Bot](https://github.com/gcjk768/Huat-Bot) · [Watchbot-Hunter](https://github.com/gcjk768/Watchbot-Hunter) · [x100bot](https://github.com/gcjk768/x100bot): Telegram bots on the NAS for TOTO results, the Singapore luxury watch market and Fujifilm X100VI lessons
- 2023: [FreshBeer-FYP-23](https://github.com/gcjk768/FreshBeer-FYP-23) (led a 4-person final-year project) · [FPS-Game-Unity-Engine](https://github.com/gcjk768/FPS-Game-Unity-Engine)

</details>
