# Securing Agentic Reasoning

**A Survey of Threats, Defenses, and Evaluation Frameworks for AI Agents**

<!-- Add a paper badge once a preprint or DOI exists, e.g.
[![Paper](https://img.shields.io/badge/paper-arXiv-b31b1b?style=flat-square)](https://arxiv.org/abs/XXXX.XXXXX)
-->
[![License](https://img.shields.io/badge/license-CC%20BY%204.0-blue?style=flat-square)](LICENSE)
![Papers](https://img.shields.io/badge/annotated%20papers-71-555?style=flat-square)
![Benchmarks](https://img.shields.io/badge/benchmarks-26-555?style=flat-square)

Currently under peer review.

Shaima Ahmad Freja, Ferhat Ozgur Catak, Chunming Rong — University of Stavanger, Norway

This repository is the annotation record behind the survey: every paper's cluster assignment, gap coding, and benchmark properties, in the same form the paper reports them.

---

## The argument in one paragraph

Security work on LLM-based agents is overwhelmingly **boundary-focused** — it inspects inputs, outputs, tool calls, and permissions. Much less of it reaches the **reasoning layer**, where chain-of-thought, ReAct, Reflexion, and multi-step planning actually form an agent's decisions. This survey measures that asymmetry paper by paper rather than asserting it, using three coupled taxonomies and one shared gap framework applied to all 71 papers.

![Roadmap of the survey](figures/roadmap.png)

*Roadmap of the survey. Cluster colours indicate the agent layer a cluster concerns: boundary, execution, and reasoning. T3 is defined by the temporal structure of an attack rather than by a single layer, so it retains the threat colour of §4.*

## Start here

| Document | What's in it |
|---|---|
| [Threat taxonomy](docs/threat-taxonomy.md) | 31 papers, T1–T4, grouped by attack class |
| [Defense taxonomy](docs/defense-taxonomy.md) | 37 papers, D1–D3, grouped by sub-cluster |
| [Evaluation taxonomy](docs/evaluation-taxonomy.md) | 64 papers, E1–E3, grouped by subgroup |
| [Paper matrix](docs/annotation-matrix.md) | All 71 papers against every coded column |
| [Benchmark inventory](docs/benchmark-inventory.md) | 26 evaluation instruments and their properties |

Every paper is listed by the short name used in the manuscript and linked to its publication.

## Taxonomies

Colour marks the security layer a cluster targets.

**Threats** — 31 papers

| | Cluster | Papers |
|---|---|---|
| 🟦 T1 | Reasoning manipulation and backdoors | 9 |
| 🟧 T2 | Indirect prompt injection and tool-chain attacks | 10 |
| 🟩 T3 | Adaptive and multi-turn attacks | 7 |
| 🟪 T4 | Monitoring evasion and obfuscation | 5 |

**Defenses** — 37 papers

| | Cluster | Papers |
|---|---|---|
| 🟦 D1 | Boundary filtering and guardrails | 12 |
| 🟧 D2 | Runtime agent monitoring and execution control | 12 |
| 🟩 D3 | Reasoning-aware process defenses | 13 |

**Evaluation** — 64 papers

| | Cluster | Papers |
|---|---|---|
| 🟦 E1 | Boundary robustness evaluation | 14 |
| 🟧 E2 | Agent execution and trajectory safety evaluation | 33 |
| 🟩 E3 | Reasoning-process integrity and monitorability evaluation | 17 |

Papers can carry assignments in more than one taxonomy, so these counts overlap and do not sum to 71.

## The gap framework

Five dimensions, coded for every paper. This is what makes the three taxonomies comparable to one another.

| | Gap | Question it asks |
|---|---|---|
| **G1** | Reasoning observability | Is the reasoning process visible to the defense or evaluation at all? |
| **G2** | Reasoning integrity metric | Is there a measure of whether that reasoning is sound? |
| **G3** | Defense capability | Does the defense act on reasoning, or only at the boundary? |
| **G4** | Adaptive robustness | Does it hold against an adversary that adapts? |
| **G5** | Agentic scope | Is it evaluated on real agents, or single-turn prompts? |

Flags render as ● addressed · ◐ partially addressed · ○ present · – not applicable, matching the paper. `PARTIAL` is admissible only in G3 (D) and G4 (D). G1 and G2 are independent: observing a reasoning trace and measuring its integrity are separate capabilities.

## Headline result

**No evaluation in the corpus closes all three reasoning-relevant gaps at once.**

Of the 64 evaluation papers, none simultaneously reports an explicit reasoning integrity metric, evaluates against an adaptive adversary, and operates at agentic scope.

| Condition | Papers (of 64) |
|---|---|
| Explicit reasoning integrity metric | 3 |
| Adaptive adversary | 16 |
| Agentic scope | 44 |
| Adaptive **and** agentic | 12 |
| Explicit RIM **and** agentic | 0 |
| Explicit RIM **and** adaptive | 0 |
| **All three** | **0** |

The emptiness is not marginal. Both pairwise intersections involving an explicit RIM are also zero: all three explicit-RIM papers are non-agentic *and* non-adaptive. Full breakdown in the [evaluation taxonomy](docs/evaluation-taxonomy.md).

## Corpus

| | Count |
|---|---|
| Screened and recorded | 89 |
| Annotated empirical corpus | 71 |
| Distinct evaluation instruments | 26 |

Publication window 2024–2026. Papers were annotated against a frozen codebook; the free-text limitation fields in the source records are descriptive only and never the basis for a coded flag.

## Repository layout

```
.
├── README.md
├── LICENSE
├── figures/
│   └── roadmap.png
└── docs/
    ├── threat-taxonomy.md
    ├── defense-taxonomy.md
    ├── evaluation-taxonomy.md
    ├── annotation-matrix.md
    └── benchmark-inventory.md
```

The documents here are generated from the project's annotation workbooks and carry a do-not-edit banner. The workbooks themselves are not published; researchers wanting them can contact the authors.

## Citation

```bibtex
@misc{freja2026securing,
  title  = {Securing Agentic Reasoning: A Survey of Threats, Defenses,
            and Evaluation Frameworks for AI Agents},
  author = {Freja, Shaima Ahmad and Catak, Ferhat Ozgur and Rong, Chunming},
  year   = {2026},
  note   = {Under review}
}
```

## License

[CC BY 4.0](LICENSE). You may share and adapt this material, including commercially, with attribution.

Cited papers remain under their own copyright; this repository links to them but does not reproduce them.

## Contact

<!-- TODO: corresponding author email, University of Stavanger -->
