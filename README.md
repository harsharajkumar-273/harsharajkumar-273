# Hi there, I'm Harsha Raj Kumar! 👋

### Software Development Engineer (SDE) | MS CS Student at Vanderbilt University

I'm a Graduate Computer Science student at **Vanderbilt University** specializing in low-level systems programming, high-performance backends, distributed systems, and resilient cloud platform engineering.

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

## 💼 Professional History

*   **VU-BEAM Lab, Vanderbilt University** | *Systems & Software Engineer Research Assistant* (Oct 2025 – Present)
    *   Engineered high-throughput multi-GPU PyTorch data loader pipelines to preprocess, augment, and cache 10,000+ high-resolution ultrasound scan frames, decreasing model training latency by **40%**.
    *   Deployed distributed monitoring with Prometheus to log training metrics across multi-GPU nodes, preventing memory leaks and thermal throttling bottlenecks.
*   **Vanderbilt University Mathematics Department** | *Platform Architect & Software Engineer* (Jan – May 2024)
    *   Engineered **[Proofdesk](https://github.com/harsharajkumar-273/proofdesk)**, a collaborative browser-based LaTeX Web IDE, reducing textbook compilation latency by **72%** (1.1s → 300ms) via client-side WebAssembly. Full technical breakdown below under Flagship Systems.

## 🎓 Academic Credentials

*   🏫 **Vanderbilt University** (Nashville, TN) | Master of Science in Computer Science (*Expected Jun 2027*)
*   🎓 **Vellore Institute of Technology (VIT)** (Chennai, India) | Bachelor of Technology in Computer Science (*Graduated May 2025*)

---

## ⚡ Flagship Systems & Implementations

### 💾 [LSM-Tree Key-Value Engine](https://github.com/harsharajkumar-273/lsm_tree) (C++20, io_uring)
*   Engineered a high-performance LSM-Tree database storage engine in C++20.
*   Implemented asynchronous, non-blocking Write-Ahead Log (WAL) appends utilizing **Linux `io_uring` with `O_DIRECT`**, completely bypassing the kernel page cache.
*   Engineered a concurrent, lock-free SkipList MemTable with atomic CAS pointers and a custom bump-pointer memory Arena.
*   Restricted read lookup penalties to at most one CPU cache line miss using 64-byte cache-aligned vectorized Block Bloom filters.

### 📐 [Proofdesk Collaborative Web IDE](https://github.com/harsharajkumar-273/proofdesk) (React, Node.js, WASM)
*   Architected a browser-based collaborative textbook IDE with a Monaco-editor frontend and sandboxed terminals, deployed to production on AWS EC2 for the Vanderbilt Math Department.
*   Ported the compiler pipeline to the client using **WebAssembly (Pyodide)**, reducing book compilation latency by **72%** (1.1s → 300ms).
*   Engineered isolated, resource-restricted sandbox container runs using WebSocket streams, `node-pty`, and Docker.
*   Implemented a resilient, distributed task queue worker pool using **Redis and BullMQ** with local fallback loops, guaranteeing 100% compiler availability during outages.

### 🔎 [Repost-Radar Content Deduplication Engine](https://github.com/harsharajkumar-273/Repost-Radar) (C++20, AVX2 SIMD, MinHash, LSH)
*   Engineered a high-throughput content-deduplication engine for high-volume Reddit moderation using AVX2 SIMD MinHash across 256-bit YMM registers, achieving a **4.2×** measured speedup over scalar baselines.
*   Optimized memory footprint via zero-copy `std::string_view` shingling, eliminating **65%** of dynamic heap allocations during peak submission stream processing.
*   Designed a concurrent LSH index sharded across 32 `std::shared_mutex` partitions, sustaining **1.45M** read queries/sec for high-volume moderation lookups.

### 📡 [PulseStream Telemetry Pipeline](https://github.com/harsharajkumar-273/PulseStream) (TypeScript, Kafka/Redpanda, Redis, PostgreSQL)
*   Engineered an event-driven telemetry ingestion pipeline sustaining **50,000+ metrics/sec** via a Fastify gateway producing to Redpanda (Kafka-compatible) partitions, acknowledging clients with HTTP 202 in under 8ms.
*   Implemented dual-layer idempotency via atomic Redis SETNX edge locks (0.4ms duplicate rejection) and PostgreSQL `ON CONFLICT` upserts on a composite key, guaranteeing zero duplicate records under peak load.
*   Designed bulk consumer micro-batching, aggregating partition feeds into 1,000-record transactions within 100ms windows — a **27×** throughput gain over per-row inserts.

---

## 🔬 Publications & Systems Recognition

*   **Open Source Contribution — PyTorch (2026)**: Merged a [bug-fix pull request to PyTorch core](https://github.com/pytorch/pytorch/pull/191092) (100k+ stars), resolving an uncaught `ZeroDivisionError` in `torch.unravel_index` for zero-dimension tensor shapes. Reviewed and approved by a PyTorch core maintainer.
*   **IEEE Published (2025)**: *An Integrated GCN–GAT–AE Framework for Robust Anomaly Detection in Industrial IoT Environments* — Developed an integrated deep learning framework combining Graph Convolutional Networks (GCN), Graph Attention Networks (GAT), and Autoencoders (AE) for robust and noise-resilient anomaly detection in Industrial IoT sensor networks.
*   **Vanderbilt Global Good Hackathon Finalist (2025)**: Co-developed **[ARIA Pathfinder](https://github.com/harsharajkumar-273/ARIA)**, a PostGIS-backed disaster response routing system utilizing Dijkstra with time-decaying edge weight equations.
*   **GDSC Technical Lead (2024–2025)**: Co-lead of the Technical Division for the Google Developer Student Club (GDSC) at VIT, conducting technical workshops for 200+ student members.

---

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
*   **SDE Portfolio**: [harsharajkumar-273.github.io/SDE-Portfolio/](https://harsharajkumar-273.github.io/SDE-Portfolio/)
*   **Email**: [harsharajkumar273@gmail.com](mailto:harsharajkumar273@gmail.com)
