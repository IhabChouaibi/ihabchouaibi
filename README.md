<div align="center">

<img src="./assets/neon-header.svg" width="100%" alt="Iheb Chouaibi — Backend, Cloud, DevOps and Cybersecurity engineer" />

<br />

<a href="https://github.com/IhabChouaibi"><img src="https://img.shields.io/badge/GitHub-IhabChouaibi-0D1117?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://www.linkedin.com/in/iheb-chouaibi-00b4632a2/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://github.com/recruitment-organisation"><img src="https://img.shields.io/badge/Recruitment-Platform-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Recruitment organization" /></a>

<br /><br />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=18&duration=2200&pause=700&color=22D3EE&center=true&vCenter=true&repeat=true&width=850&height=45&lines=%3E+building+distributed+systems;%3E+shipping+cloud-native+platforms;%3E+securing+every+trust+boundary;%3E+automating+delivery+with+GitOps;%3E+system.status%28%29+%3D+READY" alt="Animated engineering status" />

<p>
  <code>secure by design</code>&nbsp; ◆ &nbsp;
  <code>automated by default</code>&nbsp; ◆ &nbsp;
  <code>observable in production</code>
</p>

</div>

---

## `01 // SYSTEM PROFILE`

<table>
<tr>
<td width="58%" valign="top">

### Hello, I'm Iheb 👋

Backend and cloud engineer based in Tunisia. I design secure distributed systems, build event-driven services, and deliver them through automated cloud-native platforms.

- **Current focus:** platform engineering, GitOps and AI-native backends
- **Core runtime:** Java 21, Spring Boot, Kafka and Kubernetes
- **Security:** Keycloak, OAuth2/OIDC, JWT and RBAC
- **AI systems:** RAG, embeddings, Gemini and pgvector

</td>
<td width="42%" valign="top">

```yaml
identity: Iheb Chouaibi
region: Tunisia
role: Backend / Cloud Engineer
runtime: Kubernetes
delivery: GitOps
status: online
```

</td>
</tr>
</table>

## `02 // TECHNOLOGY MATRIX`

<div align="center">

### Backend & distributed systems

<img src="https://skillicons.dev/icons?i=java,spring,maven,python,kafka&theme=dark" alt="Java, Spring, Maven, Python and Kafka" />

`Java 21` · `Spring Boot` · `Spring Cloud` · `Spring Security` · `OpenFeign` · `Flowable BPMN`

### Platform & delivery

<img src="https://skillicons.dev/icons?i=docker,kubernetes,aws,azure,githubactions,git,github,linux&theme=dark" alt="Cloud and DevOps stack" />

`Docker` · `Kubernetes` · `Helm` · `Argo CD` · `GitOps` · `GitHub Actions`

### Data, frontend & intelligence

<img src="https://skillicons.dev/icons?i=postgres,mysql,redis,angular,ts&theme=dark" alt="Data and frontend stack" />

`PostgreSQL` · `pgvector` · `MinIO` · `Angular` · `RAG` · `Gemini`

</div>

---

## `03 // FEATURED SYSTEMS`

<table>
<tr>
<td width="50%" valign="top">

### 🧠 Intelligent Recruitment Platform

An AI-powered recruitment ecosystem combining microservices, semantic analysis, workflow automation and secure identity.

`Spring Boot` `Angular` `Keycloak` `Kafka` `Flowable` `MinIO` `pgvector` `Gemini`

<br />

<a href="https://github.com/recruitment-organisation"><img src="https://img.shields.io/badge/Explore_Platform-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Explore platform" /></a>

</td>
<td width="50%" valign="top">

### ☸️ Recruitment GitOps

Declarative Kubernetes delivery with reusable Helm charts, environment overlays, automated synchronization and self-healing.

`ApplicationSets` `Helm` `Argo CD` `Kubernetes` `GitOps` `Ingress`

<br />

<a href="https://github.com/recruitment-organisation/recruitment-gitops"><img src="https://img.shields.io/badge/Open_GitOps-F97316?style=for-the-badge&logo=argo&logoColor=white" alt="Open GitOps repository" /></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🤖 RAG Service

Document ingestion, semantic retrieval and AI-assisted candidate analysis backed by vector search.

`Spring AI` `Gemini` `Embeddings` `PostgreSQL` `pgvector`

<br />

<a href="https://github.com/recruitment-organisation/rag-service"><img src="https://img.shields.io/badge/Open_RAG_Service-10B981?style=for-the-badge&logo=github&logoColor=white" alt="Open RAG service" /></a>

</td>
<td width="50%" valign="top">

### 👥 HRMS Platform

Event-driven services for employee lifecycle, recruitment, leave, attendance, identity and access control.

`Microservices` `Kafka` `MinIO` `Kubernetes` `GitOps` `RBAC`

<br />

<a href="https://github.com/hrms-organisation"><img src="https://img.shields.io/badge/Explore_HRMS-DB2777?style=for-the-badge&logo=github&logoColor=white" alt="Explore HRMS" /></a>

</td>
</tr>
</table>

## `04 // PLATFORM TOPOLOGY`

```mermaid
flowchart TB
    U[Users] --> UI[Angular Frontend]
    UI --> GW[API Gateway]

    GW --> AUTH[Identity]
    GW --> CORE[Business Services]
    GW --> AI[AI Services]

    AUTH --> KC[Keycloak]
    CORE --> KAFKA[Kafka]
    CORE --> DATA[(PostgreSQL / MinIO)]
    AI --> VDB[(pgvector)]
    AI --> LLM[Gemini]

    classDef edge fill:#0891B2,color:#fff,stroke:#67E8F9,stroke-width:2px
    classDef service fill:#312E81,color:#fff,stroke:#A78BFA,stroke-width:2px
    classDef data fill:#064E3B,color:#fff,stroke:#34D399,stroke-width:2px
    classDef ai fill:#831843,color:#fff,stroke:#F472B6,stroke-width:2px

    class U,UI,GW edge
    class AUTH,CORE,KC,KAFKA service
    class DATA,VDB data
    class AI,LLM ai
```

## `05 // DELIVERY PIPELINE`

```mermaid
flowchart LR
    CODE[Code] --> PR[Pull Request]
    PR --> CI[CI & Tests]
    CI --> IMG[Versioned Image]
    IMG --> GIT[GitOps Repository]
    GIT --> ARGO[Argo CD]
    ARGO --> K8S[Kubernetes]
    K8S --> OBS[Observe]
    OBS -. feedback .-> CODE

    classDef source fill:#312E81,color:#fff,stroke:#A78BFA
    classDef build fill:#0E7490,color:#fff,stroke:#22D3EE
    classDef deploy fill:#9A3412,color:#fff,stroke:#FDBA74
    classDef run fill:#065F46,color:#fff,stroke:#6EE7B7

    class CODE,PR source
    class CI,IMG build
    class GIT,ARGO deploy
    class K8S,OBS run
```

## `06 // SECURITY & AI`

<table>
<tr>
<td width="50%" valign="top">

### 🔐 Explicit trust boundaries

```text
user → authentication → identity provider
                         ↓ signed token
gateway → resource server → business API
```

OAuth2 · OIDC · JWT · RBAC · resource servers · least privilege

</td>
<td width="50%" valign="top">

### ✨ Retrieval-augmented intelligence

```text
PDF → extract → chunk → embed → pgvector
                                  ↓
query → embed → retrieve → Gemini → score
```

Semantic search · grounded generation · workflow automation

</td>
</tr>
</table>

---

## `07 // GITHUB TELEMETRY`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=IhabChouaibi&show_icons=true&hide_border=true&bg_color=00000000&title_color=22D3EE&icon_color=F59E0B&text_color=E2E8F0&ring_color=7C3AED&include_all_commits=true" />
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=IhabChouaibi&show_icons=true&hide_border=true&title_color=0369A1&icon_color=D97706&text_color=334155&ring_color=7C3AED&include_all_commits=true" alt="GitHub statistics" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=IhabChouaibi&layout=compact&langs_count=8&hide_border=true&bg_color=00000000&title_color=F472B6&text_color=E2E8F0" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=IhabChouaibi&layout=compact&langs_count=8&hide_border=true&title_color=BE185D&text_color=334155" alt="Top languages" />
</picture>

<br /><br />

<img width="96%" src="https://github-readme-activity-graph.vercel.app/graph?username=IhabChouaibi&bg_color=0D1117&color=22D3EE&line=7C3AED&point=F59E0B&area=true&area_color=DB2777&hide_border=true&custom_title=Contribution%20Telemetry" alt="Contribution activity graph" />

</div>

<details>
<summary><b>⚡ Open the command center</b></summary>

```bash
mvn test
docker build .
helm template ./chart
argocd app sync recruitment
kubectl get pods -A
```

</details>

<br />

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=17&duration=1900&pause=650&color=F472B6&center=true&vCenter=true&width=850&height=45&lines=build+what+matters;automate+what+repeats;secure+what+connects;observe+what+runs;ship+with+confidence" alt="Engineering principles" />

### `THE SYSTEM IS NEVER FINISHED — ONLY ITERATED.`

<img src="https://capsule-render.vercel.app/api?type=waving&height=130&section=footer&color=0:F59E0B,25:DB2777,50:7C3AED,75:0891B2,100:020617" width="100%" alt="Footer" />

</div>
