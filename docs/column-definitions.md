# Column definitions

Permitted values and a one-line definition for each coded column in the [annotation matrix](annotation-matrix.md) and the [threat](threat-taxonomy.md), [defense](defense-taxonomy.md), and [evaluation](evaluation-taxonomy.md) tables. Cluster definitions are given in Tables 4–6 of the paper, and gap criteria in Section 3.4 and Table 3. Flags: ● addressed · ◐ partially addressed · ○ present · – not applicable.

| Column | Values | Definition |
|---|---|---|
| Publication status | Peer-reviewed journal / conference / workshop · Preprint | Status of the venue of record. |
| T · D · E | T1–T4 · D1–D3 · E1–E3 · – | Primary cluster in each taxonomy; – if the paper has no role in it. |
| Vector | Direct prompt · Indirect prompt · Memory · Tool · Environment · Inter-agent · Training data · Model customization | Where the attack enters the system. |
| Pattern (threat) | CoT manipulation · Tool manipulation · Memory poisoning · Goal hijacking · Backdoor | What the attack does. |
| Target | Input / perception · Reasoning / planning · Action / tool use · Memory / knowledge · Multiple | Agent component affected. |
| Structure (threat) | Single-turn · Multi-turn · Adaptive | How the attack unfolds across interactions. |
| Pattern (defense) | Input sanitization · Output verification · Guardrail · Runtime monitoring · Sandboxing · Reasoning consistency check · Adversarial training | Mechanism the defense uses. |
| Structure (defense) | Static · Adaptive · Mixed | Whether the defense behaves fixedly or adjusts during operation. |
| Reasoning-aware | Yes · Partial · No | Whether the defense operates on intermediate reasoning (Yes), constrains it without reading it (Partial), or not at all (No). |
| Scope | Agent · Multi-agent · Mixed · LLM only | Agentic setting of the reported evaluation (Section 3.4). |
| RIM | Explicit · Implicit · – | Reasoning integrity metric: a direct measure, a reasoning-level proxy, or outcome metrics only. |
| AA | Yes · No | Whether the attacker adapts during the evaluated interaction. |
| ARE | Yes · Partial · No · – | Strength of adaptive testing of a proposed defense; – if there is no defense. |
| G1, G2, G5 | ● · ○ | Recorded once per paper. G2 follows RIM; G5 follows Scope. |
| G3 (T/D/E), G4 (T/E/D) | ● · ◐ · ○ · – | Recorded per role. G3 (D) follows Reasoning-aware; G4 (T/E) follows AA; G4 (D) follows ARE. ◐ occurs only in G3 (D) and G4 (D), and in G3 (T) where it carries the G3 (D) value. |
