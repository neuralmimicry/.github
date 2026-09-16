<div align="center">

# NeuralMimicry

**Open-source neuromorphic AI · AI governance · Governed delivery · Sovereign operations · Adaptive resilience**

*UK independent platform engineering — Rugby, Warwickshire*

[![Website](https://img.shields.io/badge/Website-neuralmimicry.ai-1B2833?style=for-the-badge)](https://neuralmimicry.ai)
[![Crowdfunder](https://img.shields.io/badge/☕%20Support%20Us-Crowdfunder-E35528?style=for-the-badge)](https://www.crowdfunder.co.uk/p/qr/aWggxwPW?utm_campaign=sharemodal&utm_medium=referral&utm_source=shortlink)
[![Contact](https://img.shields.io/badge/Contact-info@neuralmimicry.ai-1B2833?style=for-the-badge&logo=gmail)](mailto:info@neuralmimicry.ai)

---

### ☕ [Support NeuralMimicry on Crowdfunder](https://www.crowdfunder.co.uk/p/qr/aWggxwPW?utm_campaign=sharemodal&utm_medium=referral&utm_source=shortlink)

*We are an independent open-source initiative. Community backing sustains the research, infrastructure, and development that keeps every product moving forwards.*

</div>

---

## What We Build

NeuralMimicry develops a suite of open-source tools for teams that need AI to be **governed, inspectable, and sovereign** — not another black-box service dependency. The platform spans five capability areas:

| Route | Lead product | What it does |
|---|---|---|
| **AI governance** | [Aria](https://github.com/neuralmimicry/aria) with [Gail](https://github.com/neuralmimicry/gail) | Request and response risk assessment, operator oversight, alerts and policy enforcement on configured AI traffic |
| **Governed delivery** | [Refiner](https://github.com/neuralmimicry/rag_demo) | LLM workflow engine, RAG, agentic delivery pipelines, Jira/Confluence analysis, project solver |
| **Sovereign operations** | [Continuum — NMC](https://github.com/neuralmimicry/nmc) | Kubernetes, vcluster, VM, node recruitment, Tracey fleet control |
| **Adaptive resilience** | [Tracey](https://github.com/neuralmimicry/tracey) | Swarm security runtime, fuzzy inference scoring, multi-agent governance |
| **Neuromorphic intelligence** | [AARNN](https://github.com/neuralmimicry/aarnn) · [aarnn\_rust](https://github.com/neuralmimicry/aarnn_rust) | Biologically-inspired AI with continuous learning and morphological adaptation |

Every product is **open source**. Inspect the architecture, raise issues, and build confidence before any commercial engagement.

---

## AI Governance with Aria

**Aria — Automated Regulation & Integrity Arbiter** governs AI requests and responses passing through **Gail**, NeuralMimicry’s shared gateway to AI providers and libraries. It helps teams identify concerning content, review incidents and apply policy at the point of use.

### How it works

1. **Assess the request.** Gail sends configured traffic to Aria before the original model call. Rules and contextual AI assessment look for risks such as instruction overrides, exposed credentials, destructive commands and harmful instructions.
2. **Apply policy.** Aria returns an **allow**, **alert** or **block** decision. In enforcement mode, Gail stops blocked requests before model execution.
3. **Assess the response.** Gail submits the output for assessment before release and withholds blocked responses in enforcement mode.
4. **Keep an operational record.** Decisions, policy revisions and operator actions remain available for review. Signed webhook alerts and Prometheus metrics connect governance to operational monitoring.

Aria’s AI assessment uses **Gail’s existing configured providers**. A restricted assessment route prevents recursive checks; a versioned HTTP contract keeps the services separate without either project importing the other.

The **operator dashboard** supports incident review and acknowledgement, threshold changes, source blocking and pauses on governed traffic. Authorised viewers and operators can inspect Gail’s actual governance mode and outage behaviour, with product navigation connecting Aria to the wider NeuralMimicry estate.

**Start with monitoring, then enable enforcement.** Monitoring records concerns without applying content blocks or pauses. Enforcement applies those controls; configurable fail-closed behaviour can stop affected traffic when assessment is unavailable. Pauses take effect at evaluation boundaries and do not undo completed actions.

Coverage depends on configured Gail routes. Streamed responses are buffered within limits before assessment and release; opaque media may be marked uninspectable. Aria retains content hashes and structured findings rather than raw prompts and responses, while assessment still processes content through Gail’s providers. It identifies risk without establishing malicious intent or guaranteeing detection, and does not certify regulatory compliance.

**Explore:** [Aria repository and setup](https://github.com/neuralmimicry/aria) · [Operational guidance](https://github.com/neuralmimicry/aria/blob/main/docs/operations.md) · [Gail integration](https://github.com/neuralmimicry/gail/blob/main/docs/aria.md) · [Discuss your use case](https://neuralmimicry.ai/contact)

---

## Open-Source Repositories

### Core Platform

| Repository | Language | Description |
|---|---|---|
| [**rag\_demo**](https://github.com/neuralmimicry/rag_demo) — Refiner | Python | LLM workflow engine and public API gateway: RAG, MCP, agentic delivery, Jira/Confluence analysis, multi-provider AI orchestration |
| [**gail**](https://github.com/neuralmimicry/gail) | Rust | Shared AI middleware: multi-provider LLM routing, neuromorphic access, AER translation, continuous fine-tuning, autonomous trading bridge; integrates Aria checks on configured AI request and response paths |
| [**aria**](https://github.com/neuralmimicry/aria) | Rust | AI governance through Gail: rules and contextual assessment, policy controls, incident dashboard, audit records and alerts |
| [**conductor**](https://github.com/neuralmimicry/conductor) | Rust | Estate control-plane: topology discovery, evidence-backed findings, governed work-item queue, staged delivery pipeline |
| [**nmc**](https://github.com/neuralmimicry/nmc) | C++ | Kubernetes/vcluster operator CLI and HTTP control plane with Tracey fleet management and provider portal orchestration |
| [**tracey**](https://github.com/neuralmimicry/tracey) | Rust | Swarm anomaly/security runtime: fuzzy scoring, multi-agent consensus, TraceyGuard/TraceyBan, fleet telemetry |

### Identity, Billing & Audit

| Repository | Language | Description |
|---|---|---|
| [**customers**](https://github.com/neuralmimicry/customers) | Python | Identity service: registration, auth, 2FA, passkeys, SSO, OIDC, and delegated group management |
| [**billing**](https://github.com/neuralmimicry/billing) | Python | Token accounting, payment capture, and auditable ledger service |
| [**nmchain**](https://github.com/neuralmimicry/nmchain) | Rust | Private permissioned blockchain: tamper-evident audit ledger for identity, payment, and token events |

### Neuromorphic AI

| Repository | Language | Description |
|---|---|---|
| [**aarnn**](https://github.com/neuralmimicry/aarnn) | C++ | Autonomic Asynchronous Recursive Neuromorphic Network — oscillatory networks, PostgreSQL persistence, VTK visualisation |
| [**aarnn\_rust**](https://github.com/neuralmimicry/aarnn_rust) | Rust | Full neuromorphic autonomous AI platform: GPU kernels, Kubernetes operator, training pipelines, embodied simulation |
| [**neuromorphic\_demo**](https://github.com/neuralmimicry/neuromorphic_demo) | Rust | Interactive SNN demo: live inputs, dynamic 3D growth, morphology-inspired AARNN dynamics |
| [**aarnn-nsys**](https://github.com/neuralmimicry/aarnn-nsys) | Rust | Ultra-low-latency zero-allocation pub/sub message bus for neuromorphic and real-time systems, incl. bare-metal `no_std` |
| [**feel-bridge**](https://github.com/neuralmimicry/feel-bridge) | Verilog | Hybrid analog–analog reservoir computing: GPU firmware physics and memristive neuron dynamics on FPGA |

### Speech, Deployment & Infrastructure

| Repository | Language | Description |
|---|---|---|
| [**nmstt**](https://github.com/neuralmimicry/nmstt) | Rust | On-premises speech-to-text (Whisper-based): privacy-first, ARM64-native, gesture and avatar-motion planning |
| [**aarnn-network**](https://github.com/neuralmimicry/aarnn-network) | HCL | Infrastructure-as-Code for building and deploying containerised AARNN and Aeron workloads |
| [**raspi-bare-metal**](https://github.com/neuralmimicry/raspi-bare-metal) | Rust | Bare-metal AArch64 demo of aarnn-nsys on Raspberry Pi 4 — no OS, no allocator |
| [**oshift**](https://github.com/neuralmimicry/oshift) | HCL | Zero Touch Provisioning pipeline for AI/HPC workloads on Red Hat OpenShift |
| [**jirastats**](https://github.com/neuralmimicry/jirastats) | Python | Lightweight Jira reporting toolkit: discovery-driven JQL refinement, throughput analysis, LLM-backed insights |

---

## Direct Technical Support

**Paul Isaac's** — Founder & CTO

> MSc (Distinction) Intelligent Systems & Robotics · 20+ years software engineering · 15+ years AI including neuromorphic systems, robotics, and distributed platforms · TEDx speaker · PhD research in cognitive AI and type-n security

Paul is available for direct, hands-on technical support across the full platform — implementation, architecture review, integration guidance, and advanced troubleshooting.

**£1,000 per day + VAT** — on-site (UK) or remote · minimum one day

Covers Refiner, Gail, Aria, Continuum, Tracey, AARNN, and the full open-source deployment stack.

**→ [Enquire: info@neuralmimicry.ai](mailto:info@neuralmimicry.ai?subject=Direct%20Technical%20Support%20Enquiry)**

For broader engagements — architecture sessions, product briefings, and controlled pilots — see [neuralmimicry.ai/contact](https://neuralmimicry.ai/contact).

---

## Support the Project

NeuralMimicry is an independent open-source initiative. Every product is free to use, inspect, and contribute to. Research, infrastructure, and ongoing development depend on community backing.

<div align="center">

### **[☕ Support us on Crowdfunder](https://www.crowdfunder.co.uk/p/qr/aWggxwPW?utm_campaign=sharemodal&utm_medium=referral&utm_source=shortlink)**

</div>

---

<div align="center">

[neuralmimicry.ai](https://neuralmimicry.ai) &nbsp;·&nbsp; [Solutions](https://neuralmimicry.ai/solutions) &nbsp;·&nbsp; [About](https://neuralmimicry.ai/about) &nbsp;·&nbsp; [Contact](https://neuralmimicry.ai/contact) &nbsp;·&nbsp; [GitHub](https://github.com/neuralmimicry)

*NeuralMimicry Ltd · Registered in England and Wales · Rugby, Warwickshire*

</div>
