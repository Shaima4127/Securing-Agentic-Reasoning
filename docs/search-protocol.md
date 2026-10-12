# Search and Screening Protocol

Companion document to *Securing Agentic Reasoning: A Survey of Threats, Defenses,
and Evaluation for AI Agents* (International Journal of Information Security).
It records the search queries and selection procedure summarised in Section 3.1
and Figure 2. The review followed a structured search and screening process; it
does not claim conformance with PRISMA.

## 1. Initial search

Four databases, covering work published 2024–2026, searched iteratively between
February and June 2026. A broad scoping search of approximately 11,645 records
preceded it and was used only for query calibration, not for selection.

| Database | Search query | Records |
|---|---|---|
| Web of Science | `"Agentic AI Security"` | 92 |
| ScienceDirect | `("Agentic AI" OR "LLM agents") AND ("security" OR "threats" OR "defense" OR "evaluation")` | 98 |
| Semantic Scholar | `("Agentic AI Security" OR "Security of Autonomous LLM Agents" OR "Agentic reasoning")` | 199 |
| Google Scholar | `("Agentic AI Security" OR "Security of Autonomous LLM Agents" OR "Agentic reasoning")` | ~180 |
| **Total** | | **~569** |

Semantic Scholar results include arXiv-indexed papers. Google Scholar reports
rounded estimates that vary between sessions. The ScienceDirect query was
recorded as a comma-separated keyword string and is shown here in Boolean form.
Database-specific filter settings were not fully preserved, and the reported
counts have not been re-executed using these expressions.

## 2. Supplementary topic-specific searches

Topic-specific queries were developed as the taxonomy took shape, targeting areas
with limited coverage. Supplementary searches also used arXiv, IEEE Xplore, and
the ACM Digital Library, particularly for monitoring evasion, defense mechanisms,
and evaluation benchmarks, alongside citation chaining and related-work review.

| Research area | Supplementary search query | Sources |
|---|---|---|
| RQ1 — T1: Reasoning Manipulation and Backdoors | `"CoT manipulation" OR "chain-of-thought attack" OR "reasoning backdoor" OR "CoT backdoor" OR "reasoning style poisoning"` | All initial databases, arXiv |
| RQ1 — T1: amplification and denial of service | `"reasoning DoS" OR "overthinking attack" OR "inference cost attack" OR "reasoning length adversarial"` | arXiv, Semantic Scholar |
| RQ1 — T2: Indirect Prompt Injection and Tool-Chain Attacks | `"indirect prompt injection" OR "tool hijacking LLM" OR "RAG poisoning agent" OR "tool-chain attack"` | All initial databases |
| RQ1 — T3: Adaptive and Multi-turn Attacks | `"adaptive jailbreak" OR "multi-turn attack LLM" OR "adaptive adversarial agent" OR "iterative jailbreak"` | All initial databases |
| RQ1 — T4: Monitoring Evasion and Obfuscation | `"monitoring evasion LLM" OR "CoT obfuscation" OR "reasoning obfuscation" OR "deceptive alignment" OR "CoT faithfulness"` | arXiv, Semantic Scholar |
| RQ2 — Defenses | `"reasoning-aware defense" OR "runtime monitoring LLM agent" OR "CoT consistency check" OR "agentic defense mechanism"` | All initial databases |
| RQ3 — Evaluation | `"agentic AI benchmark security" OR "reasoning integrity metric" OR "adaptive adversary evaluation" OR "LLM agent security evaluation"` | All initial databases |

"All initial databases" refers to the four sources in Section 1. The search record
used the then-current cluster labels C1–C4; rows appear here under the
corresponding labels T1–T4.

## 3. Screening and eligibility

Records were screened by title and abstract against four scope dimensions —
reasoning-layer security, agentic AI scope, multi-turn attacks, and
adaptive-adversary coverage — retaining 120 papers for full-text assessment at that stage.
Continued searching during full-text reading expanded the collection, and a final
screening pass was completed in September 2026.

Papers were included if they address an attack, defense, or evaluation at or near
the reasoning layer of an LLM-based or agentic system, and were published
2024–2026 in English at a peer-reviewed venue or as a credible academic preprint.
Generic LLM safety, classical non-LLM agents, infrastructure security, and
conceptual commentary without technical or empirical grounding were excluded.
Scope is recorded per paper (LLM-only, Agent, Multi-Agent, Mixed) as a coded
variable rather than an exclusion criterion, so reasoning-focused LLM settings
remain in the corpus.

Duplicates were identified using Zotero and manual verification, including studies
appearing under revised titles or across preprint and published versions.

The de-duplicated working library contained 153 papers: an 89-paper structured
corpus and 64 background and supporting references. Within the structured corpus,
71 empirical papers form the annotated corpus. Papers may contribute to more than
one taxonomy.

## 4. Limitations of this record

Per-database execution dates, stage-level exclusion counts, the number of
duplicates merged, and the contribution of each supplementary route were not
recorded.
