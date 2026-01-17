# Proposed Charter for Next-Generation Inter-Domain Routing Architecture and Protocols Research Group (IDRNG)

The Next-Generation Inter-Domain Routing Architecture and Protocols Research Group (IDRNG) investigates architecture, protocol, manageability, and operational questions for inter-domain routing in the AI era.

The group focuses on networking across heterogeneous administrative domains (ASes, operators, cloud/edge providers, IXPs, overlays), where connectivity and policy reflect diverse business objectives, security postures, compute availability, and regulatory constraints. These environments increasingly couple control-plane logic with programmable data planes and distributed compute fabrics supporting AI workloads.

Modern inter-domain routing exhibits challenges not captured by classical BGP-centric assumptions, including:

1. Policy & Trust Heterogeneity: Divergent intents, policies, and compliance regimes with limited means to express and verify end-to-end correctness.
2. Security & Assurance Gaps: Susceptibility to leaks, hijacks, and misconfigurations; insufficient binding between forwarding intent, control-plane state, and data-plane behavior.
3. Scale & Dynamics: Large route tables, anycast/multi-homing, bursty traffic, and rapid operational changes stressing convergence and stability.
4. Compute-Network Co-Scheduling: AI workloads require routing that accounts for accelerator availability, data locality, energy/carbon constraints, and latency/jitter SLOs.
5. Observability vs. Privacy: Need for high-fidelity telemetry and attestations while protecting sensitive policy or private data.

Based on these observations, topics of interest for the IDRNG include:

1. Inter-Domain Forwarding-Intent Security & Assurance: Techniques to define, exchange, and cryptographically bind forwarding intent to control-plane announcements and data-plane behavior; runtime attestation; formal models and cross-domain evidence loops.
2. AI-Native Routing: Architectures that incorporate ML/AI into control and safe, minimal data-plane functions; distributed/federated learning, RL-based routing, safety guardrails, convergence/stability analyses, and operator-oriented explainability.
3. AI for Routing: Data-driven methods improving today's routing-anomaly/leak/hijack detection, convergence prediction, configuration synthesis/validation, causal incident analysis, and robust datasets for reproducible evaluation.
4. Routing for AI: Treating AI training/inference as first-class traffic; information models for advertising/consuming compute and data attributes, enabling routing/TE that satisfies stricter latency/burst SLOs and respects privacy/compliance.
5. Multi-Agent Routing / Agentic Internet: Models and mechanisms for coordination/competition among autonomous agents (operators, tenants, applications, AI agents); negotiation, incentive-compatible designs, reputation, accountability, and human-in-the-loop explainability.
6. In-Band Intelligent Data Plane: Use of in-band telemetry and lightweight, safe programmable data-plane processing to generate verifiable evidence of SLA/intent adherence; support real-time, in-band anomaly and policy-violation detection; and enable tight integration with control-plane mechanisms for closed-loop reaction, mitigation, and optimization, while analyzing privacy, overhead, and interoperability trade-offs.

IDRNG will coordinate with adjacent industry and research communities (e.g., cloud/CDN consortia, programmable-network and telemetry ecosystems, operator/security communities, SIGCOMM/IMC/NDSS/CCS venues) and with IRTF/IETF groups (NMRG, COINRG, PANRG, IDR, SIDROPS, GROW, RTGWG). It will leverage existing route collectors, telemetry platforms, and testbeds to avoid duplication and promote reusable artifacts.

Initial goals include:

1. Engage with network operators, researchers, vendors, and standards bodies to explore new architectural concepts, AI-driven control strategies, and secure and verifiable control-plane and data-plane designs for inter-domain routing. This includes maintaining a coherent architectural framework and threat model for next-generation inter-domain routing, covering trust anchors, forwarding intent, and intent-to-compute binding, with the aim of generating research papers and Informational RFCs.
2. Develop evaluation methodologies for next-generation inter-domain routing, including metrics, representative topologies, policy models, and attack and fault models, as well as the collection and analysis of measurements on ROA/ROV dynamics, routing anomalies, and data-plane signals to empirically characterize current practice, with the aim of generating research papers and Informational RFCs.
3. Define reference scenarios and best practices for emulations and field trials, including forwarding-intent verification, multi-operator environments, and privacy-preserving mechanisms, with the aim of producing Informational RFCs or BCP RFCs.
4. Document and promote shared testbeds and infrastructure for next-generation inter-domain routing, including interoperability testing of candidate approaches, transition and deployment guidance, and cross-domain experiment coordination, with the aim of producing Experimental RFCs.
5. Document the outcomes of the above efforts through datasets, research papers, and RFCs (including BCP, Informational, and Experimental documents) as input to future IRTF and IETF work on inter-domain routing.
