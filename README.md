# Siddhant Kuwar

4th year CS @ UC San Diego.

Most of my current work is around inference systems and C++. Lately that has meant KV caches, decode paths, schedulers, latency measurements, memory behavior, and learning runtime.

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

## Current interests

Inference runtimes, C++, systems performance, serving economics, AI infrastructure, and operational software.

Outside code, mostly basketball and markets.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache)
