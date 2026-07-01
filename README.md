# Hi, I’m Yash Patil 👋  

🎓 MS in Computer Science @ Northeastern University  
⚙️ Systems & Infrastructure Engineer | Distributed Systems | Performance Engineering  

I build **high-performance, fault-tolerant systems** with a focus on **concurrency, low-latency messaging, streaming engines, and distributed storage**.  
My work emphasizes **measurable performance, correctness under failure, and production-grade system design**.

---

## 🔧 Technical Focus
- **Concurrent & Lock-Free Programming** (C++ atomics, fine-grained locking)
- **Distributed Systems** (replication, partitioning, fault tolerance)
- **Streaming & Messaging Systems** (exactly-once semantics, backpressure)
- **Performance Engineering** (P99 latency, throughput benchmarking)
- **Reliability** (WAL, checkpoints, chaos testing, recovery)

---

## 🚀 Featured Projects

### **StreamFlow — Distributed Real-Time Stream Processing Engine**
*Go · Kafka · BoltDB · Prometheus · Docker*  
- Achieved **163K events/sec** with **<20µs P99 latency** using hash-partitioned parallel workers  
- Implemented **event-time windowing** (tumbling, sliding, session) with millisecond precision  
- Built **checkpoint-replay** system enabling **exactly-once processing** and <8s recovery  
- Integrated **token-bucket backpressure** to sustain throughput under **10× traffic spikes**

---

### **NanoMQ — Ultra-Low-Latency Message Queue**
*C++17 · Lock-Free Programming · mmap · Docker*  
- Built **lock-free SPSC queue** achieving **83ns P99 latency** and **1.2M msgs/sec**  
- Reduced CPU utilization by **73%** using **zero-copy memory-mapped I/O**  
- Designed **crash-recoverable WAL** with CRC32 integrity for zero message loss  
- Validated with extensive benchmarks, stress tests, and containerized deployment

---

### **MiniKV — Distributed Key-Value Store**
*Python · FastAPI · Consistent Hashing · Prometheus · Docker*  
- Architected **3-node distributed KV store** delivering **250K+ ops/sec** with **<5ms P99 latency**  
- Implemented **async replication** with **Merkle-tree anti-entropy**, cutting recovery time by **85%**  
- Built **heartbeat-based failover** ensuring **99.9% availability** during node failures  
- Verified reliability using **chaos testing** and network partition simulations

---

### **SwiftLoad — Multithreaded File Downloader**
*Python · concurrent.futures · Docker · Linux*  
- Improved download throughput by **41.7% (1.71×)** using HTTP Range request parallelism  
- Designed **deadlock-free, thread-safe file writer** with zero corruption across **1,000+ concurrent writes**  
- Implemented **exponential backoff retries** improving success rate by **35% under packet loss**  
- Delivered modular, test-driven architecture with **48+ unit/integration/performance tests**

---

## 🛠 Tech Stack

**Languages:** Python, C++, C, Java, SQL, Bash  
**Databases:** PostgreSQL, MySQL, MongoDB, SQLite, Redis  
**Systems & Cloud:** Linux, Docker, AWS, GCP, FastAPI, Flask  
**Tools:** Git, CMake, Jenkins, Prometheus, NumPy, PyTorch, TensorFlow  

---

## 💼 Experience

Software Development Engineer Intern — Infosys
- Built distributed stream processor handling 163K events/sec with <20µs P99 latency using concurrency and hash partitioning
- Reduced recovery time 90% (30s → 3s) through automated checkpointing with replay mechanism ensuring zero data loss
- Stabilized system under 10x traffic spikes maintaining 99%+ throughput via adaptive backpressure and flow control

Software Development Engineer Intern — JustDial
- Built ML prediction platform serving 100K predictions/sec with 99.99% uptime using Kafka streaming and Redis caching
- Reduced infrastructure costs 40% through multi-instance deployment with load balancing and circuit breakers
- Achieved sub-5ms P99 response time across 10+ distributed instances using gRPC and health monitoring

---

## 📫 Let’s Connect
- **GitHub:** https://github.com/yashpatil-byte  
- **LinkedIn:** https://www.linkedin.com/in/yash-patil-57a53a1a6  
- **Email:** yashpatilcareer@gmail.com  

---

⭐ If you’re interested in **systems engineering, distributed infrastructure, or performance-critical software**, feel free to explore my projects or reach out.
