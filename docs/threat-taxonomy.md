<!-- Generated from the project's annotation workbooks. Do not edit by hand. -->

# Threat taxonomy (T1–T4)

31 threat papers from the annotated empirical corpus, grouped into four clusters. Clusters are assigned on the basis of four annotation dimensions — attack vector, attack pattern, attack target, and attack structure — recorded per paper in the table below.

## Clusters

| Cluster | Name | Attack classes | Papers |
|---|---|---|---|
| 🟦 ![T1](https://img.shields.io/badge/T1-0173B2?style=flat-square) | Reasoning Manipulation and Backdoors | 3 | 9 |
| 🟧 ![T2](https://img.shields.io/badge/T2-DE8F05?style=flat-square) | Indirect Prompt Injection and Tool-Chain Attacks | 3 | 10 |
| 🟩 ![T3](https://img.shields.io/badge/T3-66C2A5?style=flat-square) | Adaptive and Multi-turn Attacks | 3 | 7 |
| 🟪 ![T4](https://img.shields.io/badge/T4-9E9AC8?style=flat-square) | Monitoring Evasion and Obfuscation | 2 | 5 |

## Gap flag distributions

| Gap | ● Addressed | ◐ Partial | ○ Present | – N/A |
|---|---|---|---|---|
| **G1** Reasoning Observability | 15 | 0 | 16 | 0 |
| **G2** Reasoning Integrity Metric | 13 | 0 | 18 | 0 |
| **G3 (T)** Defense Capability | 5 | 2 | 3 | 21 |
| **G4 (T/E)** Adaptivity | 13 | 0 | 18 | 0 |
| **G5** Agentic Scope | 16 | 0 | 15 | 0 |

## Per-paper annotations

● addressed  ·  ◐ partially addressed  ·  ○ present  ·  – not applicable

| Paper | Cluster | Vector | Target | Pattern | Structure | Scope | G1 | G2 | G3(T) | G4(T/E) | G5 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| [ShadowCoT](https://arxiv.org/abs/2504.05605) | 🟦 T1 | Training data | Reasoning / planning | CoT manipulation, Backdoor | Single-turn | LLM only | ● | ● | – | ○ | ○ |
| [Unreal Thinking](https://arxiv.org/abs/2604.09235) | 🟦 T1 | Direct prompt, Model customization | Reasoning / planning | CoT manipulation, Backdoor | Single-turn | LLM only | ● | ● | ● | ○ | ○ |
| [BadChain](https://arxiv.org/abs/2401.12242) | 🟦 T1 | Direct prompt | Reasoning / planning | CoT manipulation, Backdoor | Single-turn | LLM only | ● | ● | ◐ | ○ | ○ |
| [DarkMind](https://arxiv.org/abs/2501.18617) | 🟦 T1 | Model customization | Reasoning / planning | CoT manipulation, Backdoor | Single-turn | LLM only | ● | ● | – | ○ | ○ |
| [CoT Hijacking](https://arxiv.org/abs/2510.26418) | 🟦 T1 | Direct prompt | Reasoning / planning | CoT manipulation | Adaptive | LLM only | ● | ● | – | ● | ○ |
| [H-CoT](https://arxiv.org/abs/2502.12893) | 🟦 T1 | Direct prompt | Reasoning / planning | CoT manipulation | Single-turn | LLM only | ● | ○ | – | ○ | ○ |
| [Reasoning-Style Poisoning](https://arxiv.org/abs/2512.14448) | 🟦 T1 | Indirect prompt | Reasoning / planning | CoT manipulation | Single-turn | Agent | ● | ● | ● | ○ | ● |
| [Thought-Transfer](https://arxiv.org/abs/2601.19061) | 🟦 T1 | Training data | Reasoning / planning | CoT manipulation | Single-turn | LLM only | ○ | ○ | – | ○ | ○ |
| [ReasoningBomb](https://arxiv.org/abs/2602.00154) | 🟦 T1 | Direct prompt | Reasoning / planning | CoT manipulation | Single-turn | LLM only | ● | ● | – | ○ | ○ |
| [Adaptive Attacks](https://doi.org/10.18653/v1/2025.findings-naacl.395) | 🟧 T2 | Indirect prompt | Action / tool use | Tool manipulation, Goal hijacking | Adaptive | Agent | ○ | ○ | – | ● | ● |
| [AdapTools](https://arxiv.org/abs/2602.20720) | 🟧 T2 | Indirect prompt | Action / tool use | Tool manipulation, Goal hijacking | Adaptive | Agent | ○ | ○ | – | ● | ● |
| [Automated Prompt Injection](https://arxiv.org/abs/2606.10525) | 🟧 T2 | Indirect prompt | Multiple components | Goal hijacking | Adaptive | Agent | ○ | ○ | – | ○ | ● |
| [AgentVigil](https://arxiv.org/abs/2505.05849) | 🟧 T2 | Indirect prompt | Action / tool use | Goal hijacking | Adaptive | Agent | ○ | ○ | – | ● | ● |
| [UDora](https://arxiv.org/abs/2503.01908) | 🟧 T2 | Indirect prompt | Reasoning / planning | CoT manipulation | Adaptive | Agent | ● | ○ | – | ● | ● |
| [SIRAJ](https://doi.org/10.18653/v1/2026.findings-eacl.171) | 🟧 T2 | Direct prompt, Indirect prompt | Multiple components | CoT manipulation | Adaptive | Agent | ○ | ○ | – | ● | ● |
| [Dark Side of LLMs](https://arxiv.org/abs/2507.06850) | 🟧 T2 | Direct prompt, Indirect prompt | Multiple components | Tool manipulation, Goal hijacking | Multi-turn | Mixed | ○ | ○ | – | ○ | ● |
| [AgentPoison](https://arxiv.org/abs/2407.12784) | 🟧 T2 | Memory | Memory / knowledge | Memory poisoning | Single-turn | Agent | ○ | ○ | – | ○ | ● |
| [PoisonedRAG](https://arxiv.org/abs/2402.07867) | 🟧 T2 | Memory | Memory / knowledge | Memory poisoning | Single-turn | Mixed | ○ | ○ | – | ○ | ● |
| [MINJA](https://proceedings.neurips.cc/paper_files/paper/2025/hash/42a97bbd9844d2bf68596730af80bcdf-Abstract-Conference.html) | 🟧 T2 | Memory | Memory / knowledge | Memory poisoning | Multi-turn | Agent | ● | ● | – | ○ | ● |
| [Attacker Moves Second](https://arxiv.org/abs/2510.09023) | 🟩 T3 | Direct prompt | Input / perception | Goal hijacking | Adaptive | Mixed | ○ | ○ | – | ● | ● |
| [Auto-RT](https://arxiv.org/abs/2501.01830) | 🟩 T3 | Direct prompt | Reasoning / planning | CoT manipulation | Adaptive | LLM only | ○ | ○ | – | ● | ○ |
| [X-Teaming](https://arxiv.org/abs/2504.13203) | 🟩 T3 | Direct prompt | Reasoning / planning | Goal hijacking | Adaptive | LLM only | ○ | ○ | ○ | ● | ○ |
| [Chain of Attack](https://doi.org/10.18653/v1/2025.findings-acl.514) | 🟩 T3 | Direct prompt | Reasoning / planning | CoT manipulation | Multi-turn, Adaptive | LLM only | ○ | ○ | – | ● | ○ |
| [ActorBreaker](https://doi.org/10.18653/v1/2025.acl-long.1207) | 🟩 T3 | Direct prompt | Reasoning / planning | CoT manipulation, Goal hijacking | Adaptive | LLM only | ○ | ○ | ○ | ● | ○ |
| [STAC](https://arxiv.org/abs/2509.25624) | 🟩 T3 | Direct prompt | Action / tool use | Tool manipulation | Multi-turn, Adaptive | Agent | ○ | ○ | ◐ | ● | ● |
| [Unsafer in Many Turns](https://arxiv.org/abs/2602.13379) | 🟩 T3 | Direct prompt, Indirect prompt | Reasoning / planning, Action / tool use | Tool manipulation | Multi-turn | Agent | ○ | ○ | ○ | ○ | ● |
| [CoT-LearnedObfuscation](https://arxiv.org/abs/2601.23086) | 🟪 T4 | Model customization | Reasoning / planning | CoT manipulation | Single-turn | LLM only | ● | ● | – | ○ | ○ |
| [Noticing the Watcher](https://arxiv.org/abs/2603.16928) | 🟪 T4 | Environment | Reasoning / planning | CoT manipulation, Goal hijacking | Adaptive | Agent | ● | ● | – | ● | ● |
| [CoT Obfuscation](https://arxiv.org/abs/2510.19851) | 🟪 T4 | Direct prompt | Reasoning / planning | CoT manipulation | Adaptive | Agent | ● | ● | ● | ○ | ● |
| [When CoT Is Necessary](https://arxiv.org/abs/2507.05246) | 🟪 T4 | Direct prompt | Reasoning / planning | CoT manipulation | Adaptive | LLM only | ● | ● | ● | ○ | ○ |
| [Covertly Sandbag](https://doi.org/10.18653/v1/2025.ijcnlp-short.33) | 🟪 T4 | Direct prompt | Reasoning / planning | CoT manipulation | Single-turn | LLM only | ● | ● | ● | ○ | ○ |

## Papers by attack class

Attack classes follow Fig. 3 of the paper.

### 🟦 T1 — Reasoning Manipulation & Backdoors

**Reasoning backdoors** (4)

- **BadChain** — [BADCHAIN: BACKDOOR CHAIN-OF-THOUGHT PROMPTING FOR LARGE LANGUAGE MODELS](https://arxiv.org/abs/2401.12242)  
  *Xiang et al. · 2024*
- **DarkMind** — [DarkMind: Latent Chain-of-Thought Backdoor in Customized LLMs](https://arxiv.org/abs/2501.18617)  
  *Guo et al. · 2025*
- **ShadowCoT** — [ShadowCoT: Cognitive Hijacking for Stealthy Reasoning Backdoors in LLMs](https://arxiv.org/abs/2504.05605)  
  *Zhao et al. · 2025*
- **Unreal Thinking** — [Unreal Thinking: Chain-of-Thought Hijacking via Two-stage Backdoor](https://arxiv.org/abs/2604.09235)  
  *Chang et al. · 2026*

**Trace hijacking & poisoning** (4)

- **CoT Hijacking** — [CHAIN-OF-THOUGHT HIJACKING](https://arxiv.org/abs/2510.26418)  
  *Zhao et al. · 2026*
- **Thought-Transfer** — [Thought-Transfer: Indirect Targeted Poisoning Attacks on Chain-of-Thought Reasoning Models](https://arxiv.org/abs/2601.19061)  
  *Chaudhari et al. · 2026*
- **Reasoning-Style Poisoning** — [Reasoning-Style Poisoning of LLM Agents via Stealthy Style Transfer: Process-Level Attacks and Runtime Monitoring in RSV Space](https://arxiv.org/abs/2512.14448)  
  *Zhou and Wang · 2026*
- **H-CoT** — [H-CoT: Hijacking the Chain-of-Thought Safety Reasoning Mechanism to Jailbreak Large Reasoning Models, Including OpenAI o1/o3, DeepSeek-R1, and Gemini 2.0 Flash Thinking](https://arxiv.org/abs/2502.12893)  
  *Kuo et al. · 2025*

**Reasoning amplification & DoS** (1)

- **ReasoningBomb** — [ReasoningBomb: A Stealthy Denial-of-Service Attack by Inducing Pathologically Long Reasoning in Large Reasoning Models](https://arxiv.org/abs/2602.00154)  
  *Liu et al. · 2026*

### 🟧 T2 — Indirect Prompt Injection & Tool-Chain Attacks

**Adaptive indirect injection** (6)

- **AdapTools** — [AdapTools: Adaptive Tool-based Indirect Prompt Injection Attacks on Agentic LLMs](https://arxiv.org/abs/2602.20720)  
  *Wang et al. · 2026*
- **AgentVigil** — [AGENTVIGIL: Generic Black-Box Red-teaming for Indirect Prompt Injection against LLM Agents](https://arxiv.org/abs/2505.05849)  
  *Wang et al. · 2025*
- **Automated Prompt Injection** — [Assessing Automated Prompt Injection Attacks in Agentic Environments](https://arxiv.org/abs/2606.10525)  
  *Hofer et al. · 2026*
- **Adaptive Attacks** — [Adaptive Attacks Break Defenses Against Indirect Prompt](https://doi.org/10.18653/v1/2025.findings-naacl.395)  
  *Zhan et al. · 2025*
- **SIRAJ** — [SIRAJ: Diverse and Efficient Red-Teaming for LLM Agents via Distilled Structured Reasoning](https://doi.org/10.18653/v1/2026.findings-eacl.171)  
  *Zhou et al. · 2026*
- **UDora** — [UDora: A Unified Red Teaming Framework against LLM Agents by Dynamically Hijacking Their Own Reasoning](https://arxiv.org/abs/2503.01908)  
  *Zhang et al. · 2025*

**Tool-chain & multi-surface compromise** (1)

- **Dark Side of LLMs** — [The Dark Side of LLMs: Agent-based Attacks for Complete Computer Takeover](https://arxiv.org/abs/2507.06850)  
  *Lupinacci et al. · 2025*

**Memory and retrieval poisoning** (3)

- **AgentPoison** — [AGENTPOISON: Red-teaming LLM Agents via Poisoning Memory or Knowledge Bases](https://arxiv.org/abs/2407.12784)  
  *Chen et al. · 2024*
- **PoisonedRAG** — [PoisonedRAG: Knowledge Corruption Attacks to Retrieval-Augmented Generation of Large Language Models](https://arxiv.org/abs/2402.07867)  
  *Zou et al. · 2025*
- **MINJA** — [Memory Injection Attacks on LLM Agents via Query-Only Interaction](https://proceedings.neurips.cc/paper_files/paper/2025/hash/42a97bbd9844d2bf68596730af80bcdf-Abstract-Conference.html)  
  *Dong et al. · 2025*

### 🟩 T3 — Adaptive & Multi-turn Attacks

**Inference-time adaptive attacks** (3)

- **Attacker Moves Second** — [THE ATTACKER MOVES SECOND: STRONGER ADAPTIVE ATTACKS BYPASS DEFENSES AGAINST LLM JAILBREAKS AND PROMPT INJECTIONS](https://arxiv.org/abs/2510.09023)  
  *Nasr et al. · 2025*
- **Auto-RT** — [AUTO-RT: Automatic Jailbreak Strategy Exploration for Red-Teaming Large Language Models](https://arxiv.org/abs/2501.01830)  
  *Liu et al. · 2025*
- **X-Teaming** — [X-Teaming: Multi-Turn Jailbreaks and Defenses with Adaptive Multi-Agents](https://arxiv.org/abs/2504.13203)  
  *Rahman et al. · 2025*

**Multi-turn intent hiding** (2)

- **Chain of Attack** — [Chain of Attack: Hide Your Intention through Multi-Turn Interrogation](https://doi.org/10.18653/v1/2025.findings-acl.514)  
  *Yang et al. · 2025*
- **ActorBreaker** — [LLMs know their vulnerabilities: Uncover Safety Gaps through Natural Distribution Shifts](https://doi.org/10.18653/v1/2025.acl-long.1207)  
  *Ren et al. · 2025*

**Multi-turn agent exploitation** (2)

- **STAC** — [STAC: WHEN INNOCENT TOOLS FORM DANGEROUS CHAINS TO JAILBREAK LLM AGENTS](https://arxiv.org/abs/2509.25624)  
  *Li et al. · 2026*
- **Unsafer in Many Turns** — [Unsafer in Many Turns: Benchmarking and Defending Multi-Turn Safety Risks in Tool-Using Agents](https://arxiv.org/abs/2602.13379)  
  *Li et al. · 2026*

### 🟪 T4 — Monitoring Evasion & Obfuscation

**Obfuscation & monitor awareness** (3)

- **CoT-LearnedObfuscation** — [Chain-of-thought obfuscation learned from output supervision can generalise to unseen tasks](https://arxiv.org/abs/2601.23086)  
  *Hadida et al. · 2026*
- **Noticing the Watcher** — [NOTICING THE WATCHER: LLM AGENTS CAN INFER COT MONITORING FROM BLOCKING FEEDBACK](https://arxiv.org/abs/2603.16928)  
  *Jiralerspong et al. · 2026*
- **CoT Obfuscation** — [CAN REASONING MODELS OBFUSCATE REASONING? STRESS-TESTING CHAIN-OF-THOUGHT MONITORABILITY](https://arxiv.org/abs/2510.19851)  
  *Zolkowski et al. · 2025*

**CoT monitorability limits** (2)

- **When CoT Is Necessary** — [When Chain of Thought is Necessary, Language Models Struggle to Evade Monitors](https://arxiv.org/abs/2507.05246)  
  *Emmons et al. · 2025*
- **Covertly Sandbag** — [LLMs Can Covertly Sandbag on Capability Evaluations Against Chain-of-Thought Monitoring](https://doi.org/10.18653/v1/2025.ijcnlp-short.33)  
  *Li et al. · 2025*
