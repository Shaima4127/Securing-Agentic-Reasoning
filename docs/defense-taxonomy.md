<!-- Generated from the project's annotation workbooks. Do not edit by hand. -->

# Defense taxonomy (D1–D3)

37 defense papers from the annotated empirical corpus, grouped into three clusters by where the defense acts: at the input/output boundary, during agent execution, or on the reasoning process itself.

## Clusters

| Cluster | Name | Sub-clusters | Papers |
|---|---|---|---|
| 🟧 ![D1](https://img.shields.io/badge/D1-FC8D62?style=flat-square) | Boundary Filtering and Guardrails | 3 | 12 |
| 🟩 ![D2](https://img.shields.io/badge/D2-7DBD54?style=flat-square) | Runtime Agent Monitoring and Execution Control | 2 | 12 |
| 🟦 ![D3](https://img.shields.io/badge/D3-6BAED6?style=flat-square) | Reasoning-Aware Process Defenses | 2 | 13 |

## Agentic scope (G5) by cluster

| Cluster | G5 = ADDRESSED |
|---|---|
| 🟧 D1 | 4 of 12 |
| 🟩 D2 | 12 of 12 |
| 🟦 D3 | 9 of 13 |

## Gap flag distributions

| Gap | ● Addressed | ◐ Partial | ○ Present |
|---|---|---|---|
| **G1** Reasoning Observability | 11 | 0 | 26 |
| **G2** Reasoning Integrity Metric | 11 | 0 | 26 |
| **G3 (D)** Defense Capability | 12 | 2 | 23 |
| **G4 (D)** Adaptivity | 12 | 12 | 13 |
| **G5** Agentic Scope | 25 | 0 | 12 |

`PARTIAL` is admissible only in G3 (D) and G4 (D); it is not a valid value for G1, G2, or G5.

## Per-paper annotations

● addressed  ·  ◐ partially addressed  ·  ○ present  ·  – not applicable

| Paper | Cluster | Sub-cluster | Pattern | Structure | Reasoning-aware | ARE | AA | Scope | G1 | G2 | G3(D) | G4(D) | G5 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [JailGuard](https://doi.org/10.1145/3724393) | 🟧 D1 | Content Filtering and Sanitization | Input sanitization, Output verification | Static | No | Partial | No | LLM only | ○ | ○ | ○ | ◐ | ○ |
| [BadChain](https://arxiv.org/abs/2401.12242) | 🟧 D1 | Content Filtering and Sanitization | Input sanitization | Static | No | No | No | LLM only | ● | ● | ◐ | ○ | ○ |
| [X-Teaming](https://arxiv.org/abs/2504.13203) | 🟧 D1 | Adversarial Training and Alignment | Adversarial training | Static | No | Yes | Yes | LLM only | ○ | ○ | ○ | ● | ○ |
| [ActorBreaker](https://doi.org/10.18653/v1/2025.acl-long.1207) | 🟧 D1 | Adversarial Training and Alignment | Adversarial training | Static | No | Partial | Yes | LLM only | ○ | ○ | ○ | ◐ | ○ |
| [PIGuard](https://doi.org/10.18653/v1/2025.acl-long.1468) | 🟧 D1 | Guardrail Classifiers | Guardrail | Static | No | Partial | No | LLM only | ○ | ○ | ○ | ◐ | ○ |
| [PISanitizer](https://arxiv.org/abs/2511.10720) | 🟧 D1 | Content Filtering and Sanitization | Input sanitization | Adaptive | No | Yes | No | Agent | ○ | ○ | ○ | ● | ● |
| StruQ | 🟧 D1 | Content Filtering and Sanitization | Input sanitization | Static | No | Yes | Yes | LLM only | ○ | ○ | ○ | ● | ○ |
| [Instruction Hierarchy](https://arxiv.org/abs/2404.13208) | 🟧 D1 | Adversarial Training and Alignment | Adversarial training | Static | No | Partial | No | LLM only | ○ | ○ | ○ | ◐ | ○ |
| [PromptArmor](https://arxiv.org/abs/2507.15219) | 🟧 D1 | Guardrail Classifiers | Guardrail | Mixed | No | Yes | Yes | Agent | ○ | ○ | ○ | ● | ● |
| SecAlign | 🟧 D1 | Adversarial Training and Alignment | Adversarial training | Static | No | Yes | Yes | Mixed | ○ | ○ | ○ | ● | ● |
| [Tool Result Parsing](https://arxiv.org/abs/2601.04795) | 🟧 D1 | Content Filtering and Sanitization | Input sanitization | Static | No | No | No | Agent | ○ | ○ | ○ | ○ | ● |
| [PromptShield](https://doi.org/10.1145/3714393.3726501) | 🟧 D1 | Guardrail Classifiers | Guardrail | Static | No | No | No | LLM only | ○ | ○ | ○ | ○ | ○ |
| [AgentMonitor](https://arxiv.org/abs/2408.14972) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring | Static | No | No | No | Multi-agent | ○ | ○ | ○ | ○ | ● |
| [RTBAS](https://arxiv.org/abs/2502.08966) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring | Static | No | Partial | No | Agent | ○ | ○ | ○ | ◐ | ● |
| [SafeAgent](https://arxiv.org/abs/2604.17562) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring, Sandboxing | Adaptive | No | No | No | Agent | ○ | ○ | ○ | ○ | ● |
| [AgentArmor](https://arxiv.org/abs/2508.01249) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring | Static | No | No | No | Agent | ○ | ○ | ○ | ○ | ● |
| [Unsafer in Many Turns](https://arxiv.org/abs/2602.13379) | 🟩 D2 | Runtime Monitoring and Guardrails | Sandboxing, Runtime monitoring | Static | No | Partial | No | Agent | ○ | ○ | ○ | ◐ | ● |
| [ProbGuard](https://arxiv.org/abs/2508.00500) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring | Static | No | No | No | Agent | ○ | ○ | ○ | ○ | ● |
| [GuardAgent](https://arxiv.org/abs/2406.09187) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring, Guardrail | Mixed | No | No | No | Agent | ○ | ○ | ○ | ○ | ● |
| [CaMeL](https://arxiv.org/abs/2503.18813) | 🟩 D2 | Execution Isolation and Sandboxing | Sandboxing, Runtime monitoring | Static | No | Partial | No | Agent | ○ | ○ | ○ | ◐ | ● |
| [AGrail](https://doi.org/10.18653/v1/2025.acl-long.399) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring | Adaptive | No | Partial | No | Agent | ○ | ○ | ○ | ◐ | ● |
| [AgentSentinel](https://doi.org/10.1145/3719027.3765064) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring | Mixed | No | Yes | No | Agent | ○ | ○ | ○ | ● | ● |
| [IsolateGPT](https://doi.org/10.14722/ndss.2025.241131) | 🟩 D2 | Execution Isolation and Sandboxing | Sandboxing | Static | No | Partial | No | Agent | ○ | ○ | ○ | ◐ | ● |
| [AgentVisor](https://arxiv.org/abs/2604.24118) | 🟩 D2 | Runtime Monitoring and Guardrails | Runtime monitoring, Sandboxing | Static | No | Yes | Yes | Agent | ○ | ○ | ○ | ● | ● |
| [AgentDoG](https://arxiv.org/abs/2601.18491) | 🟦 D3 | Reasoning-Trace Monitoring | Guardrail, Runtime monitoring | Static | Yes | Partial | No | Agent | ● | ● | ● | ◐ | ● |
| [STAC](https://arxiv.org/abs/2509.25624) | 🟦 D3 | Reasoning Repair and Consistency | Reasoning consistency check | Static | Partial | Yes | Yes | Agent | ○ | ○ | ◐ | ● | ● |
| [Reasoning-Style Poisoning](https://arxiv.org/abs/2512.14448) | 🟦 D3 | Reasoning-Trace Monitoring | Runtime monitoring | Static | Yes | No | No | Agent | ● | ● | ● | ○ | ● |
| [Monitoring Reasoning Models](https://arxiv.org/abs/2503.11926) | 🟦 D3 | Reasoning Repair and Consistency | Runtime monitoring, Reasoning consistency check | Mixed | Yes | Yes | Yes | Agent | ● | ● | ● | ● | ● |
| [Thought Purity](https://arxiv.org/abs/2507.12314) | 🟦 D3 | Reasoning Repair and Consistency | Reasoning consistency check | Adaptive | Yes | No | No | LLM only | ● | ● | ● | ○ | ○ |
| [Unreal Thinking](https://arxiv.org/abs/2604.09235) | 🟦 D3 | Reasoning Repair and Consistency | Reasoning consistency check | Static | Yes | No | No | LLM only | ● | ● | ● | ○ | ○ |
| [CoT Obfuscation](https://arxiv.org/abs/2510.19851) | 🟦 D3 | Reasoning-Trace Monitoring | Runtime monitoring | Static | Yes | Yes | No | Agent | ● | ● | ● | ● | ● |
| [When CoT Is Necessary](https://arxiv.org/abs/2507.05246) | 🟦 D3 | Reasoning-Trace Monitoring | Runtime monitoring | Static | Yes | Yes | No | LLM only | ● | ● | ● | ● | ○ |
| [Covertly Sandbag](https://doi.org/10.18653/v1/2025.ijcnlp-short.33) | 🟦 D3 | Reasoning-Trace Monitoring | Runtime monitoring | Static | Yes | Yes | No | LLM only | ● | ● | ● | ● | ○ |
| IntentGuard | 🟦 D3 | Reasoning Repair and Consistency | Runtime monitoring, Reasoning consistency check, Guardrail | Static | Yes | Partial | No | Agent | ● | ● | ● | ◐ | ● |
| [Psg-Agent](https://arxiv.org/abs/2509.23614) | 🟦 D3 | Reasoning-Trace Monitoring | Runtime monitoring | Mixed | Yes | No | No | Agent | ○ | ○ | ● | ○ | ● |
| [TrustAgent](https://doi.org/10.18653/v1/2024.findings-emnlp.585) | 🟦 D3 | Reasoning Repair and Consistency | Reasoning consistency check | Mixed | Yes | No | No | Agent | ○ | ○ | ● | ○ | ● |
| [ICON](https://arxiv.org/abs/2602.20708) | 🟦 D3 | Reasoning Repair and Consistency | Reasoning consistency check | Adaptive | Yes | Partial | No | Agent | ● | ● | ● | ◐ | ● |

## Papers by sub-cluster

### 🟧 D1 — Boundary Filtering and Guardrails

**Content Filtering and Sanitization** (5)

- **JailGuard** — [JailGuard: A Universal Detection Framework for Prompt-based Attacks on LLM Systems](https://doi.org/10.1145/3724393)  
  *Zhang et al. · 2025*
- **BadChain** — [BADCHAIN: BACKDOOR CHAIN-OF-THOUGHT PROMPTING FOR LARGE LANGUAGE MODELS](https://arxiv.org/abs/2401.12242)  
  *Xiang et al. · 2024*
- **PISanitizer** — [PISanitizer: Preventing Prompt Injection to Long-Context LLMs via Prompt Sanitization](https://arxiv.org/abs/2511.10720)  
  *Geng et al. · 2025*
- **StruQ** — StruQ: Defending Against Prompt Injection with Structured Queries  
  *Chen et al. · 2025*
- **Tool Result Parsing** — [Defense Against Indirect Prompt Injection via Tool Result Parsing](https://arxiv.org/abs/2601.04795)  
  *Yu et al. · 2026*

**Adversarial Training and Alignment** (4)

- **X-Teaming** — [X-Teaming: Multi-Turn Jailbreaks and Defenses with Adaptive Multi-Agents](https://arxiv.org/abs/2504.13203)  
  *Rahman et al. · 2025*
- **ActorBreaker** — [LLMs know their vulnerabilities: Uncover Safety Gaps through Natural Distribution Shifts](https://doi.org/10.18653/v1/2025.acl-long.1207)  
  *Ren et al. · 2025*
- **Instruction Hierarchy** — [The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions](https://arxiv.org/abs/2404.13208)  
  *Wallace et al. · 2025*
- **SecAlign** — SecAlign: Defending Against Prompt Injection with Preference Optimization  
  *Chen et al. · 2025*

**Guardrail Classifiers** (3)

- **PIGuard** — [PIGuard: Prompt Injection Guardrail via Mitigating Overdefense for Free](https://doi.org/10.18653/v1/2025.acl-long.1468)  
  *Li et al. · 2025*
- **PromptArmor** — [PromptArmor: Simple yet Effective Prompt Injection Defenses](https://arxiv.org/abs/2507.15219)  
  *Shi et al. · 2025*
- **PromptShield** — [PromptShield: Deployable Detection for Prompt Injection Attacks](https://doi.org/10.1145/3714393.3726501)  
  *Jacob et al. · 2025*

### 🟩 D2 — Runtime Agent Monitoring and Execution Control

**Runtime Monitoring and Guardrails** (10)

- **AgentMonitor** — [AGENTMONITOR: A PLUG-AND-PLAY FRAMEWORK FOR PREDICTIVE AND SECURE MULTI-AGENT SYSTEMS](https://arxiv.org/abs/2408.14972)  
  *Chan et al. · 2024*
- **RTBAS** — [RTBAS: Defending LLM Agents Against Prompt Injection and Privacy Leakage](https://arxiv.org/abs/2502.08966)  
  *Zhong et al. · 2025*
- **SafeAgent** — [SafeAgent: A Runtime Protection Architecture for Agentic Systems](https://arxiv.org/abs/2604.17562)  
  *Liu et al. · 2026*
- **AgentArmor** — [Securing Large Language Model Agents via Structured Graph Abstraction AgentArmor: Enforcing Program Analysis on Agent Runtime Trace to Defend Against Prompt Injection](https://arxiv.org/abs/2508.01249)  
  *Wang et al. · 2025*
- **Unsafer in Many Turns** — [Unsafer in Many Turns: Benchmarking and Defending Multi-Turn Safety Risks in Tool-Using Agents](https://arxiv.org/abs/2602.13379)  
  *Li et al. · 2026*
- **ProbGuard** — [ProbGuard: Probabilistic Runtime Monitoring for LLM Agent Safety](https://arxiv.org/abs/2508.00500)  
  *Wang et al. · 2026*
- **GuardAgent** — [GuardAgent: Safeguard LLM Agents via Knowledge-Enabled Reasoning](https://arxiv.org/abs/2406.09187)  
  *Xiang et al. · 2025*
- **AGrail** — [AGrail: A Lifelong Agent Guardrail with Effective and Adaptive Safety Detection](https://doi.org/10.18653/v1/2025.acl-long.399)  
  *Luo et al. · 2025*
- **AgentSentinel** — [AgentSentinel: An End-to-End and Real-Time Security Defense Framework for Computer-Use Agents](https://doi.org/10.1145/3719027.3765064)  
  *Hu et al. · 2025*
- **AgentVisor** — [AgentVisor: Defending LLM Agents Against Prompt Injection via Semantic Virtualization](https://arxiv.org/abs/2604.24118)  
  *Ying et al. · 2026*

**Execution Isolation and Sandboxing** (2)

- **CaMeL** — [Defeating Prompt Injections by Design / CaMeL](https://arxiv.org/abs/2503.18813)  
  *Debenedetti et al. · 2025*
- **IsolateGPT** — [IsolateGPT: An Execution Isolation Architecture for LLM-Based Agentic Systems](https://doi.org/10.14722/ndss.2025.241131)  
  *Wu et al. · 2025*

### 🟦 D3 — Reasoning-Aware Process Defenses

**Reasoning-Trace Monitoring** (6)

- **AgentDoG** — [AgentDoG: A Diagnostic Guardrail Framework for AI Agent Safety and Security](https://arxiv.org/abs/2601.18491)  
  *Liu et al. · 2026*
- **Reasoning-Style Poisoning** — [Reasoning-Style Poisoning of LLM Agents via Stealthy Style Transfer: Process-Level Attacks and Runtime Monitoring in RSV Space](https://arxiv.org/abs/2512.14448)  
  *Zhou and Wang · 2026*
- **CoT Obfuscation** — [CAN REASONING MODELS OBFUSCATE REASONING? STRESS-TESTING CHAIN-OF-THOUGHT MONITORABILITY](https://arxiv.org/abs/2510.19851)  
  *Zolkowski et al. · 2025*
- **When CoT Is Necessary** — [When Chain of Thought is Necessary, Language Models Struggle to Evade Monitors](https://arxiv.org/abs/2507.05246)  
  *Emmons et al. · 2025*
- **Covertly Sandbag** — [LLMs Can Covertly Sandbag on Capability Evaluations Against Chain-of-Thought Monitoring](https://doi.org/10.18653/v1/2025.ijcnlp-short.33)  
  *Li et al. · 2025*
- **Psg-Agent** — [PSG-AGENT: PERSONALITY-AWARE SAFETY GUARDRAIL FOR LLM-BASED AGENTS](https://arxiv.org/abs/2509.23614)  
  *Wu et al. · 2025*

**Reasoning Repair and Consistency** (7)

- **STAC** — [STAC: WHEN INNOCENT TOOLS FORM DANGEROUS CHAINS TO JAILBREAK LLM AGENTS](https://arxiv.org/abs/2509.25624)  
  *Li et al. · 2026*
- **Monitoring Reasoning Models** — [Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation](https://arxiv.org/abs/2503.11926)  
  *Baker et al. · 2025*
- **Thought Purity** — [Thought Purity: A Defense Framework For Chain-of-Thought Attack](https://arxiv.org/abs/2507.12314)  
  *Xue et al. · 2026*
- **Unreal Thinking** — [Unreal Thinking: Chain-of-Thought Hijacking via Two-stage Backdoor](https://arxiv.org/abs/2604.09235)  
  *Chang et al. · 2026*
- **IntentGuard** — IntentGuard: Safeguard LLM Agents via Intent Alignment  
  *Cong et al. · 2026*
- **TrustAgent** — [TrustAgent: Towards Safe and Trustworthy LLM-based Agents](https://doi.org/10.18653/v1/2024.findings-emnlp.585)  
  *Hua et al. · 2024*
- **ICON** — [ICON: Indirect Prompt Injection Defense for Agents based on Inference-Time Correction](https://arxiv.org/abs/2602.20708)  
  *Wang et al. · 2026*
