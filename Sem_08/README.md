# 🧠 Week 9: How Do We Move and Process Data Efficiently?

<span class="badge badge-blue">🧠 Memory Systems</span>  
<span class="badge badge-green">📦 Batching</span>  
<span class="badge badge-purple">📊 High-Dimensional Data</span>

## 🎯 Objectives

- Understand how data movement affects computational performance.
- Distinguish latency, bandwidth, and locality as key performance factors.
- Analyze how memory access patterns influence execution time.
- Understand why CPU–GPU transfers can become a major source of overhead.
- Use batching and chunking to process datasets that do not fit entirely in memory.
- Evaluate the trade-off between batch size, memory consumption, and throughput.
- Apply profiling principles to identify bottlenecks across the complete data pipeline.

## 📌 Topics

- Memory Hierarchy
- Data Movement
- Latency, Bandwidth, and Locality
- Batching and Chunking
- Data Loading Pipelines
- High-Dimensional Data
- Dense and Sparse Representations
- Numerical Precision
- Precision–Performance Trade-offs

## 🧠 Performance Is More Than Computation

A processor can be extremely fast and still spend a significant amount of time waiting.

The reason is simple:

> **Fast computation is only useful if data can reach the processor fast enough.**

A typical computational pipeline involves several stages:

```text
STORAGE
   ↓
RAM
   ↓
CACHE
   ↓
CPU / GPU
   ↓
COMPUTATION