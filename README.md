# Siddhant Kuwar

4th year CS @ UC San Diego.

I'm mostly interested in inference systems right now. The part I care about is everything between "model loaded" and "token returned": execution, memory, scheduling, kernels, serving, and what all of that costs.

## [MiniServe](https://github.com/skcache/miniserve)

I started MiniServe because calling a generation API stopped being satisfying. I wanted to know what was actually happening underneath it.

It's a small LLM inference runtime for Apple Silicon. I'm using a Python reference to lock down behavior, then rebuilding the path in C++20. Current work is around prefill/decode, KV caching, batching, request scheduling, token parity, and latency measurement. Metal comes later, if profiling gives me a reason to write the kernel.

The end goal is simple: I should be able to trace one token from the model file to streamed output and explain the runtime decisions along the way.

## [Cacheyard](https://github.com/skcache/cacheyard)

A C++20 content-addressed artifact cache.

This one is partly me forcing myself to get much better at C++ and systems fundamentals. I'm working through storage invariants, hashing, networking, concurrency, and eventually distributed behavior without abstracting the interesting parts away too early.

## Orvia

I'm also building operations software for inventory-heavy businesses.

The part I'm interested in is reducing how much people have to operate the software itself. A business already produces a ton of signals. Orders come in, inventory moves, invoices get created, suppliers respond, payments land. I want the system to reconstruct state from that activity and only interrupt someone when it actually needs a decision.

Long term, the thing I'm chasing is pretty consistent: understand the full path from models to runtimes to kernels to hardware, then get good at finding where performance and cost are being wasted.

Outside of code: basketball, markets, and whatever systems rabbit hole I got stuck in that week.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)
