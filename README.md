<div align="center">

<img src="./hero.svg" width="100%" alt="Anoushka Awasthi — AI Systems · Backend Architecture · Developer Tools"/>

<br>

<a href="https://www.ikyano.tech/"><img src="https://img.shields.io/badge/ikyano.tech-071525?style=for-the-badge&logo=safari&logoColor=5EEAD4&labelColor=04070D"/></a>
<a href="https://www.linkedin.com/in/anoushka-awasthi-a87754247/"><img src="https://img.shields.io/badge/LinkedIn-071525?style=for-the-badge&logo=linkedin&logoColor=5EEAD4&labelColor=04070D"/></a>
<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/GitHub-071525?style=for-the-badge&logo=github&logoColor=5EEAD4&labelColor=04070D"/></a>
<a href="mailto:awasthinush2580@gmail.com"><img src="https://img.shields.io/badge/Email-071525?style=for-the-badge&logo=maildotru&logoColor=5EEAD4&labelColor=04070D"/></a>

<br><br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=2600&pause=900&color=5EEAD4&center=true&vCenter=true&width=720&lines=somewhere+between+an+idea+and+a+working+system;multi-agent+systems+that+reason%2C+not+just+respond;retrieval+that+actually+retrieves;local-first+inference+%E2%80%94+no+giant+cloud+brain+required;I+learn+by+building%2C+breaking%2C+rebuilding" alt="rotating tagline"/>

<br>

<img src="./divider.svg" width="100%" alt=""/>

</div>

## `01` &nbsp;about

<table>
<tr>
<td width="62%" valign="top">

I build systems that have to **reason**, not just respond.

Most of my work lives one layer below the interface — multi-agent orchestration, retrieval that actually retrieves, event-driven backends, on-device inference, and the unglamorous plumbing that keeps all of it standing up: durable job queues, backpressure, caching, tamper-evident audit trails.

The interesting problems are rarely "can the model answer this." They're *can the system hold the whole situation in its head at once* — and can you prove afterwards why it decided what it decided.

Right now I'm researching **accent-invariant representation learning for SpeechLLMs** at Samsung PRISM, and building tools that remember.

</td>
<td width="38%" valign="top">

**currently**

`🜂` researching SpeechLLM accent adaptation @ **Samsung PRISM**

`🜁` building memory layers for coding agents

`🜃` 4× hackathon winner — incl. **1st / 60,000+**

<br>

**at a glance**

| | |
|:--|:--|
| 📍 | Patiala, India |
| 🎓 | B.E. Computer Engineering, Thapar |
| 📊 | CGPA **8.78** |
| 🌐 | [ikyano.tech](https://www.ikyano.tech/) |

</td>
</tr>
</table>

<img src="./divider.svg" width="100%" alt=""/>

## `02` &nbsp;impact

<div align="center">
<img src="./metrics.svg" width="100%" alt="0% false negatives, down from 44.5% across 593 labeled cases · 28 minutes earlier hazard detection · 1.26s median push-to-search latency"/>
</div>

<img src="./divider.svg" width="100%" alt=""/>

## `03` &nbsp;selected work

<table>
<tr><td>

### 🜂 &nbsp;SOP Opera
**agentic industrial safety intelligence**

<img src="https://img.shields.io/badge/🥇_1st_Place-Economic_Times_AI_Hackathon_2.0-FFB84D?style=flat-square&labelColor=04070D"/> <img src="https://img.shields.io/badge/60,000%2B_participants-071525?style=flat-square&labelColor=04070D"/> <img src="https://img.shields.io/badge/28_finalists-071525?style=flat-square&labelColor=04070D"/>

A multi-agent system that catches **compound** operational risk before high-risk work gets approved. The hard part was never getting an LLM to answer questions — it was getting the system to reason over the whole situation at once: gas readings, work permits, isolation state, and worker location, *together*. Any one of those looks fine in isolation. The danger lives in the combination.

- **Compound risk engine** fusing four independent operational signals — catches hazards that single-sensor thresholds structurally cannot see
- **LangGraph pipeline** with conditional agent fan-out, so the orchestration shape adapts to the situation instead of running a fixed chain
- **Hybrid pgvector + SQL retrieval** over a clause-level regulatory corpus — every decision cites the clause it rests on
- **Durable PostgreSQL job queue** and a non-blocking WebSocket layer with per-client backpressure
- **Hash-chained audit trail** — tamper-evident record of every safety decision made

<sub>`Python` · `TypeScript` · `FastAPI` · `LangGraph` · `PostgreSQL` · `pgvector` · `Next.js` · `Docker`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/source-071525?style=flat-square&logo=github&logoColor=5EEAD4&labelColor=04070D"/></a>

</td></tr>
</table>

<table>
<tr><td>

### 🜁 &nbsp;FlowSync
**persistent memory for coding agents**

Coding agents can write code. They're not good at remembering *why* that code exists. FlowSync turns raw project activity into searchable, branch-aware institutional memory — so the agent arrives already knowing the decisions, the risks, and what got ruled out.

```
git diff ──▶ Bedrock ──▶ decisions · risks · tasks ──▶ branch-aware retrieval ──▶ your agent
```

- **Event-driven extraction** pulling structured decisions, risks, and tasks straight out of git diffs
- **VS Code extension + MCP server** for context logging, project search, and retrieval inside the editor
- **Branch-aware RAG** with DynamoDB caching — **1.26s median** push-to-search, p95 1.60s

<sub>`TypeScript` · `Python` · `AWS Bedrock` · `Lambda` · `DynamoDB` · `S3` · `MCP` · `Next.js`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/source-071525?style=flat-square&logo=github&logoColor=5EEAD4&labelColor=04070D"/></a>

</td></tr>
</table>

<table>
<tr><td>

### 🜃 &nbsp;Konta
**your browser remembers — locally**

<img src="https://img.shields.io/badge/🏆_Winner-Samsung_PRISM_Web_Agent_Hackathon-5EEAD4?style=flat-square&labelColor=04070D"/> <img src="https://img.shields.io/badge/450%2B_participants-071525?style=flat-square&labelColor=04070D"/>

A local-first Chrome extension that turns browsing activity into a private knowledge layer. The embeddings never leave the device — no giant cloud brain required, and nothing to trust anyone with.

- **On-device semantic embeddings** via Transformers.js + ONNX, running entirely in the browser
- **Knowledge graph** linking pages across semantic, temporal, and contextual relationships
- **Sessionization with context-boundary detection**, so unrelated tasks stop bleeding into each other

<sub>`TypeScript` · `React` · `IndexedDB` · `Transformers.js` · `ONNX`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/source-071525?style=flat-square&logo=github&logoColor=5EEAD4&labelColor=04070D"/></a>

</td></tr>
</table>

<table>
<tr><td>

### 🜄 &nbsp;GINA
**ask questions, get grounded data**

Conversational analytics that turns natural language into *validated* SQL and streams the answer back — with the schema correcting itself when the question and the database disagree.

```
"why did revenue drop?" ──▶ retrieval ──▶ SQL generation ──▶ validation ──▶ PostgreSQL ──▶ streamed insight
```

- **Multi-model NL→SQL pipeline** with structured outputs and grounded query generation
- **SSE streaming** with fast-path routing over snapshots and cache restoration
- **Multi-turn conversation state**, semantic schema correction loops, failure-tolerant SSE error handling

<sub>`Next.js` · `TypeScript` · `Fastify` · `PostgreSQL` · `Supabase` · `SSE`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/source-071525?style=flat-square&logo=github&logoColor=5EEAD4&labelColor=04070D"/></a>

</td></tr>
</table>

<img src="./divider.svg" width="100%" alt=""/>

## `04` &nbsp;research

<table>
<tr><td>

### Accent-Invariant Representation Learning for SpeechLLMs
**Samsung PRISM** · *ongoing*

> How do you make a SpeechLLM robust to accented English **without** retraining the whole model?

- **Parameter-efficient adaptation** — LoRA adapters, MoE dynamic adapter routing, accent-aware front-end encoders
- **Benchmarking** SALM, Qwen Audio, SALMONN across ASR/AST tasks
- **Failure analysis** at speaker level *and* accent level, to find which accents are actually worth adapting to
- Targeting a **peer-reviewed publication** as the closure deliverable

<sub>`PyTorch` · `SALM` · `Qwen Audio` · `SALMONN` · `LoRA / PEFT`</sub>

**the goal — make speech models listen to the speaker, not the accent.**

</td></tr>
</table>

<img src="./divider.svg" width="100%" alt=""/>

## `05` &nbsp;trophy shelf

<div align="center">

| | | |
|:--|:--|:--|
| <img src="https://img.shields.io/badge/🥇_1st_Place-FFB84D?style=flat-square&labelColor=04070D"/> | **Economic Times AI Hackathon 2.0** | 60,000+ participants · 10,000+ teams · 28 finalists |
| <img src="https://img.shields.io/badge/🏆_Winner-5EEAD4?style=flat-square&labelColor=04070D"/> | **NioHack 2026** — Niograph Inc., USA | Innovate · Build · Transform |
| <img src="https://img.shields.io/badge/🏆_Winner-5EEAD4?style=flat-square&labelColor=04070D"/> | **Samsung PRISM Web Agent Hackathon** | 450+ participants · 120+ teams |
| <img src="https://img.shields.io/badge/✦_Innovation-38BDF8?style=flat-square&labelColor=04070D"/> | **Agentic AI Hackathon 2025** — Ulster University, UK | 150+ teams |

</div>

<img src="./divider.svg" width="100%" alt=""/>

## `06` &nbsp;outside the terminal

<table>
<tr>
<td width="50%" valign="top">

### Samsung PRISM
`Research Intern` · **Sept 2026 — Present** · Remote

SpeechLLMs, accented speech, and parameter-efficient adaptation. Benchmarking, failure analysis, and adapter routing — aimed at publication.

</td>
<td width="50%" valign="top">

### BharatRohan
`Software Developer Intern` · **Jul — Aug 2026** · Remote

Production geospatial features in React + OpenLayers — vector and raster layers, projections, coordinate reference systems, map interactions, spatial visualization.

</td>
</tr>
</table>

<img src="./divider.svg" width="100%" alt=""/>

## `07` &nbsp;the spellbook

<div align="center">

<br>

**languages**

<img src="https://img.shields.io/badge/Python-071525?style=flat-square&logo=python&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/TypeScript-071525?style=flat-square&logo=typescript&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/JavaScript-071525?style=flat-square&logo=javascript&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/C++-071525?style=flat-square&logo=cplusplus&logoColor=5EEAD4&labelColor=04070D"/>

**build**

<img src="https://img.shields.io/badge/React-071525?style=flat-square&logo=react&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Next.js-071525?style=flat-square&logo=nextdotjs&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Node.js-071525?style=flat-square&logo=nodedotjs&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Express-071525?style=flat-square&logo=express&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/FastAPI-071525?style=flat-square&logo=fastapi&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/PyTorch-071525?style=flat-square&logo=pytorch&logoColor=5EEAD4&labelColor=04070D"/>

**think**

<img src="https://img.shields.io/badge/LangGraph-071525?style=flat-square&logo=langchain&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/MCP-071525?style=flat-square&logo=anthropic&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Transformers.js-071525?style=flat-square&logo=huggingface&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/ONNX-071525?style=flat-square&logo=onnx&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/RAG-071525?style=flat-square&labelColor=04070D&color=071525"/> <img src="https://img.shields.io/badge/Embeddings-071525?style=flat-square&labelColor=04070D"/> <img src="https://img.shields.io/badge/Semantic_Search-071525?style=flat-square&labelColor=04070D"/>

**store**

<img src="https://img.shields.io/badge/PostgreSQL-071525?style=flat-square&logo=postgresql&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/pgvector-071525?style=flat-square&labelColor=04070D"/> <img src="https://img.shields.io/badge/MySQL-071525?style=flat-square&logo=mysql&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Redis-071525?style=flat-square&logo=redis&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/DynamoDB-071525?style=flat-square&logo=amazondynamodb&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Supabase-071525?style=flat-square&logo=supabase&logoColor=5EEAD4&labelColor=04070D"/>

**deploy**

<img src="https://img.shields.io/badge/AWS-071525?style=flat-square&logo=amazonwebservices&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Lambda-071525?style=flat-square&logo=awslambda&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Docker-071525?style=flat-square&logo=docker&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/GitHub_Actions-071525?style=flat-square&logo=githubactions&logoColor=5EEAD4&labelColor=04070D"/> <img src="https://img.shields.io/badge/Git-071525?style=flat-square&logo=git&logoColor=5EEAD4&labelColor=04070D"/>

<br>

</div>

<img src="./divider.svg" width="100%" alt=""/>

## `08` &nbsp;github, but make it statistics

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=anoushkawasthi&show_icons=true&hide_border=true&hide_title=true&include_all_commits=true&bg_color=071525&icon_color=FFB84D&text_color=8CA3B8&ring_color=5EEAD4&title_color=5EEAD4"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anoushkawasthi&layout=compact&hide_border=true&langs_count=8&bg_color=071525&title_color=5EEAD4&text_color=8CA3B8"/>

<br><br>

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=anoushkawasthi&bg_color=071525&color=5EEAD4&line=38BDF8&point=FFB84D&area=true&area_color=0E7490&hide_border=true&custom_title=contribution%20tides"/>

</div>

<br>

<div align="center">

<img src="./footer.svg" width="100%" alt="welcome to the deep end — ikyano.tech"/>

<br>

<a href="https://www.ikyano.tech/"><img src="https://img.shields.io/badge/enter_the_other_side_→-071525?style=for-the-badge&logoColor=5EEAD4&labelColor=04070D"/></a>

<br><br>

<img src="https://komarev.com/ghpvc/?username=anoushkawasthi&style=flat-square&color=5EEAD4&labelColor=04070D&label=surfaced"/>

</div>
