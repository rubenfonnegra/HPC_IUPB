# 🖥️ Week 2: Why Does Hardware Matter?


<span class="badge badge-blue">⚡ Performance</span>
<span class="badge badge-green">🖥️ Computer Architecture</span>
<span class="badge badge-purple">🤖 AI Computing</span>

## 🎯 Objectives

* Understand the theoretical limits of parallel performance using Amdahl’s Law and Gustafson’s Law.
* Identify the sources and impact of computational and communication overhead.
* Differentiate between compute-bound and memory-bound workloads.
* Explain how CPU architecture, cores, cache, and memory hierarchy affect algorithm performance.
* Understand the role of SIMD and NUMA in modern high-performance systems.
* Compare CPU and GPU architectures from a parallel computing perspective.
* Understand GPU memory hierarchy and the role of specialized hardware such as Tensor Cores.
* Connect hardware architecture with common AI operations such as matrix multiplication, convolutions, and attention.


## 📌 Topics

* ⚖️ Limits of Parallel Computing
  * Amdahl’s Law
  * Gustafson’s Law
  * Parallel Overhead

* 🧠 Performance Bottlenecks
  * Compute-Bound Workloads
  * Memory-Bound Workloads

* 🖥️ CPU Architecture
  * CPU Cores
  * Cache Hierarchy
  * Main Memory
  * SIMD — Single Instruction, Multiple Data
  * NUMA — Non-Uniform Memory Access

* 🎮 GPU Architecture
  * Massive Parallelism
  * Thousands of Computing Cores
  * GPU Memory Hierarchy
  * Tensor Cores

* 🤖 Hardware for Artificial Intelligence
  * Matrix Multiplication
  * Convolutions
  * Attention Mechanisms
  * Why AI Workloads Benefit from Parallel Hardware


## 🧠 Activities

* 🧮 Apply Amdahl’s Law to estimate the maximum theoretical speedup of different parallel workloads.
* 📈 Compare Amdahl’s Law and Gustafson’s Law under different problem sizes and numbers of processors.
* 🔍 Analyze simple programs and determine whether they are compute-bound or memory-bound.
* 🖥️ Explore the architecture of a modern CPU and identify cores, cache levels, memory, and vector-processing capabilities.
* 🎮 Compare CPU and GPU architectures and discuss why GPUs can execute thousands of operations concurrently.
* 🧮 Examine matrix multiplication as an example of a highly parallel computational operation.
* 🤖 Connect common AI operations—including matrix multiplication, convolution, and attention—to the hardware components used to accelerate them.
* 📝 Solve a short architecture-performance exercise to identify potential bottlenecks in different computational workloads.


> **💡 Weekly Challenge**
>
> Consider a computationally intensive AI workload, such as training a neural network, processing images with a CNN, or running a Transformer model.
>
> * Which operations are responsible for most of the computation?
> * Would you expect the workload to be compute-bound or memory-bound?
> * Which hardware characteristics would have the greatest impact on its performance?
> * Why might a GPU outperform a CPU for this workload?
> * Would adding more computing cores always make the program faster?
