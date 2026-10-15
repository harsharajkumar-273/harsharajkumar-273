# Harsha Raj Kumar

**Software Engineering · M.S. Computer Science at Vanderbilt · Expected April 2027**

I build APIs, collaborative applications, storage systems, and developer tools. My work spans Python, TypeScript, and C++, with an interest in reliable systems and machine learning infrastructure.

Seeking **2027 new-graduate software engineering roles**. Based in Nashville and open to relocation.

[Portfolio](https://hashadev.duckdns.org/) · [LinkedIn](https://linkedin.com/in/harsharajkumar273) · [Email](mailto:harsha.raj.kumar@vanderbilt.edu)

## Highlights

- **Two merged PyTorch contributions:** [C++ NCCL2 all_gather fix #200585](https://github.com/pytorch/pytorch/pull/200585) and [core validation fix #191092](https://github.com/pytorch/pytorch/pull/191092), both with regression tests.
- **Deployed software:** [Proofdesk](https://proofdesk.duckdns.org/), used by a professor to publish and update an online textbook.
- **Published developer tool:** [codegraph-engine on npm](https://www.npmjs.com/package/codegraph-engine).

## Selected work

| Project | What I contributed | Evidence |
| --- | --- | --- |
| [Proofdesk](https://github.com/harsharajkumar-273/Proofdesk) | Co-developed and maintain a collaborative PreTeXt textbook editor: React/Monaco, Y.js/WebSockets, Node/Express, queued Docker builds, GitHub Actions CI/CD, and a later Pyodide browser preview. | [Deployed application](https://proofdesk.duckdns.org/) · [Architecture](https://github.com/harsharajkumar-273/Proofdesk/blob/main/ARCHITECTURE.md) |
| [PulseStream](https://github.com/harsharajkumar-273/PulseStream) | Built telemetry ingestion and persistence, then addressed batch isolation, offset ordering, and conflicting replays. | **11 API-level failure scenarios**; documented local benchmark: **2,933 events/sec persisted** during a 30-second send window. [Method and limitations](https://github.com/harsharajkumar-273/PulseStream#benchmark) |
| [CodeGraph](https://github.com/harsharajkumar-273/CodeGraph) | Built a TypeScript/Tree-sitter CLI for dependency graphs, call graphs, and change-impact traversal, with confidence labels for inferred edges. | [npm package](https://www.npmjs.com/package/codegraph-engine) · [Resolution methodology](https://github.com/harsharajkumar-273/CodeGraph/blob/main/docs/PRECISION.md) |
| [LSM-Tree](https://github.com/harsharajkumar-273/lsm_tree) | Started and maintain a collaborative C++17 storage engine; contribute architecture, design review, and integration, with implementation credit documented for contributors. | **14 CTest programs** documented on main; explicit asynchronous vs durable acknowledgment contracts. [Durability](https://github.com/harsharajkumar-273/lsm_tree/blob/main/DURABILITY.md) · [Benchmarks](https://github.com/harsharajkumar-273/lsm_tree/blob/main/benchmarks/results.md) |
| [Satya](https://github.com/harsharajkumar-273/Satya-) | Built a Playwright-based tool that compares UI success claims with API or reload-persisted state; includes a CLI, reports, and FastAPI service. | [Seeded-bug demonstrations and validation](https://github.com/harsharajkumar-273/Satya-/blob/main/docs/VALIDATION.md); production-scale validation remains future work. |

Benchmarks above are local development measurements, not production capacity claims. See each repository for inputs, environment, limitations, and contributor credit.

## Experience

- **Amplify GenAI Innovation Center, Vanderbilt — Research Assistant, Software Engineering** · Aug 2026–present<br>
  Implemented Projects across React/TypeScript and Python/AWS Lambda: project, file-manifest, and memory APIs backed by three DynamoDB tables, ownership checks, and server-side chat context. [Backend PR](https://github.com/gaiin-platform/amplify-genai-backend/pull/393) · [Frontend PR](https://github.com/gaiin-platform/amplify-genai-frontend/pull/335). Implementation was tested; release was pending at last confirmation.
- **VU-BEAM Lab, Vanderbilt — Research Assistant** · Oct 2025–Aug 2026<br>
  Implemented contrastive pretraining, supervised fine-tuning, and PyTorch data loading and augmentation for ultrasound research.
- **Vanderbilt Mathematics Department — Research Assistant, Software Engineering** · Sep 2025–May 2026<br>
  Developed Proofdesk for collaborative textbook authoring. Continued maintaining the project after the appointment, including the browser preview added in June 2026.

## Open source and research

- **PyTorch distributed C++:** fixed NCCL2 `all_gather` treating distinct empty tensors as aliased buffers, preventing shape errors during uneven gathers; added distributed regression tests. [PR #200585](https://github.com/pytorch/pytorch/pull/200585) · [Landed commit](https://github.com/pytorch/pytorch/commit/e96d01e48edf389ee8e7e6e9bacfef1888dce711).
- **PyTorch core:** fixed zero-dimension validation in `torch.unravel_index`, preserving empty-input behavior and adding regression tests. [PR #191092](https://github.com/pytorch/pytorch/pull/191092) · [Landed commit](https://github.com/pytorch/pytorch/commit/f594cadbd10e281c04c0e471b40c3b0569e47c43).
- **Research publication:** co-author, [An Integrated GCN–GAT–AE Framework for Robust Anomaly Detection in Industrial IoT Environments](https://doi.org/10.1109/CICT67193.2025.11399172), IEEE CICT 2025.

## Tools I use

**Languages:** C++, Python, TypeScript/JavaScript, Java, SQL<br>
**Applications and data:** React, Node.js/Express, FastAPI, PostgreSQL/pgvector, DynamoDB, Redis, Kafka/Redpanda, Y.js<br>
**Infrastructure and ML:** Linux, Docker, Kubernetes, AWS Lambda, GitHub Actions CI/CD, Playwright, PyTorch
