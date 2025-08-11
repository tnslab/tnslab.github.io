---
title: "TNSLab - Research"
layout: textlay
excerpt: "TNSLab -- Research"
sitemap: false
permalink: /research/
---

# Research Areas

---

## 1. Cloud Networking

We investigate the design and optimization of cloud network data planes that enable containers and virtual machines to exchange data with high efficiency and low latency. Our research combines workload-aware software network stacks with selective hardware acceleration, aiming to maximize throughput while minimizing CPU utilization and operational overhead.

### Focus Areas

**Workload-aware network stack**: Leveraging advanced kernel-bypass techniques such as eBPF/XDP and DPDK to develop network stacks tailored to specific workload characteristics; incorporating specialized network functions (e.g., congestion control, flow scheduling) optimized for performance and resource efficiency.

**Hardware-accelerated networking**: Offloading compute-intensive network functions (e.g., TLS/QUIC handshakes, DPI, telemetry aggregation) to programmable hardware devices such as SmartNICs and FPGAs; building high-performance, scalable data planes for diverse cloud workloads.

---

## 2. Cloud Security

We design and implement practical security systems for cloud environments, capable of identifying and mitigating attack vectors across nodes, virtual machines, and containers. Our work emphasizes runtime enforcement and hardware-based isolation to ensure robust protection against sophisticated threats.

### Focus Areas

**Runtime security enforcement**: Automatically deriving least-privilege network and system policies from workload intent, provenance, and runtime context; enforcing these policies inline through mechanisms such as eBPF and SmartNIC-based processing.

**Hardware-isolated secyruty enforcement**: Migrating critical security functions from untrusted host CPUs to trusted hardware components such as DPUs and TEEs; ensuring policy enforcement integrity and performance even under potential host compromise.

---

## 3. AI-Assisted Networked Systems

We leverage AI (e.g., LLMs) to synthesize, optimize, and validate network functions and configurations in runtime.

### Focus Areas

**Network function generation**: Automatically generating match-action pipelines and stateful network functions for programmable hardware targets from high-level, natural language specifications.

**Configuration and policy generation**: Translating network topology, service-level objectives, and traffic requirements into deployable configurations and policy bundles (e.g., ACLs and routing rules), enabling rapid and error-resistant provisioning of networked systems.