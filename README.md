# Hi, I'm Yash Patil 👋

🎓 MS in Computer Science @ Northeastern University
⚙️ Backend & Distributed Systems Engineer | High-Performance Systems

I build **high-performance, fault-tolerant systems** with a focus on **concurrency, low-latency messaging, distributed storage, and matching-engine infrastructure**.
My work emphasizes **measurable performance, correctness under failure, and production-grade system design**.

---

## 🔧 Technical Focus

- **Concurrent & Lock-Free Programming** (C++ atomics, SPSC/MPSC queues, fine-grained locking)
- **Distributed Systems** (consistent hashing, replication, fault tolerance)
- **Low-Latency Trading Infrastructure** (order books, matching engines, price-time priority)
- **Performance Engineering** (P99 latency, throughput benchmarking)
- **Reliability** (WAL, checkpoints, crash recovery, chaos testing)

---

## 🚀 Featured Projects

### **[LiquidBook](https://github.com/yashpatil-byte/LiquidBook) — Limit Order Book & Matching Engine**
*C++17 · Lock-Free Programming · CMake · GoogleTest · Google Benchmark*

- Built a limit order book implementing **price-time priority matching** across LIMIT, MARKET, IOC, and FOK order types
- Achieved **1.8× faster best-price lookup** by replacing a `std::map`-based design with a flat array + bitmap index (O(log n) → O(1))
- Implemented a **lock-free SPSC ingress queue** with cache-line padding and release/acquire memory ordering
- Verified correctness via **randomized differential testing** against a reference engine across 43 test cases
- Zero heap allocation on the critical path via intrusive linked lists

---

### **NanoMQ — Ultra-Low-Latency Message Queue**
*C++17 · Lock-Free Programming · Memory-Mapped I/O · Atomics · CMake · Docker*

- Built a C++ message queue achieving **1.2M msg/sec throughput** with **83ns P99 latency** using lock-free SPSC ring buffers
- Implemented a **crash-recoverable WAL** with sequential writes and CRC32 checks ensuring zero message loss
- Reduced CPU usage by **73%** at 500K msg/sec load through zero-copy memory-mapped I/O

---

### **MiniKV — Distributed Key-Value Store**
*Python · FastAPI · Consistent Hashing · Merkle Trees · Prometheus*

- Built distributed storage handling **250K ops/sec** with **<5ms P99 latency** using a 3-node cluster and consistent hashing
- Reduced sync time by **85%** (30s → 4.5s) through async replication with Merkle-tree conflict detection
- Maintained **99.9% uptime** during failures via automated health monitoring and instant failover

---

### **Concurrent File Server** *(CS 5600: Computer Systems — Northeastern)*
*C · POSIX Threads · TCP Sockets · GNU Make*

- Designed a multi-threaded TCP file server in C with a custom binary RPC protocol for concurrent, thread-safe file operations
- Implemented **sharded LRU block caching** with path-hashed keys, per-shard locks, and inode stale checks
- Added an **adaptive two-tier cache** with background threshold/memory rebalancing, with latency and hit-rate metrics for evaluation

---

## 🛠 Tech Stack

**Languages:** C++, Go, Python, C, Java, SQL, Bash
**Systems:** Concurrency, Distributed Systems, Fault Tolerance, WAL, Backpressure
**Databases:** PostgreSQL, MySQL, Redis, MongoDB, BoltDB
**Cloud & DevOps:** AWS, Docker, Kubernetes, CI/CD, Linux
**Observability:** Prometheus, Grafana

---

## 💼 Experience

**Software Development Engineer Intern — Infosys** *(Nov 2024 – Feb 2025)*
- Created a distributed stream processor handling **163K events/sec** with **<20μs P99 latency** via concurrency and hash partitioning
- Reduced recovery time by **90%** (30s → 3s) with automated checkpointing and a replay mechanism ensuring zero data loss
- Stabilized the system under 10× traffic spikes, maintaining 99%+ throughput through adaptive backpressure and flow control

**Software Development Engineer Intern — JustDial** *(Jun 2023 – Sept 2023)*
- Built an ML prediction platform serving **100K predictions/sec** with **99.99% uptime** using Kafka streaming and Redis caching
- Reduced infrastructure costs by **40%** through multi-instance deployment with load balancing and circuit breakers
- Achieved **sub-5ms P99 response time** across 10+ distributed instances using gRPC and health monitoring

---

## 📫 Let's Connect

- **GitHub:** [github.com/yashpatil-byte](https://github.com/yashpatil-byte)
- **LinkedIn:** [linkedin.com/in/yashpatil](https://www.linkedin.com/in/yash-patil-57a53a1a6)
- **Email:** yashpatilcareer@gmail.com

---

⭐ If you're interested in **low-latency systems, distributed infrastructure, or trading technology**, feel free to explore my projects or reach out.
