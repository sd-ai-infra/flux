# Software-Defined Controller for AI Infrastructure (sd-ai-infra)

High-performance AI clusters demand a network control plane that is dynamic, deterministic, and workload-aware. **sd-ai-infra** is an open-source initiative dedicated to designing, prototyping, and standardizing software-defined networking controllers tailored for large-scale AI/ML fabrics.

---

## 🎯 Mission

Traditional data center networking models are built for generic east-west traffic. AI/ML workloads introduce extreme, bursty, synchronized all-to-all communication patterns (AllReduce, AlltoAll) that trigger congestion, tail-latency spikes, and fabric collapse.

Our mission is to build an open, programmable control and orchestration layer that bridges collective communication libraries directly to underlying network fabrics.

---

## 🔬 Core Focus Areas

- **Workload-Aware Traffic Engineering:** Dynamically steering collective communication flows (NCCL, RCCL) based on phase and topology.
- **Fabric Optimization & Congestion Control:** Low-latency, deterministic multi-pathing and queue management across loss-sensitive RoCEv2, Ultra Ethernet (UEC), and InfiniBand clusters.
- **Programmable Fabric Control:** Decoupled control planes leveraging P4, eBPF, and open APIs to orchestrate telemetry, path validation, and hardware-accelerated telemetry.
- **Topology & Failure Resilience:** Fast, sub-millisecond route convergence, link degradation detection, and automated fabric rebalancing without stalling active training jobs.

---

## 🛠 Active Workstreams

| Workstream | Scope |
| :--- | :--- |
| **Architecture & Specs** | System blueprints, RFCs, and API contract specifications |
| **Controller Core** | Centralized SDN controller logic, state stores, and southbound agents |
| **Fabric Telemetry** | Real-time buffer utilization, PFC/ECN monitors, and microburst tracking |
| **Simulations & Testbeds** | Emulation environments (Mininet/containerlab) and hardware lab validation |

---

## 🤝 Getting Involved

We are actively seeking system architects, networking engineers, distributed systems researchers, and kernel/firmware developers.

- **Explore RFCs & Specs:** Check our pinned repositories to review work-in-progress architecture proposals.
- **Start a Discussion:** Use the [GitHub Discussions](https://github.com/orgs/sd-ai-infra/discussions) tab to propose ideas, share telemetry findings, or debate design decisions.
- **Contribute:** Pick up an open issue labeled `good first issue` or `rfc-discussion`.

---

## 📜 Governance & Standards

All repositories under `sd-ai-infra` adhere to open-source governance principles. Code contributions are governed by the Apache 2.0 License unless specified otherwise.
