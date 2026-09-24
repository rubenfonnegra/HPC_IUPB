# 🚀 Week 3: How Do We Exploit Parallelism?

<span class="badge badge-blue">⚡ Parallel Computing</span>
<span class="badge badge-green">🧵 OpenMP</span>
<span class="badge badge-purple">🎮 CUDA</span>
<span class="badge badge-orange">🌐 MPI</span>


## 🎯 Objectives

* Understand how a sequential algorithm can be decomposed into parallel tasks.
* Identify opportunities for parallelism in computational algorithms.
* Differentiate between shared-memory, accelerator-based, and distributed-memory parallel computing.
* Understand the basic programming model behind OpenMP, CUDA, and MPI.
* Explain what type of computational problem each parallel programming paradigm is designed to solve.
* Recognize the advantages and limitations of CPU, GPU, and distributed parallelism.
* Select an appropriate parallel computing paradigm based on the characteristics of a computational problem.


## 📌 Topics

* 🧩 From Sequential to Parallel Algorithms
  * Task Decomposition
  * Data Decomposition
  * Independent vs. Dependent Operations
  * Synchronization and Communication

* 🧵 Shared-Memory Parallelism
  * Multicore CPUs
  * Threads
  * Shared Memory
  * Introduction to OpenMP

* 🎮 Accelerator-Based Parallelism
  * GPUs as Parallel Accelerators
  * Massive Data Parallelism
  * CPU–GPU Execution Model
  * Introduction to CUDA

* 🌐 Distributed-Memory Parallelism
  * Computing Across Multiple Nodes
  * Processes and Private Memory
  * Message Passing
  * Introduction to MPI

* 🔀 Choosing a Parallel Programming Model
  * OpenMP → Shared-Memory Systems
  * CUDA → GPU Accelerators
  * MPI → Distributed-Memory Systems
  * Hybrid Approaches


## 🧠 Activities

* 🔍 Analyze a sequential algorithm and identify which operations could execute concurrently.
* 🧩 Decompose a computational problem into independent tasks or data partitions.
* 🧵 Explore a simple OpenMP example to observe how multiple CPU cores can execute work concurrently.
* 🎮 Explore a simple CUDA example to understand how computational work can be distributed across many GPU threads.
* 🌐 Examine a basic MPI example to understand how processes running on different computing nodes communicate.
* ⚖️ Compare OpenMP, CUDA, and MPI in terms of memory model, hardware, communication, and typical use cases.
* 🤖 Discuss which parallel programming model would be appropriate for common AI workloads such as matrix multiplication, neural network training, and large-scale data processing.
* 📝 Solve a short scenario-based exercise by selecting the most appropriate parallel programming paradigm for different computational problems.


> **💡 Weekly Challenge**
>
> Choose a computational algorithm or AI workload from your research area and imagine that you need to significantly reduce its execution time.
>
> * Which parts of the algorithm could run in parallel?
> * Would you divide the computation by tasks, by data, or both?
> * Would you use OpenMP, CUDA, MPI, or a combination of them?
> * What data would need to be shared or communicated?
> * What could prevent the algorithm from achieving perfect parallel speedup?
