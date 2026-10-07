<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:020617,45:1e1b4b,75:312e81,100:7c3aed&height=200&section=header&text=Anoushka%20Awasthi&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=40&desc=AI%20Systems%20%C2%B7%20Backend%20Architecture%20%C2%B7%20Developer%20Tools&descAlignY=60&descSize=16&descColor=c4b5fd"/>

<a href="https://www.ikyano.tech/"><img src="https://img.shields.io/badge/ikyano.tech-7c3aed?style=for-the-badge&logo=safari&logoColor=white&labelColor=020617"/></a>
<a href="https://www.linkedin.com/in/anoushka-awasthi-a87754247/"><img src="https://img.shields.io/badge/LinkedIn-312e81?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=020617"/></a>
<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/GitHub-1e1b4b?style=for-the-badge&logo=github&logoColor=white&labelColor=020617"/></a>
<a href="mailto:awasthinush2580@gmail.com"><img src="https://img.shields.io/badge/Email-020617?style=for-the-badge&logo=gmail&logoColor=c4b5fd&labelColor=020617"/></a>

<br><br>

**Computer Engineering @ Thapar** · Patiala, India · Research Intern @ Samsung PRISM

`somewhere between an idea and a working system`

</div>

---

## about

I build systems that have to **reason**, not just respond.

Most of my work lives one layer below the interface — multi-agent orchestration, retrieval that actually retrieves, event-driven backends, local inference, and the unglamorous plumbing that keeps all of it from falling over: job queues, backpressure, caching, audit trails.

Currently researching **accent-invariant representation learning for SpeechLLMs** at Samsung PRISM, and building things that remember.

I learn by building, breaking, and rebuilding.

---

## selected wins

<div align="center">

| | | |
|:--|:--|:--|
| 🥇 **1st Place** | Economic Times AI Hackathon 2.0 | 60,000+ participants · 10,000+ teams · 28 finalists |
| 🏆 **Winner** | NioHack 2026 — Niograph Inc., USA | Innovate, Build, Transform |
| 🏆 **Winner** | Samsung PRISM Web Agent Hackathon | 450+ participants · 120+ teams |
| ✨ **Innovation Award** | Agentic AI Hackathon — Ulster University, UK | 150+ teams |

</div>

---

## things I've built

### `SOP Opera` — agentic industrial safety intelligence

> **🥇 1st Place · Economic Times AI Hackathon 2.0**

A multi-agent system that catches **compound** operational risks before high-risk work gets approved. The hard part was never making an LLM answer questions — it was making the system reason over the whole situation at once: gas readings, work permits, isolation state, and worker location, together.

| metric | result |
|:--|:--|
| false negatives | **44.5% → 0%** across 593 labeled cases |
| early detection | hazards surfaced **28 minutes** sooner |

- LangGraph pipeline with conditional agent fan-out for explainable safety decisions
- Hybrid pgvector + SQL retrieval over a clause-level regulatory corpus
- Durable PostgreSQL job queue and non-blocking WebSocket layer with per-client backpressure
- Hash-chained, tamper-evident audit trail on every recorded decision

`Python` `TypeScript` `FastAPI` `LangGraph` `PostgreSQL` `pgvector` `Next.js` `Docker`

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/repo-312e81?style=flat-square&logo=github&logoColor=white"/></a>

---

### `FlowSync` — memory for coding agents

Coding agents can write code. They're not good at remembering *why* that code exists. FlowSync turns project activity into persistent, searchable, branch-aware memory.

```
git diff → Bedrock → decisions · risks · tasks → branch-aware retrieval → your agent
```

| metric | result |
|:--|:--|
| push → search latency | **1.26s median** (p95: 1.60s) |

- Event-driven extraction of decisions, risks, and tasks straight out of git diffs
- VS Code extension + MCP server for context logging and project search
- Branch-aware RAG with DynamoDB caching

`TypeScript` `Python` `AWS Bedrock` `Lambda` `DynamoDB` `S3` `MCP` `Next.js`

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/repo-312e81?style=flat-square&logo=github&logoColor=white"/></a>

---

### `Konta` — your browser remembers, locally

> **🏆 Winner · Samsung PRISM Web Agent Hackathon**

A local-first Chrome extension that turns browsing activity into a private knowledge layer. No giant cloud brain required — the embeddings never leave the device.

- On-device semantic embeddings via Transformers.js + ONNX
- Knowledge graph linking pages by semantic, temporal, and contextual relationships
- Sessionization with context-boundary detection, so unrelated tasks don't bleed into each other

`TypeScript` `React` `IndexedDB` `Transformers.js` `ONNX`

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/repo-312e81?style=flat-square&logo=github&logoColor=white"/></a>

---

### `GINA` — ask questions, get grounded data

Conversational analytics that turns natural language into validated SQL and streams the answer back.

```
"why did revenue drop?" → retrieval → SQL generation → validation → PostgreSQL → streamed insight
```

- Multi-model NL→SQL pipeline with structured outputs and grounded query generation
- SSE streaming with fast-path routing over snapshots and cache restoration
- Multi-turn state, semantic schema correction loops, failure-tolerant SSE error handling

`Next.js` `TypeScript` `Fastify` `PostgreSQL` `Supabase` `SSE`

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/repo-312e81?style=flat-square&logo=github&logoColor=white"/></a>

---

## research

### Accent-Invariant Representation Learning for SpeechLLMs · Samsung PRISM

How do you make a SpeechLLM robust to accented English **without** retraining the whole model?

- Parameter-efficient adaptation: LoRA adapters, MoE dynamic adapter routing, accent-aware front-end encoders
- Benchmarking SALM, Qwen Audio, and SALMONN; speaker-level and accent-level failure analysis to find the weak accents worth adapting to
- Targeting a peer-reviewed publication as the closure deliverable

`PyTorch` `SALM` `Qwen Audio` `SALMONN`

> the goal: make speech models listen to the speaker, not the accent.

---

## outside the terminal

**Research Intern · Samsung PRISM** — *Sept 2026 – Present* · Remote
SpeechLLMs, accented speech, and parameter-efficient adaptation.

**Software Developer Intern · BharatRohan** — *Jul 2026 – Aug 2026* · Gurugram (Remote)
Production geospatial features in React + OpenLayers — vector and raster layers, projections, coordinate reference systems, map interactions, spatial visualization.

---

## the spellbook

<div align="center">

<img src="https://skillicons.dev/icons?i=python,ts,js,cpp,react,nextjs,nodejs,fastapi,pytorch&theme=dark" />
<br>
<img src="https://skillicons.dev/icons?i=postgres,mysql,redis,dynamodb,aws,docker,git,githubactions&theme=dark" />

<br><br>

**thinking** `LLM APIs` `Agentic AI` `RAG` `Embeddings` `Semantic Search` `SpeechLLMs` `LoRA / PEFT` `MCP`

**building** `Event-Driven Systems` `Caching` `Queues` `Backpressure` `Cloud Infrastructure` `VS Code Extensions`

</div>

---

<div align="center">

## github, but make it statistics

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=anoushkawasthi&theme=github_dark" width="90%"/>

<br><br>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=anoushkawasthi&theme=github_dark" height="170"/>
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=anoushkawasthi&theme=github_dark" height="170"/>

</div>

---

<div align="center">

```
      ~~~~~~~~~~~~~~~
    ~~~~~  ◉   ◉  ~~~~~
      ~~~~~~~~~~~~~~~
          ~~~~~~~
            ~~~
             |
           code
```

**welcome to the deep end.**

<br>

<a href="https://www.ikyano.tech/"><img src="https://capsule-render.vercel.app/api?type=soft&color=0:020617,50:312e81,100:7c3aed&height=90&section=header&text=ikyano.tech&fontSize=28&fontColor=ffffff&animation=fadeIn"/></a>

**Patiala, India · 8.78 CGPA · probably building something**

<sub>made with curiosity, caffeine, and questionable amounts of debugging.</sub>

<img src="https://komarev.com/ghpvc/?username=anoushkawasthi&style=flat-square&color=7c3aed"/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,50:312e81,100:020617&height=110&section=footer"/>

</div>
