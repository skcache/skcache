# Siddhant Kuwar

4th year CS @ UC San Diego. Most of my time right now goes into inference systems, C++, and building software I can actually explain end to end.

```text
model execution
      ↓
prefill / decode
      ↓
KV memory + scheduling
      ↓
kernels / device runtime
      ↓
serving + cost
```

That stack is where I want to get unusually good.

## [MiniServe](https://github.com/skcache/miniserve)

A small LLM inference runtime for Apple Silicon.

I started it because I wanted to understand the full path from model weights to generated tokens instead of treating inference as one opaque call.

The current runtime work is around:

- prefill and decode as separate execution paths
- KV-cache layout, growth, reuse, and memory cost
- request state, batching, and scheduling
- token-level parity between reference and native paths
- TTFT, TPOT, throughput, P50/P99 latency, and memory measurements
- C++20 + MLX C++ now, with Metal kernels later where profiling shows a real bottleneck

I keep a slower reference implementation around so the faster path has something concrete to match. The useful part of this project is being able to change one layer and see exactly what happened to correctness, latency, or memory.

## [Cacheyard](https://github.com/skcache/cacheyard)

A C++20 content-addressed artifact cache.

This is where I'm getting deeper into systems fundamentals through something with real constraints: content hashing, storage semantics, ownership, TTL/eviction, TCP/HTTP serving, concurrency, observability, and eventually sharding / multi-process behavior.

I'm building it in small pieces and keeping the invariants explicit before adding more moving parts. The point is to understand what the cache is doing under load, where contention shows up, and how the design changes as the system gets less toy-like.

## Orvia Operations

I'm building **Orvia Operations**, an AI-native operations system for inventory-heavy businesses: distributors, wholesalers, suppliers, warehouses, and similar businesses where a lot of work still happens through forms, spreadsheets, email, scanners, PDFs, and people remembering what to do next.

The product direction is to reduce how much software people have to operate manually. Orders, inventory movement, invoices, supplier messages, barcode scans, payments, and documents already produce useful signals. Orvia is being built to turn those signals into operational state, catch what changed, and move the workflow forward with as little manual input as possible.

A lot of the work now is less "build another dashboard" and more figuring out where the system can reliably infer state, automate the boring path, and only pull a human in when judgment is actually needed.

## What I'm working toward

I want to get very good at the systems and economics of inference: how model architecture, runtime behavior, memory, kernels, hardware, and serving policy all show up in latency and cost.

I also like product problems where the software can remove entire chunks of human workflow instead of making the workflow prettier.

Outside of code: basketball, markets, and whatever technical rabbit hole I managed to turn into a project that week.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)
