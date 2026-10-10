<div align="center">

<img src="./hero.svg" width="100%" alt="Anoushka Awasthi — a little bit of code, a little bit of chaos, mostly curiosity"/>

<br><br>

<a href="https://www.ikyano.tech/"><img src="https://img.shields.io/badge/ikyano.tech-FFD45C?style=for-the-badge&logo=googlechrome&logoColor=241E4E"/></a>
<a href="https://www.linkedin.com/in/anoushka-awasthi-a87754247/"><img src="https://img.shields.io/badge/linkedin-5B7CFA?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/github-241E4E?style=for-the-badge&logo=github&logoColor=FFF6EC"/></a>
<a href="mailto:awasthinush2580@gmail.com"><img src="https://img.shields.io/badge/say_hi-FF6FB5?style=for-the-badge&logo=gmail&logoColor=241E4E"/></a>

<br><br>

<img src="https://readme-typing-svg.demolab.com?font=Space+Mono&weight=700&size=16&duration=2800&pause=1000&color=FF6FB5&center=true&vCenter=true&width=640&lines=building+agents+that+think+%26+tools+that+remember;currently%3A+teaching+speech+models+about+accents;4+hackathon+wins%2C+1+jellyfish%2C+0+regrets;I+learn+by+building%2C+breaking%2C+rebuilding" alt="rotating notes"/>

<img src="./divider.svg" width="100%" alt=""/>

</div>

## ✿ hello, hello

<table>
<tr>
<td width="60%" valign="top">

I build things I find interesting — and I find a *lot* of things interesting.

Sometimes that's an **AI agent making safety calls** on a factory floor. Sometimes it's a **coding agent that remembers why**. Sometimes it's a **browser that quietly takes notes**, a **map with far too many layers**, or a SpeechLLM that absolutely refuses to understand an accent (we're working on it).

I like living underneath the interface: agents, retrieval, event-driven backends, local inference, and the plumbing that keeps it all from falling over.

I learn best by building, breaking, and rebuilding.

</td>
<td width="40%" valign="top">

**field notes**

| | |
|:--:|:--|
| 🔬 | researching at **Samsung PRISM** |
| 🏆 | **4×** hackathon winner |
| 🎓 | Comp. Eng. @ Thapar · **8.78** |
| 📍 | Patiala, India |
| ☕ | runs on curiosity & caffeine |
| 🐛 | debugging ratio: *questionable* |

</td>
</tr>
</table>

<div align="center"><img src="./divider.svg" width="100%" alt=""/></div>

## ✦ the specimen cabinet

<sub>things i've built, pinned and labelled for your viewing pleasure.</sub>

<table>
<tr>
<td width="240" valign="top" align="center"><img src="./sop-opera.svg" width="220" alt="Specimen no.01 — a hard hat singing opera"/></td>
<td valign="top">

### SOP Opera
*agentic industrial safety intelligence*

<img src="https://img.shields.io/badge/🥇_1st_place-ET_AI_Hackathon_2.0-FF6FB5?style=flat-square&labelColor=241E4E"/> <img src="https://img.shields.io/badge/out_of-10,000%2B_teams-FFD45C?style=flat-square&labelColor=241E4E"/>

A multi-agent system that catches **compound** risk before high-risk work gets approved. A gas reading, a work permit, an isolation state, a worker's location — each looks fine alone. The danger lives in the combination, so the system reasons over all of it at once.

- false negatives **44.5% → 0%** across 593 labelled cases; hazards caught **28 min** earlier
- LangGraph pipeline with conditional agent fan-out
- hybrid pgvector + SQL retrieval over clause-level regulations, so every call cites its rule
- durable Postgres job queue, WebSockets with per-client backpressure, hash-chained audit trail

<sub>`Python` `TypeScript` `FastAPI` `LangGraph` `PostgreSQL` `pgvector` `Next.js` `Docker`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/peek_inside_→-FFD45C?style=flat-square&logo=github&logoColor=241E4E"/></a>

</td>
</tr>
</table>

<table>
<tr>
<td width="240" valign="top" align="center"><img src="./flowsync.svg" width="220" alt="Specimen no.02 — a jar of whys"/></td>
<td valign="top">

### FlowSync
*persistent memory for coding agents*

Coding agents can write code. They're terrible at remembering *why* it exists. FlowSync collects the whys — decisions, risks, and tasks pulled straight out of git diffs — and keeps them in a jar your agent can reach into.

- event-driven extraction from git diffs via Bedrock
- VS Code extension + MCP server for logging, project search, and retrieval
- branch-aware RAG with DynamoDB caching — **1.26s** median push → search (p95 1.60s)

<sub>`TypeScript` `Python` `AWS Bedrock` `Lambda` `DynamoDB` `S3` `MCP` `Next.js`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/peek_inside_→-FFD45C?style=flat-square&logo=github&logoColor=241E4E"/></a>

</td>
</tr>
</table>

<table>
<tr>
<td width="240" valign="top" align="center"><img src="./konta.svg" width="220" alt="Specimen no.03 — a browser that remembers"/></td>
<td valign="top">

### Konta
*your browser remembers — locally*

<img src="https://img.shields.io/badge/🏆_winner-Samsung_PRISM_Web_Agent_Hackathon-7EE0B5?style=flat-square&labelColor=241E4E"/>

A local-first Chrome extension that turns browsing into a private little constellation of everything you've read. The embeddings never leave home — no giant cloud brain required.

- on-device semantic embeddings with Transformers.js + ONNX
- knowledge graph linking pages by meaning, time, and context
- session boundary detection, so unrelated rabbit holes stay separate

<sub>`TypeScript` `React` `IndexedDB` `Transformers.js` `ONNX`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/peek_inside_→-FFD45C?style=flat-square&logo=github&logoColor=241E4E"/></a>

</td>
</tr>
</table>

<table>
<tr>
<td width="240" valign="top" align="center"><img src="./gina.svg" width="220" alt="Specimen no.04 — data, but chatty"/></td>
<td valign="top">

### GINA
*ask questions, get grounded data*

Ask *"why did revenue drop?"* in plain words and get back validated SQL, real numbers, and an answer streamed as it's found.

- multi-model NL → SQL pipeline with structured, grounded query generation
- SSE streaming with fast-path routing over snapshots and cache restoration
- multi-turn memory and schema self-correction loops

<sub>`Next.js` `TypeScript` `Fastify` `PostgreSQL` `Supabase` `SSE`</sub>

<a href="https://github.com/anoushkawasthi"><img src="https://img.shields.io/badge/peek_inside_→-FFD45C?style=flat-square&logo=github&logoColor=241E4E"/></a>

</td>
</tr>
</table>

<div align="center"><img src="./divider.svg" width="100%" alt=""/></div>

## ☾ research corner

<table>
<tr>
<td width="240" valign="top" align="center"><img src="./research.svg" width="220" alt="Specimen no.05 — listening, properly"/></td>
<td valign="top">

### Accent-Invariant Representation Learning for SpeechLLMs
*Samsung PRISM · ongoing*

How do you teach a speech model to understand accented English **without** retraining the whole thing?

- parameter-efficient adaptation: LoRA adapters, MoE dynamic adapter routing, accent-aware encoders
- benchmarking SALM, Qwen Audio, and SALMONN
- speaker- and accent-level failure analysis to find where models stumble
- headed for a peer-reviewed publication

<sub>`PyTorch` `SALM` `Qwen Audio` `SALMONN` `LoRA / PEFT`</sub>

> *make speech models listen to the speaker, not the accent.*

</td>
</tr>
</table>

<div align="center"><img src="./divider.svg" width="100%" alt=""/></div>

## ★ trophy shelf

<div align="center">

| | | |
|:--:|:--|:--|
| <img src="https://img.shields.io/badge/🥇_1st-FF6FB5?style=for-the-badge"/> | **Economic Times AI Hackathon 2.0** | 60,000+ participants · 10,000+ teams · 28 finalists |
| <img src="https://img.shields.io/badge/🏆_winner-5B7CFA?style=for-the-badge"/> | **NioHack 2026** · Niograph Inc., USA | innovate · build · transform |
| <img src="https://img.shields.io/badge/🏆_winner-7EE0B5?style=for-the-badge"/> | **Samsung PRISM Web Agent Hackathon** | 450+ participants · 120+ teams |
| <img src="https://img.shields.io/badge/✨_innovation-FFD45C?style=for-the-badge"/> | **Agentic AI Hackathon 2025** · Ulster University, UK | 150+ teams |

</div>

<div align="center"><img src="./divider.svg" width="100%" alt=""/></div>

## ✎ where i've been

<table>
<tr>
<td width="50%" valign="top">

### Samsung PRISM
`research intern` · **Sept 2026 — now** · remote

SpeechLLMs, accented speech, and parameter-efficient adaptation. Benchmarks, failure analysis, adapter routing — aimed at publication.

</td>
<td width="50%" valign="top">

### BharatRohan
`software developer intern` · **Jul — Aug 2026** · remote

Production geospatial features in React + OpenLayers: vector and raster layers, projections, coordinate systems, and maps with far too many layers.

</td>
</tr>
</table>

<div align="center"><img src="./divider.svg" width="100%" alt=""/></div>

## ⚗ the spellbook

<div align="center">

<sub>**languages**</sub><br>
<img src="https://img.shields.io/badge/Python-FF6FB5?style=flat-square&logo=python&logoColor=241E4E"/> <img src="https://img.shields.io/badge/TypeScript-FF6FB5?style=flat-square&logo=typescript&logoColor=241E4E"/> <img src="https://img.shields.io/badge/JavaScript-FF6FB5?style=flat-square&logo=javascript&logoColor=241E4E"/> <img src="https://img.shields.io/badge/C++-FF6FB5?style=flat-square&logo=cplusplus&logoColor=241E4E"/>

<sub>**build**</sub><br>
<img src="https://img.shields.io/badge/React-5B7CFA?style=flat-square&logo=react&logoColor=white"/> <img src="https://img.shields.io/badge/Next.js-5B7CFA?style=flat-square&logo=nextdotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Node.js-5B7CFA?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Express-5B7CFA?style=flat-square&logo=express&logoColor=white"/> <img src="https://img.shields.io/badge/FastAPI-5B7CFA?style=flat-square&logo=fastapi&logoColor=white"/> <img src="https://img.shields.io/badge/Fastify-5B7CFA?style=flat-square&logo=fastify&logoColor=white"/>

<sub>**think**</sub><br>
<img src="https://img.shields.io/badge/LangGraph-B9A6FF?style=flat-square&logo=langchain&logoColor=241E4E"/> <img src="https://img.shields.io/badge/PyTorch-B9A6FF?style=flat-square&logo=pytorch&logoColor=241E4E"/> <img src="https://img.shields.io/badge/Transformers.js-B9A6FF?style=flat-square&logo=huggingface&logoColor=241E4E"/> <img src="https://img.shields.io/badge/ONNX-B9A6FF?style=flat-square&logo=onnx&logoColor=241E4E"/> <img src="https://img.shields.io/badge/MCP-B9A6FF?style=flat-square&logo=anthropic&logoColor=241E4E"/> <img src="https://img.shields.io/badge/RAG-B9A6FF?style=flat-square"/> <img src="https://img.shields.io/badge/embeddings-B9A6FF?style=flat-square"/>

<sub>**store**</sub><br>
<img src="https://img.shields.io/badge/PostgreSQL-7EE0B5?style=flat-square&logo=postgresql&logoColor=241E4E"/> <img src="https://img.shields.io/badge/pgvector-7EE0B5?style=flat-square"/> <img src="https://img.shields.io/badge/MySQL-7EE0B5?style=flat-square&logo=mysql&logoColor=241E4E"/> <img src="https://img.shields.io/badge/Redis-7EE0B5?style=flat-square&logo=redis&logoColor=241E4E"/> <img src="https://img.shields.io/badge/DynamoDB-7EE0B5?style=flat-square&logo=amazondynamodb&logoColor=241E4E"/> <img src="https://img.shields.io/badge/Supabase-7EE0B5?style=flat-square&logo=supabase&logoColor=241E4E"/>

<sub>**ship**</sub><br>
<img src="https://img.shields.io/badge/AWS-FFD45C?style=flat-square&logo=amazonwebservices&logoColor=241E4E"/> <img src="https://img.shields.io/badge/Lambda-FFD45C?style=flat-square&logo=awslambda&logoColor=241E4E"/> <img src="https://img.shields.io/badge/Docker-FFD45C?style=flat-square&logo=docker&logoColor=241E4E"/> <img src="https://img.shields.io/badge/GitHub_Actions-FFD45C?style=flat-square&logo=githubactions&logoColor=241E4E"/> <img src="https://img.shields.io/badge/Git-FFD45C?style=flat-square&logo=git&logoColor=241E4E"/>

</div>

<div align="center"><img src="./divider.svg" width="100%" alt=""/></div>

## ◔ github, but make it statistics

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=anoushkawasthi&show_icons=true&hide_title=true&include_all_commits=true&border_radius=16&bg_color=FFF6EC&border_color=241E4E&icon_color=5B7CFA&text_color=241E4E&ring_color=FF6FB5"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anoushkawasthi&layout=compact&langs_count=8&border_radius=16&bg_color=FFF6EC&border_color=241E4E&title_color=FF6FB5&text_color=241E4E"/>

<br><br>

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=anoushkawasthi&bg_color=FFF6EC&color=241E4E&line=FF6FB5&point=5B7CFA&area=true&area_color=FFD45C&radius=16&custom_title=contribution%20tides"/>

</div>

<br>

<div align="center">

<img src="./footer.svg" width="100%" alt="A postcard from the deep end — thanks for swimming all the way down here"/>

<sub>made with curiosity, caffeine, and questionable amounts of debugging.</sub>

</div>
