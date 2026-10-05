# Hey, I'm Siddhant

<img align="right" src="./sk-wordmark.svg" width="315" alt="Animated ASCII SK wordmark" />

4th year CS @ UC San Diego.

I’m mostly interested in inference systems, C++, performance, and the systems underneath modern AI workloads.

A lot of what I build comes from wanting to understand something properly by implementing it, measuring it, and then pushing it further.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com) · [Website](https://skx.si)

<br clear="right" />

## [MiniServe](https://github.com/skcache/miniserve)

LLM inference runtime for Apple Silicon.

I started with a Python reference implementation and have been moving more of the runtime into C++ / MLX.

Current work is around prefill, decode, KV caching, request state, batching, scheduling, memory behavior, and benchmarking.

I track TTFT, TPOT, throughput, tail latency, and memory, with outputs checked against the reference implementation while I optimize.

## [Cacheyard](https://github.com/skcache/cacheyard)

C++20 content-addressed artifact cache.

Built around hashing, ownership, TTL, eviction, networking, concurrency, and observability.

I’m using it to go deeper on systems design and eventually push into sharding and multi-process cache behavior.

## [ApplyRN](https://github.com/skcache/applyrn)

Job monitoring system that polls 154 company career sites across Greenhouse, Ashby, Lever, SmartRecruiters, Workday, and Taleo.

Matching roles are filtered and sent to Telegram.

Built because checking job boards manually is miserable.

## [Jev Traffic Sim](https://github.com/skcache/jevtrafficsim)

Deterministic traffic-control simulator for comparing fixed, adaptive, and structured-policy controllers under the same scenarios.

Supports congestion, accidents, closures, rain, events, starvation, corridor flow, and seeded replay for controller comparison.

## Other work

- [Plywise](https://github.com/skcache/plywise) — C++ / React chess analysis tool built around Stockfish.
- [EDN](https://github.com/skcache/edn) — repo-local engineering notebook for architecture, dependencies, design decisions, failure modes, and security boundaries.
- [PR Notes](https://github.com/skcache/prnotes) — coding-agent skill for generating PR documentation from diffs and verification evidence.
- [AirDeck](https://github.com/skcache/airdeck) — macOS webcam gesture controller using hosted vision inference and native hotkey execution.

## Currently interested in

Inference runtimes, AI serving, performance engineering, C++, systems, and warehouse / distribution software.

I'm currently looking for new-grad software engineering roles in systems, infrastructure, and AI inference, and I'm open to selective contract work where the technical fit makes sense.
