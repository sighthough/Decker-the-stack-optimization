# Decker-the-stack-optimization
Decker is A lightweight, core-aware execution engine featuring explicit dependency mapping, dynamic time-slicing quotas, and intelligent loop memoization.

The goal was simple, make something better than stacks 
introducing decker 
benchmark showing off its speed [here](https://sighthough.github.io/Decker-the-stack-optimization/)

*Co-authored by [sighthough](https://youtu.be/UtPiUGwu-0Q) and [Googles Gemini](https://www.youtube.com/shorts/R3Qo4rBgrD8).*

rust version is in the repo with the basic functions of it so it can be transfered to different languages 
also feel free to rip the index (its the benchmark) for anything you need 

Readme :

# Decker: Core-Aware, Dependency-Mapped Execution Engine

> A lightweight, high-performance execution engine featuring explicit dependency mapping, dynamic core-aware time-slicing quotas, and intelligent loop memoization.

## 🚀 Overview

Decker is an experimental runtime architecture designed to bypass the bottlenecks of traditional linear stacks and rigid LIFO queues. By scanning ahead for explicit dependencies, matching task quotas directly to host hardware threads, and utilizing optimization probes for loops, Decker achieves massive performance gains over standard sequential execution models.

## ✨ Key Features

* **Explicit Dependency Mapping:** Tasks declare their prerequisites upfront, eliminating blind blocking and unnecessary stall times.
* **Core-Aware Quota Scaling:** Automatically calibrates active task pools to match the host system's physical CPU cores.
* **Dynamic Time-Slicing:** Distributes processor cycles fairly among active tasks without exploding CPU overhead.
* **Smart Loop Optimization:** Evaluates loop behavior via optimization probes—memoizing static loops and parallelizing dynamic chunks across available cores.
* **Fail-Fast Iron Rule:** Halts execution instantly upon encountering fatal instruction faults to protect system integrity.

## 📊 Benchmark Performance

In rigorous heavy-duty stress tests, Decker's optimized scheduling pipeline significantly outperforms traditional sequential stacks:

| Metric | Standard Engine (Linear Stack) | Decker Engine (Core-Aware + Memoized) | Performance Gain |
| :--- | :--- | :--- | :--- |
| **Execution Duration** | Baseline | Optimized | **Significantly Faster** |
| **CPU Operations** | Sequential Grind | Parallelized Pool | **Redundant Ops Avoided** |
| **Concurrency Model** | Single-threaded queue | Hardware-mapped adaptive quota | **Maximized Throughput** |
