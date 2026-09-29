<!-- ====================== HEADER ====================== -->
<a href="https://github.com/gcjk768">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,100:1A472A&height=210&section=header&text=~%2Fjames%20%E2%9D%AF%20whoami&fontSize=46&fontColor=39D353&desc=Platform%20Engineering%20%C2%B7%20DevOps%20%C2%B7%20Kubernetes%20%C2%B7%20DevSecOps%20%C2%B7%20AI&descSize=16&descAlignY=72&animation=fadeIn&fontAlignY=42" alt="header" />
</a>

<div align="center">

<img src="https://readme-typing-svg.demolab.com/?lines=%24+.%2Fdeploy.sh+--env+prod;I+build+golden+paths+teams+ship+on;300+repos+%C2%B7+50%2B+pipelines+%C2%B7+DORA-instrumented;Security+gates+in+the+pipeline%2C+not+in+review;AI+inside+the+platform+%E2%80%94+air-gapped%2C+human-approved&font=Fira%20Code&size=21&pause=1200&color=39D353&center=true&vCenter=true&width=640&height=45" alt="typing" />

<p>
  <img src="https://img.shields.io/badge/Platform%20%26%20DevOps%20Engineer-39D353?style=flat-square&logo=gnubash&logoColor=black" alt="Platform & DevOps Engineer" />
  <img src="https://img.shields.io/badge/AWS%20Certified-SAA--C03-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" alt="AWS Certified" />
  <img src="https://img.shields.io/badge/CKA-In%20Progress-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="CKA in progress" />
  <img src="https://img.shields.io/badge/MTech-NUS--ISS-003D7C?style=flat-square" alt="MTech NUS-ISS" />
  <img src="https://img.shields.io/badge/Based%20in-Singapore-EF3340?style=flat-square&logo=googlemaps&logoColor=white" alt="Singapore" />
  <img src="https://komarev.com/ghpvc/?username=gcjk768&style=flat-square&color=39D353&label=Profile+views" alt="views" />
</p>

</div>

<!-- ====================== ABOUT ====================== -->
## `$ whoami`

```bash
$ whoami
James Koh — Platform & DevOps Engineer @ NCS · Singapore

$ cat about.md
"I own the path to production for a 300-repository, 50+ pipeline
 enterprise estate in a heavily regulated environment, and build the
 golden paths other teams ship on."

PLATFORM   = reusable GitLab CI templates · Terraform-managed AWS · zero-downtime EKS/ECS releases
DEVSECOPS  = SonarQube · Fortify SAST · OWASP dep-check · Nexus IQ SBOM · Trivy, enforced as pipeline gates
RELIABILITY= all four DORA metrics instrumented → ~35% cut in mean time to deploy
AI_PLATFORM= agentic self-healing CI: LLM failure analysis + draft fix MRs, air-gapped, human-approved
STUDYING   = Master of Technology in Software Engineering, NUS-ISS

$ echo "principle"
"Enforce it in the platform, not in review. Automate with intent."
```

<!-- ====================== TECH STACK ====================== -->
## `$ cat tech-stack.sh`

<div align="center">

**⚙️ Cloud, Kubernetes &amp; CI/CD**

<img src="https://skillicons.dev/icons?i=aws,kubernetes,docker,terraform,gitlab,githubactions,linux,bash&theme=dark" alt="cloud kubernetes ci/cd" />

**📊 Observability &amp; Languages**

<img src="https://skillicons.dev/icons?i=elasticsearch,grafana,prometheus,python,nodejs,react,java,go&theme=dark" alt="observability & languages" />

**🛡️ DevSecOps &amp; 🤖 AI**

<img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white" alt="SonarQube" />
<img src="https://img.shields.io/badge/Trivy-1904DA?style=for-the-badge&logo=aqua&logoColor=white" alt="Trivy" />
<img src="https://img.shields.io/badge/OWASP%20ZAP-000000?style=for-the-badge&logo=owasp&logoColor=white" alt="OWASP ZAP" />
<img src="https://img.shields.io/badge/Backstage-9BF0E1?style=for-the-badge&logo=backstage&logoColor=black" alt="Backstage" />
<img src="https://img.shields.io/badge/Claude%20API-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude API" />
<img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama" />
<img src="https://img.shields.io/badge/MCP-1E1E1E?style=for-the-badge" alt="MCP" />

</div>

<!-- ====================== PLATFORM WORK ====================== -->
## `$ kubectl get platform --all-namespaces`

> Production platform work at NCS. The code is private, so here is what each piece does.

| Project | What it does | Stack |
|---|---|---|
| 🩺 **Agentic Self-Healing CI Pipeline** | Two-phase agent inside GitLab CI: an LLM diagnoses the failure behind an 80% confidence gate, then opens a **Draft** MR with the YAML fix on an isolated branch. It never auto-merges. Runs air-gapped on CPU-only runners with no external API calls. | GitLab CI · Docker · Qwen3-Coder (Ollama) · Node.js · Python |
| 📈 **Pipeline Health & DORA Dashboard** | Live DORA metrics across 50+ pipelines, AI-assisted failure analysis, and a Library & Threat Radar that scores dependency risk. The data it surfaced drove the ~35% cut in mean time to deploy. | Node.js · React 18 · GitLab API · Elasticsearch |
| 🏗️ **Backstage IaC Self-Service Portal** *(proposal)* | Self-service infra provisioning: Backstage front door, Terraform/Terragrunt modules, GitLab CI execution, and a Claude template-selection layer scoped to the approved module library. | Backstage · Terraform · Terragrunt · GitLab CI |

<!-- ====================== PROJECTS ====================== -->
## `$ ls ~/projects`

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🔐 <a href="https://github.com/gcjk768/llmapp09">llmapp09 · LLMSecOps pipeline</a></h3>
      <p>Multi-model LLM API + web frontend, containerised and deployed to Kubernetes behind an end-to-end GitHub Actions pipeline: lint, unit tests, Trivy scanning, Promptfoo prompt evals, DeepEval LLM-as-judge, and image publishing. (NUS-ISS DOAIS)</p>
      <img src="https://img.shields.io/badge/-GitHub%20Actions-2088FF?style=flat-square" />
      <img src="https://img.shields.io/badge/-Kubernetes-326CE5?style=flat-square" />
      <img src="https://img.shields.io/badge/-Trivy-1904DA?style=flat-square" />
      <img src="https://img.shields.io/badge/-FastAPI-009688?style=flat-square" />
    </td>
    <td width="50%" valign="top">
      <h3>🧭 <a href="https://github.com/gcjk768/job-hunter">job-hunter</a></h3>
      <p>Self-hosted job-search agent running 24/7 in Docker on my home NAS. It sweeps job boards and ATS career pages, has an LLM judge each new posting's fit, drafts a tailored resume and cover letter, and sends a Telegram alert. A human decides every time: it never applies.</p>
      <img src="https://img.shields.io/badge/-Docker%20%C2%B7%20NAS-2496ED?style=flat-square" />
      <img src="https://img.shields.io/badge/-Ollama%20Cloud-000000?style=flat-square" />
      <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square" />
      <img src="https://img.shields.io/badge/-Telegram-26A5E4?style=flat-square" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🚗 <a href="https://github.com/gcjk768/sg-car-market-tracker">sg-car-market-tracker</a></h3>
      <p>Daily Singapore car-market pipeline. It scrapes COE results, used listings (Sgcarmart, Carro, Motorist) and EV price lists with Playwright, filters them against your criteria, runs a total-cost-of-ownership engine, and sends a Telegram report.</p>
      <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square" />
      <img src="https://img.shields.io/badge/-Playwright-2EAD33?style=flat-square" />
      <img src="https://img.shields.io/badge/-Docker-2496ED?style=flat-square" />
    </td>
    <td width="50%" valign="top">
      <h3>🍽️ <a href="https://github.com/gcjk768/sg-food-hunt">sg-food-hunt</a></h3>
      <p>Staged data pipeline for Singapore dining venues. It collects, dedups and scores venues from several sources, adds MRT and review analysis, and publishes ranked lists and diff reports to an Obsidian vault. Plain-file storage, NAS-friendly.</p>
      <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square" />
      <img src="https://img.shields.io/badge/-Data%20Pipeline-6E5494?style=flat-square" />
      <img src="https://img.shields.io/badge/-Obsidian-7C3AED?style=flat-square" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🍳 <a href="https://github.com/gcjk768/sg-recipe-bot">sg-recipe-bot</a></h3>
      <p>Scheduled LLM bot on a NAS. Each day it finds one recipe and checks it against strict rules: time and cost caps, a live source URL, and no repeats. A recipe that fails is dropped, never patched. The rest are posted to Telegram.</p>
      <img src="https://img.shields.io/badge/-Claude%20API-D97757?style=flat-square" />
      <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square" />
      <img src="https://img.shields.io/badge/-Docker-2496ED?style=flat-square" />
    </td>
    <td width="50%" valign="top">
      <h3>📰 <a href="https://github.com/gcjk768/ai-tech-news-bot">ai-tech-news-bot</a></h3>
      <p>Local-first AI/tech news bot. It filters 50+ RSS feeds with a local model, archives to Obsidian, and posts a daily Claude digest to Telegram.</p>
      <img src="https://img.shields.io/badge/-MCP-1E1E1E?style=flat-square" />
      <img src="https://img.shields.io/badge/-Ollama-000000?style=flat-square" />
      <img src="https://img.shields.io/badge/-Obsidian-7C3AED?style=flat-square" />
    </td>
  </tr>
</table>

<details>
<summary><b>More projects</b></summary>

- 📸 [photography-sensei](https://github.com/gcjk768/photography-sensei): an agentic photography coach. Telegram-driven Claude Code subagents critique photos, and every claim must point at evidence in the frame or EXIF.
- ⚽ [wc2026-match-predictor](https://github.com/gcjk768/wc2026-match-predictor): a hybrid-LLM World Cup assistant built on a Poisson xG model, with bilingual predictions sent to Telegram, Obsidian and Google Calendar.
- 🍻 [FreshBeer-FYP-23](https://github.com/gcjk768/FreshBeer-FYP-23): a React Native + Node.js/MongoDB app with SmartKeg tracking. I led a 4-person team, and the pilot reached 500+ downloads (SIM-UOW FYP 2023).
- 🎮 [FPS-Game-Unity-Engine](https://github.com/gcjk768/FPS-Game-Unity-Engine): a Unity/C# first-person shooter prototype.

</details>

<!-- ====================== STATS ====================== -->
## `$ git log --stat`

<div align="center">

<img height="165" src="https://streak-stats.demolab.com/?user=gcjk768&hide_border=true&theme=github-dark-green&fire=39D353&currStreakLabel=39D353" alt="streak" />

</div>

<!-- ====================== CONNECT ====================== -->
## `$ ./connect.sh`

<div align="center">

<a href="https://www.linkedin.com/in/kohguanchinjames/"><img src="https://img.shields.io/badge/LinkedIn-James%20Koh-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://github.com/gcjk768"><img src="https://img.shields.io/badge/GitHub-gcjk768-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>

</div>

<!-- ====================== FOOTER ====================== -->
<div align="center"><sub>🐧 <code>$ exit 0</code> — built &amp; shipped from a terminal near you.</sub></div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1A472A,100:0D1117&height=120&section=footer" alt="footer" />
