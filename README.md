# Siddhant Kuwar

4th year CS @ UC San Diego.

Most of my current work is around inference systems and C++. Lately that has meant KV caches, decode paths, schedulers, latency measurements, memory behavior, and learning runtime.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)

## [MiniServe](https://github.com/skcache/miniserve)

MiniServe is a small LLM inference runtime for Apple Silicon.

The Python runtime handles the reference path for attention, generation, token selection, stopping behavior, and reproducible token outputs. The native runtime is being built in C++20 with MLX C++.

Current work is focused on prefill and decode, KV caching, request state, batching, scheduling, and benchmarking.

I track TTFT, TPOT, throughput, P50/P99 latency, and memory while changing the runtime. Token outputs are pinned against the reference implementation for correctness.

Longer term, I want more of the inference path inside MiniServe, including model loading, memory management, serving, and Metal kernels.

## [Cacheyard](https://github.com/skcache/cacheyard)

Cacheyard is a C++20 content-addressed artifact cache.

I'm working through storage semantics, hashing, ownership, TTL, eviction, networking, concurrency, observability, and eventually sharding and multi-process behavior.

I'm using the project to learn C++ and systems properly through implementation.

## Orvia Operations

I'm building **Orvia Operations**, an AI-native operations system for inventory-heavy businesses.

The system works across orders, invoices, supplier messages, barcode scans, PDFs, payments, inventory movement, and the state changes connecting them.

Current work spans inventory, orders, invoicing, supplier workflows, document ingestion, barcode input, and automation around operational state.

## Other things I've built

### [Jev Traffic Sim](https://github.com/skcache/jevtrafficsim)

A mock city traffic simulator I’m building to test Jev in a real-world control scenario and see how it compares against deterministic control.

The city runs three controllers over the same traffic environment: a fixed controller, a deterministic adaptive controller with more traffic state, and Jev

You can change traffic conditions and compare how they behave under congestion, queue buildup, starvation, and corridor flow.

### [Plywise](https://github.com/skcache/plywise)

Open-source chess analysis tool with a C++ backend and React frontend.

Imports Chess.com games or PGNs, runs Stockfish, and supports review, variations, and practice data.

### [ApplyRN](https://github.com/skcache/applyrn)

Job watcher for internships and early-career roles.

Polls 154 company job boards across Greenhouse, Ashby, Lever, SmartRecruiters, Workday, and Taleo, then sends matching roles to Telegram.

### [PR Notes](https://github.com/skcache/prnotes)

A coding-agent skill for writing concise pull request descriptions from the actual diff.

Uses before / after evidence, small flow diagrams when useful, implementation details that matter for review, and verification tied to the changed path.

### [EDN](https://github.com/skcache/edn)

A coding-agent skill that keeps a local engineering notebook in sync with the repo.

Tracks architecture, components, dependencies, data flow, tradeoffs, failure modes, and security boundaries while the code changes.

### [AirDeck](https://github.com/skcache/airdeck)

Startup technical task for a macOS webcam gesture controller with hosted vision inference and native hotkey execution.

### [Battry](https://github.com/skcache/battry-app)

Prototype for a larger idea around turning daily logs into structured energy data. Back burner for now.

## Current interests

Inference runtimes, C++, systems performance, serving economics, AI infrastructure, and operational software.

Outside code, mostly basketball and markets.
