<!-- Generated from the project's annotation workbooks. Do not edit by hand. -->

# Evaluation taxonomy (E1–E3)

64 evaluation papers from the annotated empirical corpus, grouped into three clusters by what the evaluation measures.

## Clusters

| Cluster | Name | Subgroups | Papers |
|---|---|---|---|
| 🟧 ![E1](https://img.shields.io/badge/E1-FC8D62?style=flat-square) | Boundary Robustness Evaluation | 3 | 14 |
| 🟩 ![E2](https://img.shields.io/badge/E2-7DBD54?style=flat-square) | Agent Execution and Trajectory Safety Evaluation | 5 | 33 |
| 🟦 ![E3](https://img.shields.io/badge/E3-6BAED6?style=flat-square) | Reasoning-Process Integrity and Monitorability Evaluation | 3 | 17 |

## The triple conjunction

Three properties are each necessary for an evaluation to say anything about whether an agent's *reasoning* survives a determined attacker: an explicit reasoning integrity metric (RIM), an adaptive adversary (AA), and agentic scope (G5). Each is individually attested in the corpus. No paper exhibits all three.

| Condition | Papers (of 64) |
|---|---|
| RIM = Explicit | 3 |
| AA = Y | 16 |
| G5 = ADDRESSED | 44 |
| AA = Y ∧ G5 = ADDRESSED | 12 |
| RIM = Explicit ∧ G5 = ADDRESSED | 0 |
| RIM = Explicit ∧ AA = Y | 0 |
| **All three** | **0** |

## Coded column distributions

**Adaptive adversary (AA)**

| AA | Papers |
|---|---|
| N | 48 |
| Y | 16 |

**Reasoning integrity metric (RIM)**

| RIM | Papers |
|---|---|
| N/A | 41 |
| Implicit | 20 |
| Explicit | 3 |

## Gap flag distributions

| Gap | ● Addressed | ○ Present |
|---|---|---|
| **G1** Reasoning Observability | 27 | 37 |
| **G2** Reasoning Integrity Metric | 23 | 41 |
| **G3 (E)** Defense Capability | 17 | 47 |
| **G4 (T/E)** Adaptivity | 16 | 48 |
| **G5** Agentic Scope | 44 | 20 |

## Per-paper annotations

● addressed  ·  ◐ partially addressed  ·  ○ present  ·  – not applicable

| Paper | Cluster | Subgroup | Scope | Reasoning type | Model access | Benchmark | AA | RIM | G1 | G2 | G3(E) | G4(T/E) | G5 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [Attacker Moves Second](https://arxiv.org/abs/2510.09023) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | Mixed | Unspecified | White-box, Black-box | HarmBench; AgentDojo; OpenPromptInject; Adversarial Davinci | Yes | – | ○ | ○ | ○ | ● | ● |
| [JailGuard](https://doi.org/10.1145/3724393) | 🟧 E1 | E1.1 Guardrail Detection and Defense Reliability | LLM only | CoT | Black-box | Own 11,000-sample prompt-attack dataset, text + image (introduced) | No | – | ○ | ○ | ○ | ○ | ○ |
| [DarkMind](https://arxiv.org/abs/2501.18617) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | LLM only | CoT | Black-box | GSM8K; MATH; ASDiv; SVAMP; AQuA-RAT; commonsense and symbolic sets | No | Implicit | ● | ● | ○ | ○ | ○ |
| [BadChain](https://arxiv.org/abs/2401.12242) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | LLM only | CoT | Black-box | GSM8K; MATH; ASDiv; CSQA; StrategyQA; Letter | No | Implicit | ● | ● | ○ | ○ | ○ |
| [Chain of Attack](https://doi.org/10.18653/v1/2025.findings-acl.514) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | LLM only | CoT | Black-box | AdvBench | Yes | – | ○ | ○ | ○ | ● | ○ |
| [X-Teaming](https://arxiv.org/abs/2504.13203) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | LLM only | CoT, ReAct | Black-box | HarmBench | Yes | – | ○ | ○ | ○ | ● | ○ |
| [PIGuard](https://doi.org/10.18653/v1/2025.acl-long.1468) | 🟧 E1 | E1.1 Guardrail Detection and Defense Reliability | LLM only | ReAct | – | NotInject (introduced); PINT; BIPIA; WildGuard | No | – | ○ | ○ | ○ | ○ | ○ |
| [PISanitizer](https://arxiv.org/abs/2511.10720) | 🟧 E1 | E1.2 Prompt-Injection Defense Robustness | Agent | ReAct | – | LongBench (Qasper, HotpotQA, GovReport, MultiNews, LCC, PassageRetrieval) | No | – | ○ | ○ | ○ | ○ | ● |
| StruQ | 🟧 E1 | E1.2 Prompt-Injection Defense Robustness | LLM only | – | – | AlpacaEval; HackAPrompt; BIPIA | Yes | – | ○ | ○ | ○ | ● | ○ |
| [Instruction Hierarchy](https://arxiv.org/abs/2404.13208) | 🟧 E1 | E1.2 Prompt-Injection Defense Robustness | LLM only | – | – | Open-source and novel prompt-injection / jailbreak sets; TensorTrust; Gandalf | No | – | ○ | ○ | ○ | ○ | ○ |
| SecAlign | 🟧 E1 | E1.2 Prompt-Injection Defense Robustness | Mixed | – | – | AlpacaEval2; SEP; InjecAgent | Yes | – | ○ | ○ | ○ | ● | ● |
| [PromptShield](https://doi.org/10.1145/3714393.3726501) | 🟧 E1 | E1.1 Guardrail Detection and Defense Reliability | LLM only | – | – | PromptShield benchmark (introduced); FourAttacks; HackAPrompt; OpenPromptInject | No | – | ○ | ○ | ○ | ○ | ○ |
| [H-CoT](https://arxiv.org/abs/2502.12893) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | LLM only | CoT | Black-box | Malicious-Educator (introduced) | No | – | ● | ○ | ○ | ○ | ○ |
| [PoisonedRAG](https://arxiv.org/abs/2402.07867) | 🟧 E1 | E1.3 Attack-Led Robustness Evaluation | Mixed | Multiple | Black-box | NQ; HotpotQA; MS-MARCO; FEVER | No | – | ○ | ○ | ○ | ○ | ● |
| [AgentMonitor](https://arxiv.org/abs/2408.14972) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Execution monitoring and action validation | Multi-agent | ReAct | White-box, Black-box | BeaverTails; MaliciousInstruct; AdvBench (safety); HumanEval; MMLU; GSM8K (capability) | No | – | ○ | ○ | ○ | ○ | ● |
| [AgentDoG](https://arxiv.org/abs/2601.18491) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair | Agent | ReAct | White-box | ATBench (introduced) | No | Implicit | ● | ● | ○ | ○ | ● |
| [RTBAS](https://arxiv.org/abs/2502.08966) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | ReAct | – | AgentDojo; Accidental Leakage benchmark (introduced) | No | – | ○ | ○ | ○ | ○ | ● |
| [AgentDojo](https://arxiv.org/abs/2406.13352) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | ReAct | – | AgentDojo (introduced) | No | – | ○ | ○ | ○ | ○ | ● |
| [UDora](https://arxiv.org/abs/2503.01908) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | CoT / ReAct | White-box | InjecAgent; WebShop; AgentHarm | Yes | – | ● | ○ | ○ | ● | ● |
| [Automated Prompt Injection](https://arxiv.org/abs/2606.10525) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | ReAct | White-box, Black-box | AgentDojo | No | – | ○ | ○ | ○ | ○ | ● |
| [SIRAJ](https://doi.org/10.18653/v1/2026.findings-eacl.171) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | ReAct | Black-box | Agent-SafetyBench | Yes | – | ○ | ○ | ○ | ● | ● |
| [AgentVigil](https://arxiv.org/abs/2505.05849) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | ReAct | Black-box | AgentDojo; VWA-adv | Yes | – | ○ | ○ | ○ | ● | ● |
| [Adaptive Attacks](https://doi.org/10.18653/v1/2025.findings-naacl.395) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | ReAct | White-box | InjecAgent; AgentDojo | Yes | – | ○ | ○ | ○ | ● | ● |
| [AdapTools](https://arxiv.org/abs/2602.20720) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | CoT | Grey-box, Black-box | IPI-3K (introduced); InjecAgent; AgentDojo | Yes | – | ○ | ○ | ○ | ● | ● |
| [SafeAgent](https://arxiv.org/abs/2604.17562) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair | Agent | ReAct | – | Agent Security Bench (ASB); InjecAgent | No | – | ○ | ○ | ○ | ○ | ● |
| [AgentArmor](https://arxiv.org/abs/2508.01249) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Containment and multi-turn risk | Agent | ReAct | Black-box | AgentDojo; Agent Security Bench (ASB) | No | – | ○ | ○ | ○ | ○ | ● |
| [Unsafer in Many Turns](https://arxiv.org/abs/2602.13379) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Containment and multi-turn risk | Agent | ReAct | Black-box | MT-AgentRisk | No | – | ○ | ○ | ○ | ○ | ● |
| IntentGuard | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Execution monitoring and action validation | Agent | ReAct | – | Agent Security Bench (ASB) | No | Implicit | ● | ● | ● | ○ | ● |
| [ProbGuard](https://arxiv.org/abs/2508.00500) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Execution monitoring and action validation | Agent | ReAct | – | Apollo / uDrive with LawBreaker properties; SafeAgentBench | No | – | ○ | ○ | ○ | ○ | ● |
| [GuardAgent](https://arxiv.org/abs/2406.09187) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair | Agent | ReAct | – | EICU-AC; Mind2Web-SC | No | – | ○ | ○ | ○ | ○ | ● |
| [CaMeL](https://arxiv.org/abs/2503.18813) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Containment and multi-turn risk | Agent | ReAct | Black-box | AgentDojo | No | – | ○ | ○ | ○ | ○ | ● |
| [Psg-Agent](https://arxiv.org/abs/2509.23614) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair | Agent | ReAct | – | Personalized safety benchmark, ~2,900 examples across 8 scenarios (introduced) | No | – | ○ | ○ | ● | ○ | ● |
| [AGrail](https://doi.org/10.18653/v1/2025.acl-long.399) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair | Agent | ReAct | – | Mind2Web-SC; EICU-AC; Safe-OS; AdvWeb; EIA | No | – | ○ | ○ | ○ | ○ | ● |
| [TrustAgent](https://doi.org/10.18653/v1/2024.findings-emnlp.585) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair | Agent | ReAct | – | 70-datapoint dataset across 5 domains (introduced) | No | – | ○ | ○ | ● | ○ | ● |
| [AgentSentinel](https://doi.org/10.1145/3719027.3765064) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Execution monitoring and action validation | Agent | ReAct | – | BadComputerUse | No | – | ○ | ○ | ○ | ○ | ● |
| [IsolateGPT](https://doi.org/10.14722/ndss.2025.241131) | 🟩 E2 | E2.2 Runtime Execution and Trajectory Safety — Containment and multi-turn risk | Agent | ReAct | – | Enhanced security benchmark, 1,598 attacks (introduced); LangChain app benchmarks | No | – | ○ | ○ | ○ | ○ | ● |
| [PromptArmor](https://arxiv.org/abs/2507.15219) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | – | – | AgentDojo | Yes | – | ○ | ○ | ○ | ● | ● |
| [Tool Result Parsing](https://arxiv.org/abs/2601.04795) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | – | – | AgentDojo | No | – | ○ | ○ | ○ | ○ | ● |
| [AgentVisor](https://arxiv.org/abs/2604.24118) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | – | – | OpenPromptInjection; AgentDojo | Yes | – | ○ | ○ | ○ | ● | ● |
| [ICON](https://arxiv.org/abs/2602.20708) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | – | – | InjecAgent; AgentDojo; TrojanTools | No | Implicit | ● | ● | ● | ○ | ● |
| ASB | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | – | – | Agent Security Bench / ASB (introduced) | No | – | ● | ○ | ○ | ○ | ● |
| [AgentPoison](https://arxiv.org/abs/2407.12784) | 🟩 E2 | E2.3 Attack-Led Agent-Execution Stress Testing | Agent | CoT | Black-box | Agent-Driver; ReAct-StrategyQA; EHRAgent | No | – | ○ | ○ | ○ | ○ | ● |
| AgentHarm | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | Multiple | Black-box | AgentHarm (introduced) | No | – | ○ | ○ | ○ | ○ | ● |
| [WASP](https://arxiv.org/abs/2504.18575) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | Multiple | Black-box | WASP, on the VisualWebArena sandbox (introduced) | No | Implicit | ● | ● | ○ | ○ | ● |
| [InjecAgent](https://arxiv.org/abs/2403.02691) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | ReAct | Black-box | InjecAgent (introduced) | No | – | ● | ○ | ○ | ○ | ● |
| [Agent-Safetybench](https://arxiv.org/abs/2412.14470) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | Unspecified | – | Agent-SafetyBench (introduced) | No | – | ○ | ○ | ○ | ○ | ● |
| [AgentDyn](https://arxiv.org/abs/2602.03117) | 🟩 E2 | E2.1 Security-Utility Evaluation in Tool Environments | Agent | – | – | AgentDyn (introduced) | No | – | ○ | ○ | ○ | ○ | ● |
| [ReasoningBomb](https://arxiv.org/abs/2602.00154) | 🟦 E3 | E3.1 Reasoning Manipulation and Repair Evaluation | LLM only | CoT | White-box | SimpleQA; SimpleBench; AIME 2024; LLM-Generated Puzzles; LRM-Generated Puzzles; ReasoningBomb attack prompts (128 / 256 / 512-token budgets) | No | Implicit | ● | ● | ○ | ○ | ○ |
| [CoT Hijacking](https://arxiv.org/abs/2510.26418) | 🟦 E3 | E3.1 Reasoning Manipulation and Repair Evaluation | LLM only | CoT | Black-box | HarmBench | Yes | Implicit | ● | ● | ○ | ● | ○ |
| [Reasoning-Style Poisoning](https://arxiv.org/abs/2512.14448) | 🟦 E3 | E3.1 Reasoning Manipulation and Repair Evaluation | Agent | Multiple | White-box | HotpotQA; FEVER | No | Implicit | ● | ● | ● | ○ | ● |
| [Monitoring Reasoning Models](https://arxiv.org/abs/2503.11926) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | Agent | CoT | White-box | Agentic coding environment (repository unit-test tasks) | Yes | Implicit | ● | ● | ● | ● | ● |
| [Thought Purity](https://arxiv.org/abs/2507.12314) | 🟦 E3 | E3.1 Reasoning Manipulation and Repair Evaluation | LLM only | CoT | White-box | Letter; CSQA; GSM8K; StrategyQA | No | Implicit | ● | ● | ● | ○ | ○ |
| [Unreal Thinking](https://arxiv.org/abs/2604.09235) | 🟦 E3 | E3.1 Reasoning Manipulation and Repair Evaluation | LLM only | CoT | White-box | AdvBench; StrongREJECT; GSM8K; MMLU; XSTest | No | Implicit | ● | ● | ● | ○ | ○ |
| [Noticing the Watcher](https://arxiv.org/abs/2603.16928) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | Agent | ReAct | Black-box | SHADE-Arena (Calendar Agendas, Bank Transfer) | Yes | Implicit | ● | ● | ● | ● | ● |
| [CoT Obfuscation](https://arxiv.org/abs/2510.19851) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | Agent | ReAct | – | SHADE-Arena; toy hidden-task settings | No | Implicit | ● | ● | ● | ○ | ● |
| [When CoT Is Necessary](https://arxiv.org/abs/2507.05246) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | LLM only | CoT | Black-box | Forced-CoT algebra tasks; GPQA; SHADE-Arena-style side-task environment | No | Explicit | ● | ● | ● | ○ | ○ |
| [Covertly Sandbag](https://doi.org/10.18653/v1/2025.ijcnlp-short.33) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | LLM only | CoT | Black-box | WMDP; MMLU; ProtocolQA | No | Implicit | ● | ● | ● | ○ | ○ |
| [MonitorBench](https://arxiv.org/abs/2603.28590) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | Mixed | CoT | – | MonitorBench (introduced) | Yes | Implicit | ● | ● | ● | ● | ● |
| [AutoMonitor-Bench](https://arxiv.org/abs/2601.05752) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | LLM only | – | – | AutoMonitor-Bench (introduced) | No | Implicit | ● | ● | ● | ○ | ○ |
| [BONA FIDE](https://arxiv.org/abs/2605.25052) | 🟦 E3 | E3.3 Faithfulness Metrics and Judge Validation | LLM only | – | – | BONA FIDE (introduced) | No | Explicit | ● | ● | ● | ○ | ○ |
| [CoT Faithfulness Audit](https://arxiv.org/abs/2505.05410) | 🟦 E3 | E3.3 Faithfulness Metrics and Judge Validation | LLM only | – | – | Paired multiple-choice hint prompts; 6 synthetic RL reward-hack environments | No | Implicit | ● | ● | ● | ○ | ○ |
| [C2-Faith](https://arxiv.org/abs/2603.05167) | 🟦 E3 | E3.3 Faithfulness Metrics and Judge Validation | LLM only | – | – | C2-Faith, PRM800K-based (introduced) | No | Explicit | ● | ● | ○ | ○ | ○ |
| [MINJA](https://proceedings.neurips.cc/paper_files/paper/2025/hash/42a97bbd9844d2bf68596730af80bcdf-Abstract-Conference.html) | 🟦 E3 | E3.1 Reasoning Manipulation and Repair Evaluation | Agent | Multiple | Grey-box | WebShop (RAP); MIMIC-III and eICU (EHRAgent); MMLU (QA agent) | No | Implicit | ● | ● | ○ | ○ | ● |
| [SHADE-Arena](https://arxiv.org/abs/2506.15740) | 🟦 E3 | E3.2 CoT Monitorability and Evasion Evaluation | Agent | ReAct | – | SHADE-Arena (introduced) | No | Implicit | ● | ● | ● | ○ | ● |

## Papers by subgroup

### 🟧 E1 — Boundary Robustness Evaluation

**E1.3 Attack-Led Robustness Evaluation** (7)

- **Attacker Moves Second** — [THE ATTACKER MOVES SECOND: STRONGER ADAPTIVE ATTACKS BYPASS DEFENSES AGAINST LLM JAILBREAKS AND PROMPT INJECTIONS](https://arxiv.org/abs/2510.09023)  
  *Nasr et al. · 2025*
- **DarkMind** — [DarkMind: Latent Chain-of-Thought Backdoor in Customized LLMs](https://arxiv.org/abs/2501.18617)  
  *Guo et al. · 2025*
- **BadChain** — [BADCHAIN: BACKDOOR CHAIN-OF-THOUGHT PROMPTING FOR LARGE LANGUAGE MODELS](https://arxiv.org/abs/2401.12242)  
  *Xiang et al. · 2024*
- **Chain of Attack** — [Chain of Attack: Hide Your Intention through Multi-Turn Interrogation](https://doi.org/10.18653/v1/2025.findings-acl.514)  
  *Yang et al. · 2025*
- **X-Teaming** — [X-Teaming: Multi-Turn Jailbreaks and Defenses with Adaptive Multi-Agents](https://arxiv.org/abs/2504.13203)  
  *Rahman et al. · 2025*
- **H-CoT** — [H-CoT: Hijacking the Chain-of-Thought Safety Reasoning Mechanism to Jailbreak Large Reasoning Models, Including OpenAI o1/o3, DeepSeek-R1, and Gemini 2.0 Flash Thinking](https://arxiv.org/abs/2502.12893)  
  *Kuo et al. · 2025*
- **PoisonedRAG** — [PoisonedRAG: Knowledge Corruption Attacks to Retrieval-Augmented Generation of Large Language Models](https://arxiv.org/abs/2402.07867)  
  *Zou et al. · 2025*

**E1.1 Guardrail Detection and Defense Reliability** (3)

- **JailGuard** — [JailGuard: A Universal Detection Framework for Prompt-based Attacks on LLM Systems](https://doi.org/10.1145/3724393)  
  *Zhang et al. · 2025*
- **PIGuard** — [PIGuard: Prompt Injection Guardrail via Mitigating Overdefense for Free](https://doi.org/10.18653/v1/2025.acl-long.1468)  
  *Li et al. · 2025*
- **PromptShield** — [PromptShield: Deployable Detection for Prompt Injection Attacks](https://doi.org/10.1145/3714393.3726501)  
  *Jacob et al. · 2025*

**E1.2 Prompt-Injection Defense Robustness** (4)

- **PISanitizer** — [PISanitizer: Preventing Prompt Injection to Long-Context LLMs via Prompt Sanitization](https://arxiv.org/abs/2511.10720)  
  *Geng et al. · 2025*
- **StruQ** — StruQ: Defending Against Prompt Injection with Structured Queries  
  *Chen et al. · 2025*
- **Instruction Hierarchy** — [The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions](https://arxiv.org/abs/2404.13208)  
  *Wallace et al. · 2025*
- **SecAlign** — SecAlign: Defending Against Prompt Injection with Preference Optimization  
  *Chen et al. · 2025*

### 🟩 E2 — Agent Execution and Trajectory Safety Evaluation

**E2.2 Runtime Execution and Trajectory Safety — Execution monitoring and action validation** (4)

- **AgentMonitor** — [AGENTMONITOR: A PLUG-AND-PLAY FRAMEWORK FOR PREDICTIVE AND SECURE MULTI-AGENT SYSTEMS](https://arxiv.org/abs/2408.14972)  
  *Chan et al. · 2024*
- **IntentGuard** — IntentGuard: Safeguard LLM Agents via Intent Alignment  
  *Cong et al. · 2026*
- **ProbGuard** — [ProbGuard: Probabilistic Runtime Monitoring for LLM Agent Safety](https://arxiv.org/abs/2508.00500)  
  *Wang et al. · 2026*
- **AgentSentinel** — [AgentSentinel: An End-to-End and Real-Time Security Defense Framework for Computer-Use Agents](https://doi.org/10.1145/3719027.3765064)  
  *Hu et al. · 2025*

**E2.2 Runtime Execution and Trajectory Safety — Trajectory-level guardrails and repair** (6)

- **AgentDoG** — [AgentDoG: A Diagnostic Guardrail Framework for AI Agent Safety and Security](https://arxiv.org/abs/2601.18491)  
  *Liu et al. · 2026*
- **SafeAgent** — [SafeAgent: A Runtime Protection Architecture for Agentic Systems](https://arxiv.org/abs/2604.17562)  
  *Liu et al. · 2026*
- **GuardAgent** — [GuardAgent: Safeguard LLM Agents via Knowledge-Enabled Reasoning](https://arxiv.org/abs/2406.09187)  
  *Xiang et al. · 2025*
- **Psg-Agent** — [PSG-AGENT: PERSONALITY-AWARE SAFETY GUARDRAIL FOR LLM-BASED AGENTS](https://arxiv.org/abs/2509.23614)  
  *Wu et al. · 2025*
- **AGrail** — [AGrail: A Lifelong Agent Guardrail with Effective and Adaptive Safety Detection](https://doi.org/10.18653/v1/2025.acl-long.399)  
  *Luo et al. · 2025*
- **TrustAgent** — [TrustAgent: Towards Safe and Trustworthy LLM-based Agents](https://doi.org/10.18653/v1/2024.findings-emnlp.585)  
  *Hua et al. · 2024*

**E2.1 Security-Utility Evaluation in Tool Environments** (12)

- **RTBAS** — [RTBAS: Defending LLM Agents Against Prompt Injection and Privacy Leakage](https://arxiv.org/abs/2502.08966)  
  *Zhong et al. · 2025*
- **AgentDojo** — [AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for LLM Agents](https://arxiv.org/abs/2406.13352)  
  *Debenedetti et al. · 2024*
- **PromptArmor** — [PromptArmor: Simple yet Effective Prompt Injection Defenses](https://arxiv.org/abs/2507.15219)  
  *Shi et al. · 2025*
- **Tool Result Parsing** — [Defense Against Indirect Prompt Injection via Tool Result Parsing](https://arxiv.org/abs/2601.04795)  
  *Yu et al. · 2026*
- **AgentVisor** — [AgentVisor: Defending LLM Agents Against Prompt Injection via Semantic Virtualization](https://arxiv.org/abs/2604.24118)  
  *Ying et al. · 2026*
- **ICON** — [ICON: Indirect Prompt Injection Defense for Agents based on Inference-Time Correction](https://arxiv.org/abs/2602.20708)  
  *Wang et al. · 2026*
- **ASB** — Agent Security Bench (ASB): Formalizing and Benchmarking Attacks and Defenses in LLM-based Agents  
  *Zhang et al. · 2025*
- **AgentHarm** — AgentHarm: A Benchmark for Measuring Harmfulness of LLM Agents  
  *Andriushchenko et al. · 2025*
- **WASP** — [WASP: Benchmarking Web Agent Security Against Prompt Injection Attacks](https://arxiv.org/abs/2504.18575)  
  *Evtimov et al. · 2025*
- **InjecAgent** — [INJECAGENT: Benchmarking Indirect Prompt Injections in Tool-Integrated Large Language Model Agents](https://arxiv.org/abs/2403.02691)  
  *Zhan et al. · 2024*
- **Agent-Safetybench** — [AGENT-SAFETYBENCH: Evaluating the Safety of LLM Agents](https://arxiv.org/abs/2412.14470)  
  *Zhang et al. · 2025*
- **AgentDyn** — [AgentDyn: Are Your Agent Security Defenses Deployable in Real-World Dynamic Environments?](https://arxiv.org/abs/2602.03117)  
  *Li et al. · 2026*

**E2.3 Attack-Led Agent-Execution Stress Testing** (7)

- **UDora** — [UDora: A Unified Red Teaming Framework against LLM Agents by Dynamically Hijacking Their Own Reasoning](https://arxiv.org/abs/2503.01908)  
  *Zhang et al. · 2025*
- **Automated Prompt Injection** — [Assessing Automated Prompt Injection Attacks in Agentic Environments](https://arxiv.org/abs/2606.10525)  
  *Hofer et al. · 2026*
- **SIRAJ** — [SIRAJ: Diverse and Efficient Red-Teaming for LLM Agents via Distilled Structured Reasoning](https://doi.org/10.18653/v1/2026.findings-eacl.171)  
  *Zhou et al. · 2026*
- **AgentVigil** — [AGENTVIGIL: Generic Black-Box Red-teaming for Indirect Prompt Injection against LLM Agents](https://arxiv.org/abs/2505.05849)  
  *Wang et al. · 2025*
- **Adaptive Attacks** — [Adaptive Attacks Break Defenses Against Indirect Prompt](https://doi.org/10.18653/v1/2025.findings-naacl.395)  
  *Zhan et al. · 2025*
- **AdapTools** — [AdapTools: Adaptive Tool-based Indirect Prompt Injection Attacks on Agentic LLMs](https://arxiv.org/abs/2602.20720)  
  *Wang et al. · 2026*
- **AgentPoison** — [AGENTPOISON: Red-teaming LLM Agents via Poisoning Memory or Knowledge Bases](https://arxiv.org/abs/2407.12784)  
  *Chen et al. · 2024*

**E2.2 Runtime Execution and Trajectory Safety — Containment and multi-turn risk** (4)

- **AgentArmor** — [Securing Large Language Model Agents via Structured Graph Abstraction AgentArmor: Enforcing Program Analysis on Agent Runtime Trace to Defend Against Prompt Injection](https://arxiv.org/abs/2508.01249)  
  *Wang et al. · 2025*
- **Unsafer in Many Turns** — [Unsafer in Many Turns: Benchmarking and Defending Multi-Turn Safety Risks in Tool-Using Agents](https://arxiv.org/abs/2602.13379)  
  *Li et al. · 2026*
- **CaMeL** — [Defeating Prompt Injections by Design / CaMeL](https://arxiv.org/abs/2503.18813)  
  *Debenedetti et al. · 2025*
- **IsolateGPT** — [IsolateGPT: An Execution Isolation Architecture for LLM-Based Agentic Systems](https://doi.org/10.14722/ndss.2025.241131)  
  *Wu et al. · 2025*

### 🟦 E3 — Reasoning-Process Integrity and Monitorability Evaluation

**E3.1 Reasoning Manipulation and Repair Evaluation** (6)

- **ReasoningBomb** — [ReasoningBomb: A Stealthy Denial-of-Service Attack by Inducing Pathologically Long Reasoning in Large Reasoning Models](https://arxiv.org/abs/2602.00154)  
  *Liu et al. · 2026*
- **CoT Hijacking** — [CHAIN-OF-THOUGHT HIJACKING](https://arxiv.org/abs/2510.26418)  
  *Zhao et al. · 2026*
- **Reasoning-Style Poisoning** — [Reasoning-Style Poisoning of LLM Agents via Stealthy Style Transfer: Process-Level Attacks and Runtime Monitoring in RSV Space](https://arxiv.org/abs/2512.14448)  
  *Zhou and Wang · 2026*
- **Thought Purity** — [Thought Purity: A Defense Framework For Chain-of-Thought Attack](https://arxiv.org/abs/2507.12314)  
  *Xue et al. · 2026*
- **Unreal Thinking** — [Unreal Thinking: Chain-of-Thought Hijacking via Two-stage Backdoor](https://arxiv.org/abs/2604.09235)  
  *Chang et al. · 2026*
- **MINJA** — [Memory Injection Attacks on LLM Agents via Query-Only Interaction](https://proceedings.neurips.cc/paper_files/paper/2025/hash/42a97bbd9844d2bf68596730af80bcdf-Abstract-Conference.html)  
  *Dong et al. · 2025*

**E3.2 CoT Monitorability and Evasion Evaluation** (8)

- **Monitoring Reasoning Models** — [Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation](https://arxiv.org/abs/2503.11926)  
  *Baker et al. · 2025*
- **Noticing the Watcher** — [NOTICING THE WATCHER: LLM AGENTS CAN INFER COT MONITORING FROM BLOCKING FEEDBACK](https://arxiv.org/abs/2603.16928)  
  *Jiralerspong et al. · 2026*
- **CoT Obfuscation** — [CAN REASONING MODELS OBFUSCATE REASONING? STRESS-TESTING CHAIN-OF-THOUGHT MONITORABILITY](https://arxiv.org/abs/2510.19851)  
  *Zolkowski et al. · 2025*
- **When CoT Is Necessary** — [When Chain of Thought is Necessary, Language Models Struggle to Evade Monitors](https://arxiv.org/abs/2507.05246)  
  *Emmons et al. · 2025*
- **Covertly Sandbag** — [LLMs Can Covertly Sandbag on Capability Evaluations Against Chain-of-Thought Monitoring](https://doi.org/10.18653/v1/2025.ijcnlp-short.33)  
  *Li et al. · 2025*
- **MonitorBench** — [MonitorBench: A Comprehensive Benchmark for Chain-of-Thought Monitorability in Large Language Models](https://arxiv.org/abs/2603.28590)  
  *Wang et al. · 2026*
- **AutoMonitor-Bench** — [AutoMonitor-Bench: Evaluating the Reliability of LLM-Based Misbehavior Monitors](https://arxiv.org/abs/2601.05752)  
  *Yang et al. · 2026*
- **SHADE-Arena** — [SHADE-Arena: Evaluating Sabotage and Monitoring in LLM Agents](https://arxiv.org/abs/2506.15740)  
  *Kutasov et al. · 2025*

**E3.3 Faithfulness Metrics and Judge Validation** (3)

- **BONA FIDE** — [Faithfulness Metrics Don’t Measure Faithfulness: A Meta-Evaluation with Ground Truth](https://arxiv.org/abs/2605.25052)  
  *Gur-Arieh et al. · 2026*
- **CoT Faithfulness Audit** — [Reasoning Models Don’t Always Say What They Think](https://arxiv.org/abs/2505.05410)  
  *Chen et al. · 2025*
- **C2-Faith** — [C2-Faith: Benchmarking LLM Judges for Causal and Coverage Faithfulness in Chain-of-Thought Reasoning](https://arxiv.org/abs/2603.05167)  
  *Mittal and Arike · 2026*
