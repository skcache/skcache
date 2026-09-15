# Siddhant Kuwar

4th year CS @ UC San Diego. Mostly working down the inference stack right now.

```text
models
  ↓
runtime
  ↓
memory + scheduling
  ↓
kernels
  ↓
hardware
  ↓
serving cost
```

## [MiniServe](https://github.com/skcache/miniserve)

LLM inference runtime for Apple Silicon.

Python reference first, then C++20. I'm working through prefill/decode, KV-cache behavior, batching, scheduling, and the measurements around them: TTFT, TPOT, throughput, P50/P99, memory.

The reference path pins token behavior before I start changing the runtime underneath it. Metal comes after profiling tells me where it is actually worth touching.

## [Cacheyard](https://github.com/skcache/cacheyard)

C++20 content-addressed artifact cache.

I'm using it to get much better at the systems pieces I don't want to hand-wave: storage invariants, hashing, ownership, networking, concurrency, and eventually distributed behavior.

## Orvia

Operations software for inventory-heavy businesses. I'm exploring how much explicit software interaction can disappear if the system can reconstruct state from the signals the business already produces.

Lately I've been spending most of my time on inference, C++, systems performance, and the economics of running models on finite hardware.

Basketball and markets usually eat whatever time is left.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)
