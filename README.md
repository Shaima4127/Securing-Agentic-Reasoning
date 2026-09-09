# Securing Agentic Reasoning

**A Survey of Threats, Defenses, and Evaluation for AI Agents**

Companion repository for the survey. It publishes the five annotation tables behind
the paper so that every classification and gap flag reported in the manuscript can be
inspected, sorted, and reused.

**Authors:** Shaima Ahmad Freja, Ferhat Ozgur Catak, Chunming Rong
**Affiliation:** Department of Electrical Engineering and Computer Science, University of Stavanger, Norway
**Paper:** [link to be added]

---

## Overview

Large language model agents increasingly serve as the reasoning core of autonomous
systems — planning across multiple steps, invoking tools, processing external content,
and maintaining memory as they act. That shift from single-turn inference to a
persistent reasoning–action loop expands the attack surface well beyond conventional
input–output robustness.

This survey uses **reasoning-layer security** as the organizing lens connecting
threats, defenses, and evaluation. From a structured review of 89 papers published
between 2024 and 2026, it develops three complementary taxonomies over an annotated
set of 71 empirical studies:

- a **threat** taxonomy of how adversaries corrupt, hijack, or obscure reasoning
- a **defense** taxonomy of where mitigations intervene in the agent pipeline
- an **evaluation** taxonomy of which evidence layer an experiment observes — boundary
  inputs and responses, execution trajectories, or reasoning processes

Synthesizing across the three, defenses and evaluations remain concentrated at the
input–output boundary and execution layers, while reasoning-aware mechanisms,
adaptive-adversary testing, and validated reasoning-integrity measurement remain
limited.

---

## Tables

| Table | Contents | Rows |
|---|---|---|
| [Threat taxonomy](docs/threat-taxonomy.md) | T1–T4, attack class, vector, target, structure, gap flags | 31 |
| [Defense taxonomy](docs/defense-taxonomy.md) | D1–D3, sub-cluster, defense pattern, reasoning-awareness, gap flags | 37 |
| [Evaluation taxonomy](docs/evaluation-taxonomy.md) | E1–E3, subgroup, benchmark, adaptive adversary, RIM, gap flags | 64 |
| [Annotation matrix](docs/annotation-matrix.md) | Per-paper coded values across all three taxonomies | 71 |
| [Benchmark inventory](docs/benchmark-inventory.md) | Security evaluation instruments with scope, adversary model, metrics | 26 |

Each table is also available as CSV in [`data/`](data/) for direct reuse.

---

## Taxonomies

**Threats (T1–T4)**

| | Cluster | Papers |
|---|---|---|
| T1 | Reasoning manipulation and backdoors | 9 |
| T2 | Indirect injection and tool-chain attacks | 10 |
| T3 | Adaptive and multi-turn attacks | 7 |
| T4 | Monitoring evasion and obfuscation | 5 |

**Defenses (D1–D3)**

| | Cluster | Papers |
|---|---|---|
| D1 | *cluster name* | 12 |
| D2 | *cluster name* | 12 |
| D3 | *cluster name* | 13 |

**Evaluation (E1–E3)**

| | Cluster | Papers |
|---|---|---|
| E1 | *cluster name* | 14 |
| E2 | *cluster name* | 33 |
| E3 | *cluster name* | 17 |

---

## Gap framework

Five cross-cutting gaps are flagged per paper in every table:

| Flag | Gap |
|---|---|
| **G1** | Reasoning observability |
| **G2** | Reasoning integrity metric |
| **G3** | Reasoning-layer defense capability |
| **G4** | Adaptive robustness |
| **G5** | Agentic evaluation scope |

Flag values: `●` addressed · `◐` partial · `○` present · `—` not applicable

---

## Selected findings

- **0 of 64** evaluation papers combine explicit reasoning-integrity measurement,
  an adaptive adversary, and agentic scope.
- **16 of 64** evaluation papers test against an adaptive adversary; **12** of those
  also operate at agentic scope.
- Of 26 catalogued benchmarks, evaluation converges on four instruments, none of which
  carries a reasoning-integrity metric.

---

## Citation

```bibtex
@article{freja2026securing,
  title   = {Securing Agentic Reasoning: A Survey of Threats, Defenses, and Evaluation for AI Agents},
  author  = {Freja, Shaima Ahmad and Catak, Ferhat Ozgur and Rong, Chunming},
  journal = {International Journal of Information Security},
  year    = {2026}
}
```

---

## Contact

Shaima Ahmad Freja — shaima.a.freja@uis.no
