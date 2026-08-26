# Hi there, I'm Harsha Raj Kumar! 👋

### Software Development Engineer (SDE) | MS CS Student at Vanderbilt University

I'm a Graduate Computer Science student at **Vanderbilt University** specializing in low-level systems programming, high-performance backends, and distributed systems.

---

## 🛠️ Technical Arsenal

<div align="center">
  
  <!-- Languages -->
  <img src="https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python" />
  <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white" alt="Go" />
  
  <br/>
  
  <!-- Frameworks & Backends -->
  <img src="https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB" alt="Express.js" />
  <img src="https://img.shields.io/badge/fastapi-109989?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB" alt="React" />
  
  <br/>
  
  <!-- Database & Infra -->
  <img src="https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS" />
  
</div>

---

## 🏆 Featured: Merged Core Contribution to PyTorch

**[pytorch/pytorch#191092](https://github.com/pytorch/pytorch/pull/191092)** — fixed an uncaught `ZeroDivisionError` in `torch.unravel_index`, reviewed and merged by PyTorch core maintainers. Six additional PRs across `distributed`, `linalg`, and BLAS code are currently in review.

---

## 💼 Professional Experience

*   **Amplify GenAI Innovation (AGI) Center, Vanderbilt University** | *Software Engineer — GenAI Platform & Systems* <!-- TODO: confirm exact start date, currently reads as a future date — fix before publishing -->
    *   Engineering scalable GenAI platform tooling, API integrations, and multi-agent workflows across Vanderbilt's College of Connected Computing.
    *   Building high-throughput LLM middleware services and vector indexing pipelines to accelerate AI application deployment.
*   **VU-BEAM Lab, Vanderbilt University** | *Research Assistant* (Oct 2025 – Aug 2026)
    *   Designed **ReCL (Reconstructive Contrastive Learning)**, a self-supervised ultrasound model evaluated against baselines on the PICMUS benchmark. Submitted to NeurIPS 2026 (not accepted).
    *   Optimized offline batch-processing data pipelines across **10,000+** ultrasound scan frames, reducing multi-GPU training execution time by **40%**.
*   **Vanderbilt University Mathematics Department** | *Platform Architect & Software Engineer* (Jan – May 2026)
    *   Engineered **Proofdesk**, a collaborative Web IDE sandbox, reducing compilation feedback latency by **72%** (from 1.1s to **300ms**) via client-side WebAssembly (Pyodide).
    *   Deployed WebSocket sandboxed terminal runtimes (`node-pty`) inside resource-restricted Docker containers (512MB RAM limit).
    *   Architected a distributed background worker task queue using **Redis and BullMQ** with local fallback loops.

## 🎓 Academic Credentials

*   🏫 **Vanderbilt University** (Nashville, TN) | Master of Science in Computer Science (*Expected Jun 2027*)
*   🎓 **Vellore Institute of Technology (VIT)** (Chennai, India) | Bachelor of Technology in Computer Science (*Graduated May 2025*)

---

## ⚡ Flagship Systems & Implementations

### 📈 [PulseStream Telemetry Pipeline](https://github.com/harsharajkumar-273/PulseStream) (TypeScript, Redpanda/Kafka, KEDA)
*   Designed a horizontally scalable telemetry ingestion gateway targeting **50,000+ metrics/sec** across distributed Redpanda (Kafka-compatible) event streams (see repo for benchmark-reproduction script).
*   Decoupled write paths from persistence using device ID hash partition keys for fast HTTP 202 ingestion ACKs.
*   Implemented double-layer idempotency utilizing **Redis `SETNX` edge locks** and atomic PostgreSQL batch upserts.

### 🔁 [revert-ai](https://github.com/harsharajkumar-273/revert-ai) (TypeScript, Node.js, AST Parsers, Git API, NPM)
*   Built and published `revert-ai` on npm — a dependency-aware undo/redo CLI for AI coding assistants (Claude Code, Aider), reading session logs and git history to track file operations.
*   Engineered AST-based dependency analysis for JS/TS and Python import graphs to safely cascade file reversions while preserving unrelated edits.
*   Implemented side-by-side terminal diff previews and Git stashing safety guards, validated by a Jest test suite.

### 💾 [LSM-Tree Key-Value Engine](https://github.com/harsharajkumar-273/lsm_tree) (C++20, io_uring)
*   Engineered a high-performance LSM-Tree database storage engine in C++20 with a small team, via a structured open-source-club build (issue-driven PRs, CI, dependabot).
*   Implemented asynchronous, non-blocking Write-Ahead Log (WAL) appends utilizing **Linux `io_uring` with `O_DIRECT`**, bypassing the kernel page cache.
*   Engineered a concurrent, lock-free SkipList MemTable with atomic CAS pointers and a custom bump-pointer memory Arena.
*   Restricted read lookup penalties to at most one CPU cache line miss using 64-byte cache-aligned vectorized Block Bloom filters.

---

<!--
  TODO before publishing — confirm each of these with sources, or remove:
  - "IEEE Published Paper (2025)" — could not be located on IEEE Xplore by title or author search; verify or remove.
  - "Vanderbilt Global Good Hackathon Finalist (2025)" — confirm.
  - "GDSC Technical Lead (2024–2025)" — confirm.
  See Career Intelligence Report for details.
-->

## 📊 GitHub Contribution Stats

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=harsharajkumar-273&theme=nord" alt="Harsha's GitHub Streak" />
</div>

<br/>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=harsharajkumar-273&theme=nord&column=7" alt="Harsha's Trophies" />
</div>

---

## 🔗 Connect with Me
*   **LinkedIn**: [linkedin.com/in/harsharajkumar273](https://linkedin.com/in/harsharajkumar273)
*   **Website Portfolio**: [hashadev.duckdns.org](https://hashadev.duckdns.org/)
*   **Email**: [harsharajkumar273@gmail.com](mailto:harsharajkumar273@gmail.com)
