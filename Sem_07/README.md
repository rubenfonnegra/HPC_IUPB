# ⚡ Week 7: From Bottlenecks to Parallelism — Where Should My Algorithm Run?

<span class="badge badge-blue">⚡ Parallel Computing</span>
<span class="badge badge-green">🖥️ CPU Computing</span>
<span class="badge badge-purple">🎮 GPU Computing</span>


## 🎯 Objectives

* Connect performance profiling with parallel computing decisions.
* Identify computational hotspots that may benefit from parallel execution.
* Analyze data and control dependencies before attempting to parallelize an algorithm.
* Recognize different forms of parallelism, including data parallelism and task parallelism.
* Understand how workload characteristics influence the choice between sequential CPU, multicore CPU, and GPU execution.
* Understand the overhead associated with multiprocessing and GPU execution.
* Compare implementations using execution time, speedup, efficiency, and analytical equivalence.


## 📌 Topics

* 🔍 From Profiling to Parallelization
  * Performance Hotspots
  * Bottleneck Identification
  * Computational Cost
  * Optimization Candidates

* 🔗 Dependency Analysis
  * Data Dependencies
  * Control Dependencies
  * Independent Operations
  * Sequential Dependencies
  * Parallelizable Loops

* ⚡ Finding Parallelism
  * Data Parallelism
  * Task Parallelism
  * Work Decomposition
  * Granularity
  * Independent Chunks

* 🖥️ Multicore CPU Computing
  * Processes and Workers
  * Multiprocessing
  * Work Distribution
  * Chunking
  * Process Creation Overhead
  * Inter-Process Communication
  * Combining Partial Results

* 🧭 CPU or GPU?
  * Workload Size
  * Computational Intensity
  * Memory Requirements
  * Data Transfer Cost
  * Parallelism Degree
  * Hardware Availability


## 🧠 From Bottleneck to Parallel Execution

Finding a bottleneck does not automatically mean that it should be parallelized.

The first question is:

> **Does the hotspot contain independent work that can execute simultaneously?**

A useful workflow is:

```text
PROFILE
   ↓
IDENTIFY HOTSPOT
   ↓
ANALYZE DEPENDENCIES
   ↓
FIND PARALLELISM
   ↓
CHOOSE CPU / GPU
   ↓
MAP THE WORKLOAD
   ↓
MEASURE AGAIN