# ⚡ Week 6: Performance Engineering — Where Is the Bottleneck?

<span class="badge badge-blue">⚡ Performance</span>
<span class="badge badge-green">📊 Benchmarking</span>
<span class="badge badge-purple">🔍 Profiling</span>


## 🎯 Objectives

* Understand the role of performance engineering in High Performance Computing.
* Establish a reproducible performance baseline before attempting optimization.
* Differentiate between wall-clock time, CPU time, latency, and throughput.
* Understand FLOPS as a measure of computational performance and recognize its limitations.
* Measure CPU and GPU utilization to identify underused computational resources.
* Decompose total execution time into loading, preprocessing, data transfer, computation, synchronization, communication, and I/O.
* Use profiling to identify where a program actually spends its execution time.
* Distinguish between compute-bound, memory-bound, I/O-bound, and communication-bound workloads.
* Form evidence-based optimization hypotheses instead of optimizing code blindly.
* Validate that performance optimizations preserve the analytical correctness of the original computation.


## 📌 Topics

* ⏱️ Measuring Performance
  * Baseline
  * Benchmarking
  * Wall-Clock Time vs. CPU Time
  * Latency
  * Throughput
  * FLOPS

* 📊 Resource Utilization
  * CPU Utilization
  * GPU Utilization
  * Memory Usage
  * Resource Saturation

* 🔍 Profiling
  * Where Does the Program Spend Its Time?
  * Function-Level Profiling
  * Identifying Hotspots
  * Cumulative Execution Time
  * Call Frequency

* 🧩 Execution-Time Decomposition
  * Data Loading
  * Data Preprocessing
  * CPU ↔ GPU Data Transfer
  * Computation
  * Synchronization
  * Communication
  * Input / Output

* 🚧 Performance Bottlenecks
  * Compute-Bound Workloads
  * Memory-Bound Workloads
  * I/O-Bound Workloads
  * Communication-Bound Workloads
  * Python and Framework Overhead

* 🛠️ Performance Engineering Tools
  * `time`
  * `htop`
  * `perf`
  * `nvidia-smi`
  * Python Profiling Tools

* 🧪 Optimization as an Experiment
  * Measure Before Optimizing
  * Identify the Bottleneck
  * Form an Optimization Hypothesis
  * Change One Component
  * Benchmark Again
  * Validate Analytical Equivalence


## ⏱️ Where Does the Time Go?

A useful way to reason about application performance is to decompose total execution time:

```
Ttotal =
    Tload
  + Tpreprocess
  + Ttransfer
  + Tcompute
  + Tsync
  + Tcommunication
  + TIO
```