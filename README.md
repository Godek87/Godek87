<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=190&color=0:0d1117,50:1f2a44,100:7c3aed&text=Davlet%20Ataoglu&fontColor=ffffff&fontSize=52&fontAlignY=38&desc=Intelligence%2C%20built%20to%20remember.&descAlignY=60&descSize=18" width="100%" alt="Davlet Ata" />

<a href="https://portfolio.davletvm.workers.dev/">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&duration=2800&pause=900&color=A78BFA&center=true&vCenter=true&width=720&lines=ML+%2F+LLM+Systems+Engineer+%26+Researcher;Agent+memory+%C2%B7+Deep+retrieval+%C2%B7+Calibrated+autonomy;Sole+architect+of+Brain+Engine+%E2%80%94+184K+lines+in+production;20+years%3A+Linux+kernel+%E2%86%92+Kubernetes+%E2%86%92+agents" alt="Typing headline" />
</a>

<p>
  <a href="https://portfolio.davletvm.workers.dev/"><img src="https://img.shields.io/badge/Portfolio-0d1117?style=for-the-badge&logo=cloudflare&logoColor=F38020" alt="Portfolio" /></a>
  <a href="https://brain-engine.davletvm.workers.dev/"><img src="https://img.shields.io/badge/Brain_Engine-7c3aed?style=for-the-badge&logo=probot&logoColor=white" alt="Brain Engine" /></a>
  <a href="https://www.linkedin.com/in/devlet-ataoglu/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:davletvm@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://portfolio.davletvm.workers.dev/assets/davlet-ataoglu-cv.pdf"><img src="https://img.shields.io/badge/CV-PDF-1f2a44?style=for-the-badge&logo=readdotcv&logoColor=white" alt="CV" /></a>
</p>

</div>

## About

I build the **memory and retrieval layers that let LLM agents work over long horizons** — and the calibration and guardrails that decide when an agent is allowed to act on its own.

My background runs through the Linux kernel and virtualization, Kubernetes, developer tools and JavaScript engine performance. That is why my AI work is mostly about state, uncertainty and failure, and less about prompts.

```python
davlet = {
    "now":       "Creator of Brain Engine — memory and decision layer for autonomous operations",
    "research":  ["token-free recall", "bi-temporal knowledge graphs", "learning from incidents"],
    "position":  "recall is reconstruction and association, not text generation",
    "languages": ["Turkish", "Russian", "English", "Serbian"],
    "open_to":   "relocation · pilots · research collaboration",
}
```

## Brain Engine &nbsp;<img src="https://img.shields.io/badge/status-in_production-22c55e?style=flat-square" alt="in production" />

An autonomous agent that runs a short-term rental business without a human in the loop. It reads every incoming message, watches device state, works out what the situation actually is, decides, and acts. It escalates to a human only when its own confidence or the risk of the action says it should.

<div align="center">

| 184K | 725 | 7 | 562 | 6+ | 50+ |
|:---:|:---:|:---:|:---:|:---:|:---:|
| lines of Python | files | memory tiers | eval scenarios, 15 stages | message channels | connected devices |

</div>

```mermaid
flowchart LR
    O([Observe]) --> R([Remember]) --> D([Decide]) --> A([Act]) --> L([Learn])
    L -. outcomes feed back .-> R
    D -- low confidence / high risk --> H{{Human escalation}}
    H --> A

    classDef core fill:#1f2a44,stroke:#7c3aed,stroke-width:2px,color:#ffffff
    classDef human fill:#3b1d6e,stroke:#a78bfa,stroke-width:2px,color:#ffffff
    class O,R,D,A,L core
    class H human
```

<details>
<summary><b>How it works</b></summary>
<br />

| Layer | What is inside |
|---|---|
| **Memory** | Seven tiers over a bi-temporal knowledge graph with soft-invalidate semantics and point-in-time navigation. It answers not just *what is true* but *what did I believe when I made that call*. |
| **Retrieval** | Hybrid dense/sparse search in Qdrant with cross-encoder reranking (bge-reranker-v2-m3 via TEI). One multilingual index serves Russian, Turkish and English. |
| **Harness** | **Brain Graph** — my own agent-graph execution engine for long-lived, resumable, stateful runs over a custom bi-temporal timeline. |
| **Decisions** | DecisionCase → PatternMiner → ConditionSynthesizer → Wilson lower-bound scoring → Validator → RuleStore. Rules are mined from outcomes, not hand-written. |
| **Calibration** | Mondrian conformal prediction and beta calibration, so autonomy rests on real confidence intervals instead of raw model scores. |
| **Evaluation** | 562-scenario taxonomy across 15 stages, RAGAS baselines and an LLM-as-judge harness gating the production path. |
| **Safety** | Six-tier guardrails and an autonomy state machine: `OBSERVE → SEMI_AUTO → AUTOPILOT`. The agent earns write access per scenario class by measured reliability. |
| **Applied ML** | LightGBM + SHAP fraud-risk scoring with per-decision attribution shown to reviewers. |

</details>

## Research

| Project | Status | Idea |
|---|---|---|
| **Memory Engine** | in build | Token-free recall: graph traversal, cross-encoder scoring and a bandit access controller, with **no generative model in the loop**. Builds on ideas from KGERMAR, MemCon, MRAgent, Graphiti and Mem0. |
| **Lessons Store** | research | Learning from incidents the way people do: extract *incident → cause → prescription*, then surface the lesson in structurally similar situations. Behavioral improvement without retraining. |
| **Brain Engine 3.0** | architecture | A computable enterprise platform: eleven composable runtime layers and a MetaModel architecture-search subsystem. Principle: *composable intelligence, deterministic execution*. |

## Career

| Company | Role | What I worked on |
|---|---|---|
| **Brain Engine** | Creator | Memory, MetaModel and decision layers for an enterprise intelligence system. |
| **Cendra** | Founding Engineer · Chief Architect | Chief architect and primary developer of an AI operations platform for property management and short-term rentals. **The product raised $1M in investment.** 6+ unified channels, 50+ home-automation integrations, escalation and on-call layer. |
| **Ruwada AI** | Co-Founder | Zero to product. First generation of Brain Engine; founder-led sales and customer integrations. |
| **Mozilla** | Staff Software Engineer | Test engineering lead for Firefox Telemetry (Python, Docker, BigQuery). JavaScript performance. Monitor team (React, TypeScript, Next.js). Telemetry-informed funnel work contributed to a **54% reduction in user churn**. Co-led Continuous Deployment adoption with a DORA-metrics service catalog. |
| **Opera** | Full Stack Engineer | Recommendation systems and serving infrastructure, Node.js microservices, Opera Mini for Android. Led a team technically and as manager. |
| **Red Hat** | Principal Staff Software Engineer | Core kernel team: Linux kernel for RHEL and Fedora, C, eBPF, clang/LLVM. Kubernetes. |
| **Microsoft** | Staff Software Engineer | .NET platform. First ML/AI work. |
| **Yandex** | Software Engineer | Yandex.Maps, Yandex.Music, search and information retrieval at Yandex Labs. |
| **JetBrains** | Software Engineer | IDE development (WebStorm, PhpStorm), Android tooling. |
| **Parallels** | Linux Kernel Developer | Linux kernel and virtualization: OpenVZ, KVM, memory and device cgroups. |
| **Borland** | Software Engineer | C++ Builder. |

<sub>M.Sc. Computer Science, Bauman Moscow State Technical University · Executive programs: MIT Sloan (Digital Business Strategy), INSEAD (Digital Strategy), Harvard Business School (Digital Transformation)</sub>

## Stack

**Agents & retrieval**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_+_pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![LiteLLM](https://img.shields.io/badge/LiteLLM-111827?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-111827?style=flat-square&logo=modelcontextprotocol&logoColor=white)
![RAGAS](https://img.shields.io/badge/RAGAS-111827?style=flat-square)

**Machine learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![JAX](https://img.shields.io/badge/JAX-5E97F6?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM_+_SHAP-2E7D32?style=flat-square)
![Hugging Face](https://img.shields.io/badge/TEI-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Conformal](https://img.shields.io/badge/Conformal_prediction-6D28D9?style=flat-square)
![Bandits](https://img.shields.io/badge/Contextual_bandits-6D28D9?style=flat-square)

**Systems**

![Linux](https://img.shields.io/badge/Linux_internals-FCC624?style=flat-square&logo=linux&logoColor=black)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![eBPF](https://img.shields.io/badge/eBPF-F9C80E?style=flat-square&logo=ebpf&logoColor=black)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C%2FC++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

## Activity

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Godek87&bg_color=0d1117&color=a78bfa&line=7c3aed&point=ffffff&area=true&area_color=7c3aed&hide_border=true&custom_title=Contribution%20graph" width="100%" alt="Contribution graph" />

<img src="https://streak-stats.demolab.com?user=Godek87&hide_border=true&background=0d1117&ring=7c3aed&fire=a78bfa&currStreakLabel=a78bfa&sideLabels=ffffff&currStreakNum=ffffff&sideNums=ffffff&dates=8b949e&stroke=30363d" height="165" alt="Streak" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Godek87&layout=compact&hide_border=true&bg_color=0d1117&title_color=a78bfa&text_color=ffffff&langs_count=8" height="165" alt="Top languages" />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Godek87/Godek87/output/github-contribution-grid-snake-dark.svg" />
  <img src="https://raw.githubusercontent.com/Godek87/Godek87/output/github-contribution-grid-snake.svg" width="100%" alt="Contribution snake" />
</picture>

</div>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=90&section=footer&color=0:7c3aed,50:1f2a44,100:0d1117" width="100%" alt="" />

<sub>Open to pilots, research collaboration and relocation · <a href="mailto:davletvm@gmail.com">davletvm@gmail.com</a></sub>

</div>
