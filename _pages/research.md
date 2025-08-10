---
title: "TNSLab - Research"
layout: textlay
excerpt: "TNSLab -- Research"
sitemap: false
permalink: /research/
---

# Research Areas

The Trustworthy Networked Systems Lab (TNS Lab) advances the foundations and practice of high-performance, trustworthy networked systems. We design and evaluate programmable data planes, systems software, and security mechanisms that scale from a single server to cloud-scale infrastructure.

---

## 1. Cloud Networking

We study cloud network data planes that enable containers and virtual machines to exchange data efficiently and predictably. Our approach couples workload-aware software stacks with selective hardware acceleration to maximize throughput while minimizing tail latency and CPU cost.

### Focus Areas

**Programmable data planes**: eBPF/XDP, DPDK, and kernel-bypass techniques for low-latency packet processing; safe in-kernel datapath extensions with verifier-friendly patterns.

**Accelerated networking**: SmartNIC/DPU/FPGA offload for compute-intensive functions (e.g., TLS/QUIC handshakes, DPI, telemetry aggregation) and queue management at line rate.

**Container/RDMA integration**: transparent RDMA support for TCP/IP workloads, verb-aware tracing, and policy-compliant redirection through user/kernelspace agents.

---

## 2. Cloud Security

We build practical security systems that identify and eliminate attack vectors across nodes, VMs, and containers in cloud environments. Our work includes runtime security enforcement systems and security enhanced container network interfaces.

### Focus Areas

**Policy synthesis and enforcement**: automatic derivation of least-privilege network and system policies from workload intent, provenance, and runtime context; inline enforcement via eBPF/SmartNICs.

**Zero-trust networked systems**: micro-segmentation and per-workload identity, with continuous attestation of endpoints and data paths.

**Efficient telemetry**: programmable, low-overhead collection and aggregation that preserves fidelity for forensics while bounding resource usage.

---

## 3. AI-Assisted Networked Systems

We leverage AI—especially large language models (LLMs)—to synthesize, optimize, and validate network functions and configurations, turning expert workflows into repeatable toolchains.

### Focus Areas

**NF synthesis and composition**: generating match-action pipelines and stateful NFs from formalized intent; compiling to safe eBPF/XDP or P4-like targets under verifier/hardware constraints.

**Autotuning and design-space exploration**: LLM-orchestrated search over protocol parameters, queueing policies, and offload placements with closed-loop measurement.

**Configuration and policy generation**: translating topology, SLOs, and traffic descriptions into deployable configurations and policy bundles (e.g., ACLs, routing, rate limits).


