# Cache Simulator

A high-performance cache memory simulator developed in **C** to analyze the impact of architectural configurations on system performance. This tool models the interaction between a CPU and its memory hierarchy, providing a detailed analysis of hit/miss ratios, memory latency, and data throughput.

## 🚀 Key Features
* **Flexible Mapping:** Supports Direct-Mapped, N-Way Set Associative, and Fully Associative cache configurations.
* **Replacement Logic:** Implements the **LRU (Least Recently Used)** replacement algorithm to simulate realistic hardware behavior and cache aging.
* **Trace-Driven Analysis:** Processes memory trace files to simulate real-world CPU memory access patterns (Read/Write).
* **Performance Metrics:** Outputs comprehensive statistics including:
    * Total Cache Hits/Misses
    * Hit/Miss Ratios
    * Memory Write-Back operations
    * Analysis of Tag, Index, and Offset bits

## 🛠 Technical Stack
* **Language:** C (Standard C99/C11)
* **Environment:** Linux / Unix / macOS
* **Concepts:** Computer Architecture, Memory Management, Bitwise Operations, and Pointers.

## 📐 Architectural Logic
The simulator performs address translation by decomposing 32-bit or 64-bit memory addresses into:
1. **Tag:** To verify the identity of the cached data.
2. **Index:** To map the address to a specific set within the cache.
3. **Block Offset:** To identify the specific byte within the cache line.

## 📋 Getting Started

### Prerequisites
* GCC (GNU Compiler Collection)
* Make

### Installation & Compilation
Clone the repository and compile using the provided Makefile:
```bash
git clone [https://github.com/elsamird003/Cache-Simulator.git](https://github.com/elsamird003/Cache-Simulator.git)
cd Cache-Simulator
make
