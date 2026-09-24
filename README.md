# Siddhant Kuwar

4th year CS @ UC San Diego.

Most of what I’m working on right now is around inference systems, C++, performance, and just getting better at understanding what actually happens below the API layer.

I like building stuff where I can measure what changed instead of just saying it got better.

[LinkedIn](https://www.linkedin.com/in/skuwar) · [X](https://x.com/skcache) · [Email](mailto:siddhankuwar116@gmail.com)

## [MiniServe](https://github.com/skcache/miniserve)

Probably the project I care about the most right now.

MiniServe is a small LLM inference runtime for Apple Silicon. I started with a Python reference implementation so I could actually understand attention, generation, token selection, stopping, all that stuff, and now I’m moving more of it into C++ with MLX.

Right now I’m mostly working on prefill, decode, KV caching, request state, batching, scheduling, and benchmarking.

I track TTFT, TPOT, throughput, tail latency, memory, whatever is useful for the thing I’m changing, and I keep token outputs pinned against the reference implementation so I know I didn’t just make it faster and wrong.

Long term I want to push more of the inference path into it, especially memory management, serving, and eventually Metal kernels.

## [Cacheyard](https://github.com/skcache/cacheyard)

C++20 content-addressed artifact cache.

This one is mostly me forcing myself to learn systems properly by building the pieces instead of reading about them forever.

So far that means hashing, ownership, TTL, eviction, networking, concurrency, observability, and eventually sharding / multi-process stuff.

## Orvia Operations

This is the product I’m building.

Orvia is an operations system for inventory-heavy businesses, so suppliers, wholesalers, warehouses, that kind of thing.

The main idea is that people running these businesses already create a ton of signals through orders, invoices, emails, scans, PDFs, payments, inventory movement etc, and the software should understand as much of that as possible without making them manually enter everything again.

Right now I’m working across inventory, orders, invoicing, supplier workflows, barcode input, document ingestion, and automating more of the state changes between all of it.

## Some other stuff

### [Jev Traffic Sim](https://github.com/skcache/jevtrafficsim)

A traffic simulator I built to test Jev in something closer to a real control problem.

It runs fixed control, deterministic adaptive control, and Jev over the same city so you can mess with congestion, queues, starvation, corridor flow, accidents, closures, rain, whatever, and see how the controllers behave.

### [Plywise](https://github.com/skcache/plywise)

Open-source chess analysis tool with a C++ backend and React frontend.

Imports Chess.com games or PGNs, runs Stockfish, and supports review, variations, and practice.

### [ApplyRN](https://github.com/skcache/applyrn)

Job watcher I built because manually checking company boards is miserable.

Polls 154 company job boards across Greenhouse, Ashby, Lever, SmartRecruiters, Workday, and Taleo, then sends matching roles to Telegram.

### [PR Notes](https://github.com/skcache/prnotes)

Small coding-agent skill for writing better PR descriptions from the actual diff.

It can pull in before / after evidence, add a small flow diagram when it actually helps, and keep the note focused on what changed and how it was verified.

### [EDN](https://github.com/skcache/edn)

Another coding-agent skill, this one keeps a local engineering notebook synced with the repo while you work.

Mostly tracks architecture, components, dependencies, data flow, tradeoffs, failure modes, security boundaries, stuff that usually ends up scattered across your head and random notes.

### [AirDeck](https://github.com/skcache/airdeck)

macOS webcam gesture controller I built for a startup technical task.

Hosted vision inference on one side, native hotkey execution on the other.

### [Battry](https://github.com/skcache/battry-app)

Prototype around turning daily logs into structured energy data.

This one is on the back burner right now.

## What I’m into right now

Inference runtimes, C++, systems performance, AI infrastructure, serving economics, operational software.

Outside code, mostly basketball and markets.
