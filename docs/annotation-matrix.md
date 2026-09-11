<!-- Generated from the project's annotation workbooks. Do not edit by hand. -->

# Annotation matrix

The full per-paper annotation matrix: 71 papers × 21 columns. This is the artifact the manuscript refers to as the accompanying repository annotation matrix, and it is the record from which every count in the paper is computed.

A paper may carry a threat, defense, and/or evaluation cluster assignment, so the three taxonomy counts overlap and do not sum to 71. Blank cluster cells mean the paper was not routed to that taxonomy; `N/A` in a coded column means the dimension does not apply to that paper's contribution type.

Papers are identified by short name, as used in the manuscript. The `ID` column is retained only as a join key against the CSV exports and the source workbooks.

## Coded vocabulary

| Column | Admissible values |
|---|---|
| Adaptive adversary (AA) | `Y` / `N` / `N/A` |
| Reasoning integrity metric (RIM) | `Explicit` / `Implicit` / `N/A` |
| Adaptive robustness eval (ARE) | `Y` / `Partial` / `N` |
| G1, G2, G5 | `ADDRESSED` / `PRESENT` / `N/A` |
| G3 (D), G4 (D) | `ADDRESSED` / `PARTIAL` / `PRESENT` / `N/A` |
| G3 (T), G3 (E), G4 (T/E) | `ADDRESSED` / `PRESENT` / `N/A` |

Free-text `Gap / Limitation` fields in the source workbooks are descriptive only and are never the basis for a coded flag.

## Matrix

● addressed  ·  ◐ partially addressed  ·  ○ present  ·  – not applicable

| Paper | ID | Yr | T | D | E | Scope | RIM | AA | ARE | R-aware | G1 | G2 | G3(T) | G3(D) | G3(E) | G4(T/E) | G4(D) | G5 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [Attacker Moves Second](https://arxiv.org/abs/2510.09023) | E01 | 2025 | 🟩 T3 | – | 🟧 E1 | Mixed | – | Yes | – | – | ○ | ○ | – | – | ○ | ● | – | ● |
| [AgentMonitor](https://arxiv.org/abs/2408.14972) | E02 | 2024 | – | 🟩 D2 | 🟩 E2 | Multi-agent | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| [JailGuard](https://doi.org/10.1145/3724393) | E05 | 2025 | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ○ |
| [AgentDoG](https://arxiv.org/abs/2601.18491) | E07 | 2026 | – | 🟦 D3 | 🟩 E2 | Agent | Implicit | No | Partial | Yes | ● | ● | – | ● | ○ | ○ | ◐ | ● |
| [RTBAS](https://arxiv.org/abs/2502.08966) | E08 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| [AgentDojo](https://arxiv.org/abs/2406.13352) | E09 | 2024 | – | – | 🟩 E2 | Agent | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| [ReasoningBomb](https://arxiv.org/abs/2602.00154) | E10 | 2026 | 🟦 T1 | – | 🟦 E3 | LLM only | Implicit | No | – | – | ● | ● | – | – | ○ | ○ | – | ○ |
| [UDora](https://arxiv.org/abs/2503.01908) | E11 | 2025 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | – | ● | ○ | – | – | ○ | ● | – | ● |
| [Automated Prompt Injection](https://arxiv.org/abs/2606.10525) | E12 | 2026 | 🟧 T2 | – | 🟩 E2 | Agent | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| [SIRAJ](https://doi.org/10.18653/v1/2026.findings-eacl.171) | E13 | 2026 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | – | ○ | ○ | – | – | ○ | ● | – | ● |
| [Dark Side of LLMs](https://arxiv.org/abs/2507.06850) | E14 | 2025 | 🟧 T2 | – | – | Mixed | – | No | – | – | ○ | ○ | – | – | – | ○ | – | ● |
| [AgentVigil](https://arxiv.org/abs/2505.05849) | E15 | 2025 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | – | ○ | ○ | – | – | ○ | ● | – | ● |
| [CoT Hijacking](https://arxiv.org/abs/2510.26418) | E16 | 2026 | 🟦 T1 | – | 🟦 E3 | LLM only | Implicit | Yes | – | – | ● | ● | – | – | ○ | ● | – | ○ |
| [STAC](https://arxiv.org/abs/2509.25624) | E17 | 2026 | 🟩 T3 | 🟦 D3 | – | Agent | – | Yes | Yes | Partial | ○ | ○ | ◐ | ◐ | – | ● | ● | ● |
| [ShadowCoT](https://arxiv.org/abs/2504.05605) | E18 | 2025 | 🟦 T1 | – | – | LLM only | Implicit | No | – | – | ● | ● | – | – | – | ○ | – | ○ |
| [DarkMind](https://arxiv.org/abs/2501.18617) | E20 | 2025 | 🟦 T1 | – | 🟧 E1 | LLM only | Implicit | No | – | – | ● | ● | – | – | ○ | ○ | – | ○ |
| [Adaptive Attacks](https://doi.org/10.18653/v1/2025.findings-naacl.395) | E21 | 2025 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | – | ○ | ○ | – | – | ○ | ● | – | ● |
| [AdapTools](https://arxiv.org/abs/2602.20720) | E22 | 2026 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | – | ○ | ○ | – | – | ○ | ● | – | ● |
| [Reasoning-Style Poisoning](https://arxiv.org/abs/2512.14448) | E23 | 2026 | 🟦 T1 | 🟦 D3 | 🟦 E3 | Agent | Implicit | No | No | Yes | ● | ● | ● | ● | ● | ○ | ○ | ● |
| [BadChain](https://arxiv.org/abs/2401.12242) | E24 | 2024 | 🟦 T1 | 🟧 D1 | 🟧 E1 | LLM only | Implicit | No | No | No | ● | ● | ◐ | ◐ | ○ | ○ | ○ | ○ |
| [Auto-RT](https://arxiv.org/abs/2501.01830) | E25 | 2025 | 🟩 T3 | – | – | LLM only | – | Yes | – | – | ○ | ○ | – | – | – | ● | – | ○ |
| [Monitoring Reasoning Models](https://arxiv.org/abs/2503.11926) | E26 | 2025 | – | 🟦 D3 | 🟦 E3 | Agent | Implicit | Yes | Yes | Yes | ● | ● | – | ● | ● | ● | ● | ● |
| [Thought-Transfer](https://arxiv.org/abs/2601.19061) | E27 | 2026 | 🟦 T1 | – | – | LLM only | – | No | – | – | ○ | ○ | – | – | – | ○ | – | ○ |
| [Thought Purity](https://arxiv.org/abs/2507.12314) | E28 | 2026 | – | 🟦 D3 | 🟦 E3 | LLM only | Implicit | No | No | Yes | ● | ● | – | ● | ● | ○ | ○ | ○ |
| [Unreal Thinking](https://arxiv.org/abs/2604.09235) | E30 | 2026 | 🟦 T1 | 🟦 D3 | 🟦 E3 | LLM only | Implicit | No | No | Yes | ● | ● | ● | ● | ● | ○ | ○ | ○ |
| [Noticing the Watcher](https://arxiv.org/abs/2603.16928) | E31 | 2026 | 🟪 T4 | – | 🟦 E3 | Agent | Implicit | Yes | – | – | ● | ● | – | – | ● | ● | – | ● |
| [SafeAgent](https://arxiv.org/abs/2604.17562) | E32 | 2026 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| [Chain of Attack](https://doi.org/10.18653/v1/2025.findings-acl.514) | E33 | 2025 | 🟩 T3 | – | 🟧 E1 | LLM only | – | Yes | – | – | ○ | ○ | – | – | ○ | ● | – | ○ |
| [CoT-LearnedObfuscation](https://arxiv.org/abs/2601.23086) | E34 | 2026 | 🟪 T4 | – | – | LLM only | Implicit | No | – | – | ● | ● | – | – | – | ○ | – | ○ |
| [AgentArmor](https://arxiv.org/abs/2508.01249) | E35 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| [X-Teaming](https://arxiv.org/abs/2504.13203) | E36 | 2025 | 🟩 T3 | 🟧 D1 | 🟧 E1 | LLM only | – | Yes | Yes | No | ○ | ○ | ○ | ○ | ○ | ● | ● | ○ |
| [ActorBreaker](https://doi.org/10.18653/v1/2025.acl-long.1207) | E37 | 2025 | 🟩 T3 | 🟧 D1 | – | LLM only | – | Yes | Partial | No | ○ | ○ | ○ | ○ | – | ● | ◐ | ○ |
| [CoT Obfuscation](https://arxiv.org/abs/2510.19851) | E38 | 2025 | 🟪 T4 | 🟦 D3 | 🟦 E3 | Agent | Implicit | No | Yes | Yes | ● | ● | ● | ● | ● | ○ | ● | ● |
| [Unsafer in Many Turns](https://arxiv.org/abs/2602.13379) | E39 | 2026 | 🟩 T3 | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | No | ○ | ○ | ○ | ○ | ○ | ○ | ◐ | ● |
| [When CoT Is Necessary](https://arxiv.org/abs/2507.05246) | E40 | 2025 | 🟪 T4 | 🟦 D3 | 🟦 E3 | LLM only | Explicit | No | Yes | Yes | ● | ● | ● | ● | ● | ○ | ● | ○ |
| [Covertly Sandbag](https://doi.org/10.18653/v1/2025.ijcnlp-short.33) | E41 | 2025 | 🟪 T4 | 🟦 D3 | 🟦 E3 | LLM only | Implicit | No | Yes | Yes | ● | ● | ● | ● | ● | ○ | ● | ○ |
| IntentGuard | E42 | 2026 | – | 🟦 D3 | 🟩 E2 | Agent | Implicit | No | Partial | Yes | ● | ● | – | ● | ● | ○ | ◐ | ● |
| [ProbGuard](https://arxiv.org/abs/2508.00500) | E43 | 2026 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| [GuardAgent](https://arxiv.org/abs/2406.09187) | E44 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| [CaMeL](https://arxiv.org/abs/2503.18813) | E45 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| [Psg-Agent](https://arxiv.org/abs/2509.23614) | E46 | 2025 | – | 🟦 D3 | 🟩 E2 | Agent | – | No | No | Yes | ○ | ○ | – | ● | ● | ○ | ○ | ● |
| [AGrail](https://doi.org/10.18653/v1/2025.acl-long.399) | E47 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| [TrustAgent](https://doi.org/10.18653/v1/2024.findings-emnlp.585) | E48 | 2024 | – | 🟦 D3 | 🟩 E2 | Agent | – | No | No | Yes | ○ | ○ | – | ● | ● | ○ | ○ | ● |
| [AgentSentinel](https://doi.org/10.1145/3719027.3765064) | E49 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Yes | No | ○ | ○ | – | ○ | ○ | ○ | ● | ● |
| [IsolateGPT](https://doi.org/10.14722/ndss.2025.241131) | E50 | 2025 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| [PIGuard](https://doi.org/10.18653/v1/2025.acl-long.1468) | E51 | 2025 | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ○ |
| [PISanitizer](https://arxiv.org/abs/2511.10720) | E52 | 2025 | – | 🟧 D1 | 🟧 E1 | Agent | – | No | Yes | No | ○ | ○ | – | ○ | ○ | ○ | ● | ● |
| StruQ | E53 | 2025 | – | 🟧 D1 | 🟧 E1 | LLM only | – | Yes | Yes | No | ○ | ○ | – | ○ | ○ | ● | ● | ○ |
| [Instruction Hierarchy](https://arxiv.org/abs/2404.13208) | E54 | 2025 | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | Partial | No | ○ | ○ | – | ○ | ○ | ○ | ◐ | ○ |
| [PromptArmor](https://arxiv.org/abs/2507.15219) | E55 | 2025 | – | 🟧 D1 | 🟩 E2 | Agent | – | Yes | Yes | No | ○ | ○ | – | ○ | ○ | ● | ● | ● |
| SecAlign | E56 | 2025 | – | 🟧 D1 | 🟧 E1 | Mixed | – | Yes | Yes | No | ○ | ○ | – | ○ | ○ | ● | ● | ● |
| [Tool Result Parsing](https://arxiv.org/abs/2601.04795) | E57 | 2026 | – | 🟧 D1 | 🟩 E2 | Agent | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| [PromptShield](https://doi.org/10.1145/3714393.3726501) | E59 | 2025 | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ○ |
| [AgentVisor](https://arxiv.org/abs/2604.24118) | E60 | 2026 | – | 🟩 D2 | 🟩 E2 | Agent | – | Yes | Yes | No | ○ | ○ | – | ○ | ○ | ● | ● | ● |
| [ICON](https://arxiv.org/abs/2602.20708) | E61 | 2026 | – | 🟦 D3 | 🟩 E2 | Agent | Implicit | No | Partial | Yes | ● | ● | – | ● | ● | ○ | ◐ | ● |
| [MonitorBench](https://arxiv.org/abs/2603.28590) | E62 | 2026 | – | – | 🟦 E3 | Mixed | Implicit | Yes | – | – | ● | ● | – | – | ● | ● | – | ● |
| [AutoMonitor-Bench](https://arxiv.org/abs/2601.05752) | E63 | 2026 | – | – | 🟦 E3 | LLM only | Implicit | No | – | – | ● | ● | – | – | ● | ○ | – | ○ |
| [BONA FIDE](https://arxiv.org/abs/2605.25052) | E64 | 2026 | – | – | 🟦 E3 | LLM only | Explicit | No | – | – | ● | ● | – | – | ● | ○ | – | ○ |
| [CoT Faithfulness Audit](https://arxiv.org/abs/2505.05410) | E65 | 2025 | – | – | 🟦 E3 | LLM only | Implicit | No | – | – | ● | ● | – | – | ● | ○ | – | ○ |
| [C2-Faith](https://arxiv.org/abs/2603.05167) | E66 | 2026 | – | – | 🟦 E3 | LLM only | Explicit | No | – | – | ● | ● | – | – | ○ | ○ | – | ○ |
| ASB | E67 | 2025 | – | – | 🟩 E2 | Agent | – | No | – | – | ● | ○ | – | – | ○ | ○ | – | ● |
| [H-CoT](https://arxiv.org/abs/2502.12893) | E68 | 2025 | 🟦 T1 | – | 🟧 E1 | LLM only | – | No | – | – | ● | ○ | – | – | ○ | ○ | – | ○ |
| [AgentPoison](https://arxiv.org/abs/2407.12784) | E69 | 2024 | 🟧 T2 | – | 🟩 E2 | Agent | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| [PoisonedRAG](https://arxiv.org/abs/2402.07867) | E70 | 2025 | 🟧 T2 | – | 🟧 E1 | Mixed | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| AgentHarm | E71 | 2025 | – | – | 🟩 E2 | Agent | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| [WASP](https://arxiv.org/abs/2504.18575) | E72 | 2025 | – | – | 🟩 E2 | Agent | Implicit | No | – | – | ● | ● | – | – | ○ | ○ | – | ● |
| [MINJA](https://proceedings.neurips.cc/paper_files/paper/2025/hash/42a97bbd9844d2bf68596730af80bcdf-Abstract-Conference.html) | E73 | 2025 | 🟧 T2 | – | 🟦 E3 | Agent | Implicit | No | – | – | ● | ● | – | – | ○ | ○ | – | ● |
| [InjecAgent](https://arxiv.org/abs/2403.02691) | E74 | 2024 | – | – | 🟩 E2 | Agent | – | No | – | – | ● | ○ | – | – | ○ | ○ | – | ● |
| [SHADE-Arena](https://arxiv.org/abs/2506.15740) | E75 | 2025 | – | – | 🟦 E3 | Agent | Implicit | No | – | – | ● | ● | – | – | ● | ○ | – | ● |
| [Agent-Safetybench](https://arxiv.org/abs/2412.14470) | E76 | 2025 | – | – | 🟩 E2 | Agent | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| [AgentDyn](https://arxiv.org/abs/2602.03117) | E77 | 2026 | – | – | 🟩 E2 | Agent | – | No | – | – | ○ | ○ | – | – | ○ | ○ | – | ● |
