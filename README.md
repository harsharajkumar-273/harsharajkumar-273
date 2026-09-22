<h1 align="center">Harsha Raj Kumar</h1>

<p align="center">
  <b>Software Engineer · Backend &amp; Distributed Systems</b><br/>
  M.S. Computer Science @ Vanderbilt University · graduating April 2027 · open to 2027 new-grad roles
</p>

<p align="center">
  <a href="https://hashadev.duckdns.org"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-hashadev-1B3A6B?style=flat-square"/></a>
  <a href="https://linkedin.com/in/harsharajkumar273"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-harsharajkumar273-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:harsha.raj.kumar@vanderbilt.edu"><img alt="Email" src="https://img.shields.io/badge/Email-harsha.raj.kumar%40vanderbilt.edu-555?style=flat-square&logo=maildotru&logoColor=white"/></a>
  <a href="https://huggingface.co/harsharajkumar273"><img alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-harsharajkumar273-FFD21E?style=flat-square&logo=huggingface&logoColor=black"/></a>
</p>

I build backend services, storage systems, and developer tools. I like work where the numbers can be checked: every benchmark below links to the script that produced it.

---

### Highlights

| | |
|---|---|
| **PyTorch contributor** | Fix merged into core ([#191092](https://github.com/pytorch/pytorch/pull/191092)); `all_reduce` avg-reduction backward approved by a distributed maintainer ([#190630](https://github.com/pytorch/pytorch/pull/190630)). |
| **Open-source maintainer** | Reviewed and merged **112 pull requests** from 4 contributors to [lsm_tree](https://github.com/harsharajkumar-273/lsm_tree/pulls?q=is%3Apr+is%3Amerged) and [Proofdesk](https://github.com/harsharajkumar-273/Proofdesk/pulls?q=is%3Apr+is%3Amerged) during ELUSOC 2026. |
| **Publication** | Co-author, [*An Integrated GCN–GAT–AE Framework for Robust Anomaly Detection in Industrial IoT Environments*](https://doi.org/10.1109/CICT67193.2025.11399172), IEEE CICT 2025. |

---

### Selected work

| Project | What it is | Evidence |
|---|---|---|
| [**LSM-Tree Storage Engine**](https://github.com/harsharajkumar-273/lsm_tree) · C++17 | Collaborative key-value storage engine: lock-free SkipList MemTable, io_uring + O_DIRECT write-ahead log, blocked Bloom filters, leveled compaction. I lead and maintain it: architecture, design reviews, and integrating contributors' work. | **254K writes/sec**, 32 µs P99 · [benchmarks](https://github.com/harsharajkumar-273/lsm_tree/tree/main/benchmarks) |
| [**Proofdesk**](https://github.com/harsharajkumar-273/Proofdesk) · TypeScript, React | Collaborative textbook IDE: Y.js CRDT editing over authenticated WebSockets, BullMQ/Redis build queue, resource-capped Docker workers, in-browser Pyodide preview. | **358 ms** median in-browser preview (local, 5 runs) · [benchmarks](https://github.com/harsharajkumar-273/Proofdesk/tree/main/benchmarks) |
| [**PulseStream**](https://github.com/harsharajkumar-273/PulseStream) · TypeScript, Kafka | Telemetry ingestion: Express → Kafka → PostgreSQL with device-keyed partitions, Redis idempotency keys, retries, and a dead-letter queue. | **3,991 req/s**, 11 ms p50 / 34 ms p99 (local Docker) · [load test](https://github.com/harsharajkumar-273/PulseStream/tree/main/benchmarks) |
| [**Satya**](https://github.com/harsharajkumar-273/Satya-) · Python, Playwright | Agent that runs UI flows and flags success messages the backend contradicts (a "Deleted!" toast with no DELETE call). FastAPI service, SQLite run history, JUnit reports. | 77 tests in CI |
| [**ENGRAM**](https://github.com/harsharajkumar-273/ENGRAM) · TypeScript | Memory engine for LLM agents: decay, reinforcement, contradiction detection, and hot/warm/cold tiered vector retrieval with int8 cold storage. | 73% fewer vector comparisons at equal Recall@5 (synthetic) · [results](https://github.com/harsharajkumar-273/ENGRAM/blob/main/BENCHMARK_RESULTS.md) |
| [**ReCL**](https://github.com/harsharajkumar-273/ReCL) · PyTorch | Self-supervised learning for ultrasound/EEG sim-to-real transfer (InfoNCE + NCC reconstruction loss), with 3-seed baselines and ablations. | [checkpoints](https://huggingface.co/harsharajkumar273/ReCL-Ultrasound-Checkpoints) · [dataset](https://huggingface.co/datasets/harsharajkumar273/ReCL-Ultrasound-Dataset) |

---

### Experience

- **Amplify GenAI Innovation Center, Vanderbilt** — Software Engineer, Backend & Platform Systems · *Aug 2026 – present*<br/>
  FastAPI/Redis APIs for LLM tool calls and session state; pgvector hybrid retrieval that cut retrieval latency by 38%; QA that fixed 20+ defects.
- **VU-BEAM Lab, Vanderbilt** — Research Assistant · *Oct 2025 – Aug 2026*<br/>
  Built ReCL; async multi-GPU data loading that cut training time by 40%; Slurm sweeps on the ACCRE GPU cluster.
- **Mathematics Department, Vanderbilt** — Software Engineer · *Sep 2025 – May 2026*<br/>
  Built Proofdesk, a collaborative editor and sandboxed build system for PreTeXt textbooks.

### Toolkit

**Languages** C++17 · Python · TypeScript/JavaScript · Java · Go · SQL<br/>
**Backend & data** Node.js/Express · FastAPI · PostgreSQL/pgvector · Redis · Kafka/Redpanda · BullMQ · SQLite<br/>
**Systems & ML** Linux (io_uring) · Docker · AWS · GitHub Actions · Prometheus · Playwright · React · PyTorch

<sub>Also: AWS Certified AI Practitioner · Microsoft Azure AI Fundamentals · Vanderbilt Global Good Hackathon finalist (2025, <a href="https://github.com/harsharajkumar-273/ARIA">ARIA</a>) · GDSC Technical Lead (2024–25)</sub>
