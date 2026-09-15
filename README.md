# Siddhant Kuwar

4th year CS @ UC San Diego.

Lately I've been spending most of my time around inference systems and C++. I keep getting pulled toward the parts of the stack where behavior stops being obvious. KV memory, scheduling, batching, kernels, device behavior, latency, cost. Once I can see the path end to end, I usually want to keep going lower.

## [MiniServe](https://github.com/skcache/miniserve)

A small LLM inference runtime for Apple Silicon.

MiniServe started as a way to get past the high-level generation path and see what was actually happening during inference. The Python side gives me a reference implementation I can inspect and test against. The native side is moving into C++20 with MLX C++, with separate prefill and decode paths, KV caching, request state, batching, scheduling, and benchmarking.

I'm tracking TTFT, TPOT, throughput, tail latency, and memory while the runtime changes underneath it. The token path stays pinned so I can tell when a performance change also changed behavior.

Eventually I want the runtime to own more of the path itself. Model loading, memory management, scheduling, serving, and selected Metal work are all in scope. The repo is still early enough that the interesting part is watching the abstractions disappear one by one.

## [Cacheyard](https://github.com/skcache/cacheyard)

A C++20 content-addressed artifact cache.

I'm using Cacheyard to get much sharper on systems fundamentals through something that has to deal with actual state and contention. Storage semantics, hashing, ownership, TTL and eviction, networking, concurrency, observability, and eventually sharding and multi-process behavior all show up naturally here.

The implementation is still early. I care more about getting the invariants right now than racing toward a distributed architecture I don't understand well enough yet.

## Orvia Operations

I'm also building **Orvia Operations**, an AI-native operations system for inventory-heavy businesses.

A lot of operational work still leaks through email, PDFs, barcode scans, supplier messages, invoices, spreadsheets, payments, and someone's memory. Orvia sits in that mess and tries to keep the system state current as those signals arrive.

The interesting part for me is reducing how often someone has to stop what they're doing, open software, find the right screen, and explain to the system what already happened in the real world.

I'm building this seriously and pushing it toward something we can put in front of accelerators in the next few months.

## Current interests

Inference runtimes, C++, systems performance, serving economics, and software that removes work instead of moving it into a nicer interface.

Outside code, mostly basketball and markets.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)
