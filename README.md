# Siddhant Kuwar

CS @ UC San Diego.

I like systems where the abstraction eventually stops being useful and I have to figure out what is actually happening underneath it.

Right now I'm mostly working on **AI inference and systems**: model execution, memory, scheduling, kernels, serving, and the economics behind all of it.

I don't care much about collecting frameworks. I care about knowing where the latency, memory, and money go.

## Building

### [MiniServe](https://github.com/skcache/miniserve)

A small LLM inference runtime for Apple Silicon.

I'm building it from a readable Python reference toward a C++20 runtime, then dropping into Metal where profiling says it is worth it.

Current work includes:

- explicit prefill / decode paths
- KV-cache design and memory behavior
- batching and request scheduling
- token-parity correctness checks
- TTFT, TPOT, throughput, and P50/P99 latency measurements

The point is not to wrap another serving library. I want to be able to trace one token from the model file to streamed output and explain the runtime decisions along the way.

### [Cacheyard](https://github.com/skcache/cacheyard)

A C++20 content-addressed artifact cache I'm building to get deeper into storage, networking, concurrency, and distributed systems.

I'm keeping the project deliberately low-level: define the invariants first, then build the storage and serving path instead of hiding the hard parts behind libraries.

### Orvia

AI-native operations software for inventory-heavy businesses.

The idea is simple: operational software should need less explicit input. The system should observe the signals a business already produces, reconstruct state, detect what changed, and either act or ask for the smallest possible human decision.

## What I'm trying to get good at

Cross-layer systems work: models → runtimes → kernels → hardware → fleets.

Long term, I want to understand how to make increasingly capable models economically deployable on finite hardware.

Outside code: basketball, markets, and spending too much time pulling apart systems that were working perfectly fine before I got curious.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)
