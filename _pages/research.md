---
title: "TNSLab - Research"
layout: textlay
excerpt: "TNSLab -- Research"
sitemap: false
permalink: /research/
---

# Research Areas

The Trustworthy Networked Systems Lab (TNS Lab) advances the foundations and practice of high-performance, trustworthy networked systems. We design and evaluate programmable data planes, systems software, and security mechanisms that scale from a single server to Internet-scale infrastructure. Our work spans operating systems, networking, and security, with a strong emphasis on measurable performance, verifiable correctness, and deployability in real platforms.

---

## 1. Cloud Networking

We study network data planes that enable containers and virtual machines to exchange data efficiently and predictably. Our approach couples workload-aware software stacks with selective hardware acceleration to maximize throughput while minimizing tail latency and CPU cost.

### Focus Areas

**Per-workload network stacks**: specialization of TCP/QUIC/RDMA paths and zero-copy I/O; adaptive offload vs. host processing based on traffic mix and SLOs.

**Programmable data planes**: eBPF/XDP, DPDK, and kernel-bypass techniques for low-latency packet processing; safe in-kernel datapath extensions with verifier-friendly patterns.

**Accelerated networking**: SmartNIC/DPU/FPGA offload for compute-intensive functions (e.g., TLS/QUIC handshakes, DPI, telemetry aggregation) and queue management at line rate.

**Container/RDMA integration**: transparent RDMA support for TCP/IP workloads, verb-aware tracing, and policy-compliant redirection through user/kernelspace agents.

**Methodology**: end-to-end evaluation with throughput/latency/JCT and CPU-efficiency metrics; reproducible testbeds and open artifacts.

### Planned Directions

- Cross-layer schedulers that co-optimize NIC queues, socket stacks, and application runtimes.
- Portable offload abstractions that map network functions across CPUs, DPUs, and GPUs based on cost models.
- Automated verification of datapath transformations (e.g., offload decisions, inline rewrites) against SLA and safety constraints.

---

## 2. Cloud Security

We build practical defenses that identify and eliminate attack vectors across nodes, VMs, and containers, and we enforce policies with negligible overhead in the critical I/O path.

### Focus Areas

**Policy synthesis and enforcement**: automatic derivation of least-privilege network and system policies from workload intent, provenance, and runtime context; inline enforcement via eBPF/SmartNICs.

**Causal, multi-step attack detection**: correlating system calls, network flows, and container events to surface attacks that evade pointwise monitors.

**Zero-trust networked systems**: micro-segmentation and per-workload identity, with continuous attestation of endpoints and data paths.

**Efficient telemetry**: programmable, low-overhead collection and aggregation that preserves fidelity for forensics while bounding resource usage.

**Compatibility**: controls that work with unmodified applications and standard orchestration (Kubernetes/VM platforms).

### Planned Directions

- Learning-guided policy refinement that reduces false positives while preserving strong guarantees.
- NIC-resident enforcement frameworks that validate content and context (e.g., protocol state) at line rate.
- End-to-end evidence pipelines that link detections to actionable remediation with auditable proofs.

---

## 3. AI-Assisted Networked Systems

We leverage AI—especially large language models (LLMs)—to synthesize, optimize, and validate network functions and configurations, turning expert workflows into repeatable toolchains.

### Focus Areas

**NF synthesis and composition**: generating match-action pipelines and stateful NFs from formalized intent; compiling to safe eBPF/XDP or P4-like targets under verifier/hardware constraints.

**Autotuning and design-space exploration**: LLM-orchestrated search over protocol parameters, queueing policies, and offload placements with closed-loop measurement.

**Configuration and policy generation**: translating topology, SLOs, and traffic descriptions into deployable configurations and policy bundles (e.g., ACLs, routing, rate limits).

**Evaluation assistants**: automatic test generation, workload emulation, and regression analysis for continuous performance/robustness testing.

**Trust & safety**: guardrails that ensure generated artifacts are correct-by-construction, resource-aware, and verifiable.

### Planned Directions

- Co-design of LLM-aware compilers that emit verifier-friendly eBPF and NIC programs with proof-carrying hints.
- Reinforcement-learning controllers that adapt network stacks to live traffic while satisfying safety invariants.
- Benchmarks and open datasets for AI-driven networking and systems research.


