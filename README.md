# Harsha Raj Kumar

**Software Engineering · M.S. Computer Science, Vanderbilt University · Expected April 2027**

I build collaborative applications, APIs, storage systems, and developer tools with Python, TypeScript, and C++.
Seeking **2027 new-graduate software engineering roles**. Based in Nashville and open to relocation.

[Portfolio](https://hashadev.duckdns.org/) · [LinkedIn](https://linkedin.com/in/harsharajkumar273) · [Email](mailto:harsha.raj.kumar@vanderbilt.edu)

## Highlights

- **PyTorch contributor:** two merged fixes in [C++ NCCL2 `all_gather`](https://github.com/pytorch/pytorch/pull/200585) and [`torch.unravel_index`](https://github.com/pytorch/pytorch/pull/191092), with regression tests.
- **Shipped software:** built Amplify's Projects workspace, now available to users; co-developed Proofdesk, used by a professor to publish and update *Interactive Linear Algebra*.
- **Published developer tool:** [codegraph-engine on npm](https://www.npmjs.com/package/codegraph-engine), with a [browser-based repository explorer](https://codegraph-eta.vercel.app/).

## Selected projects

### [Proofdesk](https://github.com/harsharajkumar-273/Proofdesk) — collaborative textbook authoring

Co-developed a PreTeXt editor with React/Monaco, Y.js/WebSockets, Express APIs, and queued Docker builds. Continued the project after the university appointment, adding a Pyodide browser preview, Terraform configuration, and CI/CD improvements, and opening it to contributors.

[Architecture](https://github.com/harsharajkumar-273/Proofdesk/blob/main/ARCHITECTURE.md) · [Build and preview measurements](https://github.com/harsharajkumar-273/Proofdesk/blob/main/benchmarks/docker_pipeline/README.md)

### [PulseStream](https://github.com/harsharajkumar-273/PulseStream) — event ingestion and recovery

Built an Express/Kafka/PostgreSQL pipeline with idempotent ingestion, per-message transaction isolation, and offset advancement after database commit. CI covers **11 API failure scenarios**. In a **30-second, 50-connection MacBook Air/Docker Desktop run**, measured **430 persisted events/s** and **854 ms p99 send-to-row latency**. A separate **3,000-event run** stored every broker-acknowledged event after three consumer/database kills.

These are scoped local measurements, not production capacity or exactly-once guarantees. [Method and limitations](https://github.com/harsharajkumar-273/PulseStream#benchmark)

### [CodeGraph](https://github.com/harsharajkumar-273/CodeGraph) — inspect the impact of code changes

Built dependency and call graphs, confidence labels, and reverse-edge traversal for affected code and tests. Supports TypeScript, JavaScript, Python, and Go. Maintainer-run evaluation uses compiler/type-checker and Jedi reference results across **10 repositories**; it reports confidence tiers and limitations separately, rather than one broad accuracy claim.

[npm package](https://www.npmjs.com/package/codegraph-engine) · [Evaluation methodology](https://github.com/harsharajkumar-273/CodeGraph/blob/main/docs/ORACLE-EVAL.md)

### [LSM-Tree](https://github.com/harsharajkumar-273/lsm_tree) — C++17 storage engine

Started and maintain the engine with contributors. Added range scans that merge MemTable and SSTable cursors, resolve versions and tombstones, and are checked against `std::map`. The project distinguishes asynchronous acknowledgments from durable writes and tests recovery, cancellation, and injected failures. Contributor implementation credits are documented in the repository.

[Range-scan implementation](https://github.com/harsharajkumar-273/lsm_tree/pull/137) · [Durability contract](https://github.com/harsharajkumar-273/lsm_tree/blob/main/DURABILITY.md) · [Benchmarks](https://github.com/harsharajkumar-273/lsm_tree/blob/main/benchmarks/results.md)

### [Satya](https://github.com/harsharajkumar-273/Satya-) — check UI claims against persisted state

Built a Playwright tool that compares visible success claims with API state or state after reload. Includes CLI/CI reports and a FastAPI service. Validation covers seeded bugs and third-party TodoMVC apps; large production-app validation remains future work.

[Demonstrations and validation](https://github.com/harsharajkumar-273/Satya-/blob/main/docs/VALIDATION.md)

## Experience

- **Amplify GenAI Innovation Center, Vanderbilt — Research Assistant, Software Engineering** · Aug 2026–present  
  Built and shipped Projects across React/TypeScript and Python/AWS Lambda, with DynamoDB-backed APIs, ownership checks, and project context in conversations. Fixed generated artifacts displaying as raw code instead of sandboxed previews. [Backend implementation PR](https://github.com/gaiin-platform/amplify-genai-backend/pull/393) · [Frontend implementation PR](https://github.com/gaiin-platform/amplify-genai-frontend/pull/335).
- **VU-BEAM Lab, Vanderbilt — Research Assistant** · Oct 2025–Aug 2026  
  Implemented contrastive pretraining, supervised fine-tuning, and PyTorch data loading and augmentation for ultrasound research.
- **Vanderbilt Mathematics Department — Research Assistant, Software Engineering**  
  Developed Proofdesk for collaborative textbook authoring; continued developing it as an open project after the appointment.

## Open source and research

- **PyTorch distributed C++:** fixed NCCL2 treating distinct empty tensors as aliased buffers during uneven gathers. [Landed commit](https://github.com/pytorch/pytorch/commit/e96d01e48edf389ee8e7e6e9bacfef1888dce711).
- **PyTorch core:** fixed zero-dimension validation while preserving empty-input behavior. [Landed commit](https://github.com/pytorch/pytorch/commit/f594cadbd10e281c04c0e471b40c3b0569e47c43).
- **Research publication:** co-author, [An Integrated GCN–GAT–AE Framework for Robust Anomaly Detection in Industrial IoT Environments](https://doi.org/10.1109/CICT67193.2025.11399172), IEEE CICT 2025.

## Tools I use

**Languages:** C++, Python, TypeScript/JavaScript, Java, SQL  
**Applications and data:** React, Node.js/Express, FastAPI, PostgreSQL/pgvector, DynamoDB, Redis, Kafka/Redpanda, Y.js  
**Engineering:** Linux, Docker, AWS Lambda, Terraform, GitHub Actions CI/CD, Playwright, PyTorch, Claude Code
