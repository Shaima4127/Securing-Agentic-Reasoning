<!-- Generated from the project's annotation workbooks. Do not edit by hand. -->

# Annotation matrix

The full per-paper annotation matrix: 71 papers × 23 columns. This is the artifact the manuscript refers to as the accompanying repository annotation matrix, and it is the record from which every count in the paper is computed.

A paper may carry a threat, defense, and/or evaluation cluster assignment, so the three taxonomy counts overlap and do not sum to 71. Blank cluster cells mean the paper was not routed to that taxonomy; `N/A` in a coded column means the dimension does not apply to that paper's contribution type.

Papers are identified by short name, as used in the manuscript. The `ID` column is retained only as a join key against the CSV exports and the source workbooks.

## Coded vocabulary

| Column | Admissible values |
|---|---|
| Publication status | `Peer-reviewed journal` / `Peer-reviewed conference` / `Peer-reviewed workshop` / `Preprint` / `Technical report` / `Other non-peer-reviewed` |
| Scope level | `LLM-only` / `Agent` / `Multi-Agent` / `Mixed` (rendered below as LLM only / Agent / Multi-agent / Mixed) |
| Adaptive adversary (AA) | `Y` / `N` / `N/A` |
| Reasoning integrity metric (RIM) | `Explicit` / `Implicit` / `N/A` |
| Adaptive robustness eval (ARE) | `Y` / `Partial` / `N` |
| G1, G2, G5 | `ADDRESSED` / `PRESENT` / `N/A` |
| G3 (D), G4 (D) | `ADDRESSED` / `PARTIAL` / `PRESENT` / `N/A` |
| G3 (T), G3 (E), G4 (T/E) | `ADDRESSED` / `PRESENT` / `N/A` |
| Gap flags, as rendered below | ● addressed  ·  ◐ partially addressed  ·  ○ present  ·  – not applicable |

Publication status is assigned from the venue of record, not from the BibTeX entry type, because entry types are inconsistent for the same venue. `Technical report` requires a citable institutional artifact distinct from the arXiv paper (report number, named series, system card); institutional affiliation alone is not sufficient, and no paper in this corpus met that test, so the level is defined but unpopulated. `Preprint` means arXiv is the venue of record and no distinct institutional report was identified. Benchmark is deliberately *not* a publication-status value: a benchmark paper may itself be peer reviewed, and contribution type is recorded separately. All 71 papers were checked individually in October 2026; 30 were confirmed from the venue already recorded in the bibliography and 41 were verified against external indexes (ACL Anthology, IEEE Xplore, DBLP, OpenReview, and the ICML/ICLR proceedings sites).

Scope level: `Agent` when all evaluated settings are agentic and involve a single agent; `Multi-Agent` when all evaluated settings are agentic and at least one involves multiple interacting agents; `Mixed` when the paper empirically evaluates both standalone LLM settings and agentic ones; `LLM-only` when no evaluated setting is agentic. A setting counts as agentic only on evidence of tool use, persistent memory, environment interaction, action execution, or autonomous iterative planning, supported by a reported evaluation in an identifiable agentic experimental setting; long-context prompting, ordinary multi-turn conversation, or describing a system as agentic does not qualify on its own. G5 is read from this field: `Agent`, `Multi-Agent`, and `Mixed` → `ADDRESSED`; `LLM-only` → `PRESENT`.

Free-text `Gap / Limitation` fields in the source workbooks are descriptive only and are never the basis for a coded flag.

## Paper matrix

● addressed  ·  ◐ partially addressed  ·  ○ present  ·  – not applicable

| ID | Short name | Yr | Publication status | Venue | T | D | E | Scope | RIM | AA | ARE | G1 | G2 | G3(T) | G3(D) | G3(E) | G4(T/E) | G4(D) | G5 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| E01 | [Attacker Moves Second](https://arxiv.org/abs/2510.09023) | 2025 | Peer-reviewed conference | USENIX Security Symposium 2026 | 🟩 T3 | – | 🟧 E1 | Mixed | – | Yes | – | ○ | ○ | – | – | ○ | ● | – | ● |
| E02 | [AgentMonitor](https://arxiv.org/abs/2408.14972) | 2024 | Preprint | arXiv:2408.14972 | – | 🟩 D2 | 🟩 E2 | Multi-agent | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| E05 | [JailGuard](https://doi.org/10.1145/3724393) | 2025 | Peer-reviewed journal | ACM Transactions on Software Engineering and Methodology | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ○ |
| E07 | [AgentDoG](https://arxiv.org/abs/2601.18491) | 2026 | Preprint | arXiv:2601.18491 | – | 🟦 D3 | 🟩 E2 | Agent | Implicit | No | Partial | ● | ● | – | ● | ○ | ○ | ◐ | ● |
| E08 | [RTBAS](https://arxiv.org/abs/2502.08966) | 2025 | Preprint | arXiv:2502.08966 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| E09 | [AgentDojo](https://arxiv.org/abs/2406.13352) | 2024 | Peer-reviewed conference | Advances in Neural Information Processing Systems 37 (NeurIPS 2024) Datasets and Benchmarks Track | – | – | 🟩 E2 | Agent | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| E10 | [ReasoningBomb](https://arxiv.org/abs/2602.00154) | 2026 | Preprint | arXiv:2602.00154 | 🟦 T1 | – | 🟦 E3 | LLM only | Implicit | No | – | ● | ● | – | – | ○ | ○ | – | ○ |
| E11 | [UDora](https://arxiv.org/abs/2503.01908) | 2025 | Peer-reviewed conference | Proceedings of the 42nd International Conference on Machine Learning (ICML) | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | ● | ○ | – | – | ○ | ● | – | ● |
| E12 | [Automated Prompt Injection](https://arxiv.org/abs/2606.10525) | 2026 | Preprint | arXiv (no identifier recorded) | 🟧 T2 | – | 🟩 E2 | Agent | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| E13 | [SIRAJ](https://doi.org/10.18653/v1/2026.findings-eacl.171) | 2026 | Peer-reviewed conference | Findings of the Association for Computational Linguistics: EACL 2026 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | ○ | ○ | – | – | ○ | ● | – | ● |
| E14 | [Dark Side of LLMs](https://arxiv.org/abs/2507.06850) | 2025 | Preprint | arXiv:2507.06850 | 🟧 T2 | – | – | Multi-agent | – | No | – | ○ | ○ | – | – | – | ○ | – | ● |
| E15 | [AgentVigil](https://arxiv.org/abs/2505.05849) | 2025 | Peer-reviewed conference | Findings of EMNLP 2025 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | ○ | ○ | – | – | ○ | ● | – | ● |
| E16 | [CoT Hijacking](https://arxiv.org/abs/2510.26418) | 2026 | Preprint | arXiv:2510.26418 | 🟦 T1 | – | 🟦 E3 | LLM only | Implicit | Yes | – | ● | ● | – | – | ○ | ● | – | ○ |
| E17 | [STAC](https://arxiv.org/abs/2509.25624) | 2026 | Preprint | arXiv:2509.25624 | 🟩 T3 | 🟦 D3 | – | Agent | – | Yes | Yes | ○ | ○ | ◐ | ◐ | – | ● | ● | ● |
| E18 | [ShadowCoT](https://arxiv.org/abs/2504.05605) | 2025 | Peer-reviewed journal | IEEE Trans. Information Forensics and Security 21 (2026) | 🟦 T1 | – | – | LLM only | Implicit | No | – | ● | ● | – | – | – | ○ | – | ○ |
| E20 | [DarkMind](https://arxiv.org/abs/2501.18617) | 2025 | Preprint | arXiv:2501.18617 | 🟦 T1 | – | 🟧 E1 | LLM only | Implicit | No | – | ● | ● | – | – | ○ | ○ | – | ○ |
| E21 | [Adaptive Attacks](https://doi.org/10.18653/v1/2025.findings-naacl.395) | 2025 | Peer-reviewed conference | Findings of the Association for Computational Linguistics: NAACL 2025 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | ○ | ○ | – | – | ○ | ● | – | ● |
| E22 | [AdapTools](https://arxiv.org/abs/2602.20720) | 2026 | Preprint | arXiv:2602.20720 | 🟧 T2 | – | 🟩 E2 | Agent | – | Yes | – | ○ | ○ | – | – | ○ | ● | – | ● |
| E23 | [Reasoning-Style Poisoning](https://arxiv.org/abs/2512.14448) | 2026 | Preprint | arXiv:2512.14448 | 🟦 T1 | 🟦 D3 | 🟦 E3 | Agent | Implicit | No | No | ● | ● | ● | ● | ● | ○ | ○ | ● |
| E24 | [BadChain](https://arxiv.org/abs/2401.12242) | 2024 | Peer-reviewed conference | International Conference on Learning Representations (ICLR) | 🟦 T1 | 🟧 D1 | 🟧 E1 | LLM only | Implicit | No | No | ● | ● | ◐ | ◐ | ○ | ○ | ○ | ○ |
| E25 | [Auto-RT](https://arxiv.org/abs/2501.01830) | 2025 | Preprint | arXiv:2501.01830 | 🟩 T3 | – | – | LLM only | – | Yes | – | ○ | ○ | – | – | – | ● | – | ○ |
| E26 | [Monitoring Reasoning Models](https://arxiv.org/abs/2503.11926) | 2025 | Preprint | arXiv:2503.11926 | – | 🟦 D3 | 🟦 E3 | Agent | Implicit | Yes | Yes | ● | ● | – | ● | ● | ● | ● | ● |
| E27 | [Thought-Transfer](https://arxiv.org/abs/2601.19061) | 2026 | Preprint | arXiv:2601.19061 | 🟦 T1 | – | – | LLM only | – | No | – | ○ | ○ | – | – | – | ○ | – | ○ |
| E28 | [Thought Purity](https://arxiv.org/abs/2507.12314) | 2026 | Preprint | arXiv:2507.12314 | – | 🟦 D3 | 🟦 E3 | LLM only | Implicit | No | No | ● | ● | – | ● | ● | ○ | ○ | ○ |
| E30 | [Unreal Thinking](https://arxiv.org/abs/2604.09235) | 2026 | Preprint | arXiv:2604.09235 | 🟦 T1 | 🟦 D3 | 🟦 E3 | LLM only | Implicit | No | No | ● | ● | ● | ● | ● | ○ | ○ | ○ |
| E31 | [Noticing the Watcher](https://arxiv.org/abs/2603.16928) | 2026 | Preprint | arXiv:2603.16928 | 🟪 T4 | – | 🟦 E3 | Agent | Implicit | Yes | – | ● | ● | – | – | ● | ● | – | ● |
| E32 | [SafeAgent](https://arxiv.org/abs/2604.17562) | 2026 | Preprint | arXiv:2604.17562 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| E33 | [Chain of Attack](https://doi.org/10.18653/v1/2025.findings-acl.514) | 2025 | Peer-reviewed conference | Findings of the Association for Computational Linguistics: ACL 2025 | 🟩 T3 | – | 🟧 E1 | LLM only | – | Yes | – | ○ | ○ | – | – | ○ | ● | – | ○ |
| E34 | [CoT-LearnedObfuscation](https://arxiv.org/abs/2601.23086) | 2026 | Preprint | arXiv:2601.23086 | 🟪 T4 | – | – | LLM only | Implicit | No | – | ● | ● | – | – | – | ○ | – | ○ |
| E35 | [AgentArmor](https://arxiv.org/abs/2508.01249) | 2025 | Preprint | arXiv:2508.01249 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| E36 | [X-Teaming](https://arxiv.org/abs/2504.13203) | 2025 | Preprint | arXiv:2504.13203 | 🟩 T3 | 🟧 D1 | 🟧 E1 | LLM only | – | Yes | Yes | ○ | ○ | ○ | ○ | ○ | ● | ● | ○ |
| E37 | [ActorBreaker](https://doi.org/10.18653/v1/2025.acl-long.1207) | 2025 | Peer-reviewed conference | Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) | 🟩 T3 | 🟧 D1 | – | LLM only | – | Yes | Partial | ○ | ○ | ○ | ○ | – | ● | ◐ | ○ |
| E38 | [CoT Obfuscation](https://arxiv.org/abs/2510.19851) | 2025 | Preprint | arXiv:2510.19851 | 🟪 T4 | 🟦 D3 | 🟦 E3 | Agent | Implicit | No | Yes | ● | ● | ● | ● | ● | ○ | ● | ● |
| E39 | [Unsafer in Many Turns](https://arxiv.org/abs/2602.13379) | 2026 | Peer-reviewed conference | ICML 2026 | 🟩 T3 | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | ○ | ○ | ○ | ○ | ○ | ○ | ◐ | ● |
| E40 | [When CoT Is Necessary](https://arxiv.org/abs/2507.05246) | 2025 | Preprint | arXiv:2507.05246 | 🟪 T4 | 🟦 D3 | 🟦 E3 | LLM only | Explicit | No | Yes | ● | ● | ● | ● | ● | ○ | ● | ○ |
| E41 | [Covertly Sandbag](https://doi.org/10.18653/v1/2025.ijcnlp-short.33) | 2025 | Peer-reviewed conference | Proceedings of the 14th International Joint Conference on Natural Language Processing and the 4th Conference of the Asia-Pacific Chapter of the Association for Computational Linguistics | 🟪 T4 | 🟦 D3 | 🟦 E3 | LLM only | Implicit | No | Yes | ● | ● | ● | ● | ● | ○ | ● | ○ |
| E42 | [IntentGuard](https://openreview.net/forum?id=kabNlhXQkT) | 2026 | Peer-reviewed workshop | AAAI 2026 Workshop on Trustworthy Agentic AI | – | 🟦 D3 | 🟩 E2 | Agent | Implicit | No | Partial | ● | ● | – | ● | ● | ○ | ◐ | ● |
| E43 | [ProbGuard](https://arxiv.org/abs/2508.00500) | 2026 | Preprint | arXiv:2508.00500 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| E44 | [GuardAgent](https://arxiv.org/abs/2406.09187) | 2025 | Peer-reviewed conference | Proceedings of the 42nd International Conference on Machine Learning (ICML) | – | 🟩 D2 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| E45 | [CaMeL](https://arxiv.org/abs/2503.18813) | 2025 | Peer-reviewed conference | IEEE SaTML 2026 | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| E46 | [Psg-Agent](https://arxiv.org/abs/2509.23614) | 2025 | Preprint | arXiv:2509.23614 | – | 🟦 D3 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ● | ● | ○ | ○ | ● |
| E47 | [AGrail](https://doi.org/10.18653/v1/2025.acl-long.399) | 2025 | Peer-reviewed conference | Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| E48 | [TrustAgent](https://doi.org/10.18653/v1/2024.findings-emnlp.585) | 2024 | Peer-reviewed conference | Findings of the Association for Computational Linguistics: EMNLP 2024 | – | 🟦 D3 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ● | ● | ○ | ○ | ● |
| E49 | [AgentSentinel](https://doi.org/10.1145/3719027.3765064) | 2025 | Peer-reviewed conference | Proceedings of the 2025 ACM SIGSAC Conference on Computer and Communications Security (CCS '25) | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Yes | ○ | ○ | – | ○ | ○ | ○ | ● | ● |
| E50 | [IsolateGPT](https://doi.org/10.14722/ndss.2025.241131) | 2025 | Peer-reviewed conference | Network and Distributed System Security (NDSS) Symposium | – | 🟩 D2 | 🟩 E2 | Agent | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| E51 | [PIGuard](https://doi.org/10.18653/v1/2025.acl-long.1468) | 2025 | Peer-reviewed conference | Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ○ |
| E52 | [PISanitizer](https://arxiv.org/abs/2511.10720) | 2025 | Preprint | arXiv:2511.10720 | – | 🟧 D1 | 🟧 E1 | Mixed | – | No | Yes | ○ | ○ | – | ○ | ○ | ○ | ● | ● |
| E53 | [StruQ](https://www.usenix.org/conference/usenixsecurity25/presentation/chen-sizhe) | 2025 | Peer-reviewed conference | 34th USENIX Security Symposium (USENIX Security 25) | – | 🟧 D1 | 🟧 E1 | LLM only | – | Yes | Yes | ○ | ○ | – | ○ | ○ | ● | ● | ○ |
| E54 | [Instruction Hierarchy](https://arxiv.org/abs/2404.13208) | 2025 | Preprint | arXiv:2404.13208 | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ○ |
| E55 | [PromptArmor](https://arxiv.org/abs/2507.15219) | 2025 | Preprint | arXiv:2507.15219 | – | 🟧 D1 | 🟩 E2 | Agent | – | Yes | Yes | ○ | ○ | – | ○ | ○ | ● | ● | ● |
| E56 | [SecAlign](https://doi.org/10.1145/3719027.3744836) | 2025 | Peer-reviewed conference | Proceedings of the 2025 ACM SIGSAC Conference on Computer and Communications Security | – | 🟧 D1 | 🟧 E1 | Mixed | – | No | Partial | ○ | ○ | – | ○ | ○ | ○ | ◐ | ● |
| E57 | [Tool Result Parsing](https://arxiv.org/abs/2601.04795) | 2026 | Preprint | arXiv:2601.04795 | – | 🟧 D1 | 🟩 E2 | Agent | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ● |
| E59 | [PromptShield](https://doi.org/10.1145/3714393.3726501) | 2025 | Peer-reviewed conference | Proceedings of the Fifteenth ACM Conference on Data and Application Security and Privacy (CODASPY '25) | – | 🟧 D1 | 🟧 E1 | LLM only | – | No | No | ○ | ○ | – | ○ | ○ | ○ | ○ | ○ |
| E60 | [AgentVisor](https://arxiv.org/abs/2604.24118) | 2026 | Preprint | arXiv:2604.24118 | – | 🟩 D2 | 🟩 E2 | Agent | – | Yes | Yes | ○ | ○ | – | ○ | ○ | ● | ● | ● |
| E61 | [ICON](https://arxiv.org/abs/2602.20708) | 2026 | Preprint | arXiv:2602.20708 | – | 🟦 D3 | 🟩 E2 | Agent | Implicit | No | Partial | ● | ● | – | ● | ● | ○ | ◐ | ● |
| E62 | [MonitorBench](https://arxiv.org/abs/2603.28590) | 2026 | Preprint | arXiv:2603.28590 | – | – | 🟦 E3 | Mixed | Implicit | Yes | – | ● | ● | – | – | ● | ● | – | ● |
| E63 | [AutoMonitor-Bench](https://arxiv.org/abs/2601.05752) | 2026 | Peer-reviewed conference | Findings of ACL 2026 | – | – | 🟦 E3 | LLM only | Implicit | No | – | ● | ● | – | – | ● | ○ | – | ○ |
| E64 | [BONA FIDE](https://arxiv.org/abs/2605.25052) | 2026 | Preprint | arXiv:2605.25052 | – | – | 🟦 E3 | LLM only | Explicit | No | – | ● | ● | – | – | ● | ○ | – | ○ |
| E65 | [CoT Faithfulness Audit](https://arxiv.org/abs/2505.05410) | 2025 | Preprint | arXiv:2505.05410 | – | – | 🟦 E3 | LLM only | Implicit | No | – | ● | ● | – | – | ● | ○ | – | ○ |
| E66 | [C2-Faith](https://arxiv.org/abs/2603.05167) | 2026 | Peer-reviewed workshop | GEM Workshop 2026 (ACL) | – | – | 🟦 E3 | LLM only | Explicit | No | – | ● | ● | – | – | ○ | ○ | – | ○ |
| E67 | [ASB](https://proceedings.iclr.cc/paper_files/paper/2025/hash/5750f91d8fb9d5c02bd8ad2c3b44456b-Abstract-Conference.html) | 2025 | Peer-reviewed conference | International Conference on Learning Representations | – | – | 🟩 E2 | Agent | – | No | – | ● | ○ | – | – | ○ | ○ | – | ● |
| E68 | [H-CoT](https://arxiv.org/abs/2502.12893) | 2025 | Preprint | arXiv:2502.12893 | 🟦 T1 | – | 🟧 E1 | LLM only | – | No | – | ● | ○ | – | – | ○ | ○ | – | ○ |
| E69 | [AgentPoison](https://arxiv.org/abs/2407.12784) | 2024 | Peer-reviewed conference | Advances in Neural Information Processing Systems | 🟧 T2 | – | 🟩 E2 | Agent | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| E70 | [PoisonedRAG](https://arxiv.org/abs/2402.07867) | 2025 | Peer-reviewed conference | Proc. 34th USENIX Security Symposium | 🟧 T2 | – | 🟧 E1 | Mixed | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| E71 | [AgentHarm](https://proceedings.iclr.cc/paper_files/paper/2025/hash/c493d23af93118975cdbc32cbe7323f5-Abstract-Conference.html) | 2025 | Peer-reviewed conference | International Conference on Learning Representations | – | – | 🟩 E2 | Agent | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| E72 | [WASP](https://arxiv.org/abs/2504.18575) | 2025 | Peer-reviewed conference | Advances in Neural Information Processing Systems 38 (NeurIPS 2025) Datasets and Benchmarks Track | – | – | 🟩 E2 | Agent | Implicit | No | – | ● | ● | – | – | ○ | ○ | – | ● |
| E73 | [MINJA](https://proceedings.neurips.cc/paper_files/paper/2025/hash/42a97bbd9844d2bf68596730af80bcdf-Abstract-Conference.html) | 2025 | Peer-reviewed conference | NeurIPS 2025 (Main Conference Track) | 🟧 T2 | – | 🟦 E3 | Agent | Implicit | No | – | ● | ● | – | – | ○ | ○ | – | ● |
| E74 | [InjecAgent](https://arxiv.org/abs/2403.02691) | 2024 | Peer-reviewed conference | Findings of the Association for Computational Linguistics: ACL 2024 | – | – | 🟩 E2 | Agent | – | No | – | ● | ○ | – | – | ○ | ○ | – | ● |
| E75 | [SHADE-Arena](https://arxiv.org/abs/2506.15740) | 2025 | Preprint | arXiv:2506.15740 | – | – | 🟦 E3 | Agent | Implicit | No | – | ● | ● | – | – | ● | ○ | – | ● |
| E76 | [Agent-Safetybench](https://arxiv.org/abs/2412.14470) | 2025 | Preprint | arXiv:2412.14470 | – | – | 🟩 E2 | Agent | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
| E77 | [AgentDyn](https://arxiv.org/abs/2602.03117) | 2026 | Preprint | arXiv:2602.03117 | – | – | 🟩 E2 | Agent | – | No | – | ○ | ○ | – | – | ○ | ○ | – | ● |
