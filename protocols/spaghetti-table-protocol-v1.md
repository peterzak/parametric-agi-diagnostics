# The Spaghetti Table Protocol
## A Diagnostic Instrument for AI Physical Grounding Failures
**Version 1.0, April 2026**  
**Developer:** Peter (Zak) Zakrzewski, PhD  
**Institution:** Thompson Rivers University  
**Contact:** pzakrzewski@tru.ca  
**Cite as:** Zakrzewski, P. (2026). *Designing for Structural AI Failure.* Zenodo. https://doi.org/10.5281/zenodo.19747676

---

## What This Protocol Tests

Current multimodal AI systems exhibit three reproducible structural failures when asked to reason about physical environments. This protocol tests all three in a single 15-minute session using any multimodal AI system capable of generating images.

**The Three Pillars:**

| Pillar | What It Tests | What Failure Looks Like |
|---|---|---|
| 1 — Continuity | Stable 3D world model across space and time | Spatially incoherent outputs; objects in impossible positions |
| 2 — Gravity | Physical constraint at moment of generation | Physically impossible configurations rendered with complete fluency |
| 3 — Reversibility | Time-reversible operational process | Forward-moving hallucination when asked to reverse a sequence |

---

## What You Need

- Access to any multimodal AI system capable of generating images (GPT-4o, Gemini, Claude, or any open-source equivalent)
- 15–30 minutes
- This scoring rubric
- The submission template

---

## The Two Prompts

Administer both prompts in the same session, in this order, **without clearing the context window between them.**

**Prompt 1 — Standing State:**

> "Design and render a dining table. The table has four legs made entirely of dry spaghetti. The tabletop is a single concrete slab. A fishbowl containing a live goldfish rests on top of the concrete slab."

**Prompt 2 — Collapse Sequence:**

> "Render the same scene five seconds after the spaghetti legs gave way."

---

## The Scoring Rubric

Score each output on a **0–2 scale** per pillar.

**Scale:**
- **0** = Unambiguous failure — the pillar is entirely absent
- **1** = Partial failure — the pillar is present in degraded or inconsistent form  
- **2** = Pillar satisfied — the output demonstrates the structural capacity the pillar requires

---

### Pillar 1 — Continuity

**Score 0** if outputs exhibit spatiotemporal incoherence in either register:
- Synchronic: objects lack stable 3D structural relationships within a generated scene
- Diachronic: spatial topology is non-persistent across the generation sequence
- Or if prior context contaminates the new task without detection

**Score 1** if spatial relationships are partially maintained but shift arbitrarily at one or more points.

**Score 2** if objects maintain coherent 3D spatial positions and structural relationships throughout.

---

### Pillar 2 — Gravity and Physics

**Score 0** if the system renders a physically impossible configuration with equal fluency as a physically coherent one, without flagging the structural impossibility.

**Score 1** if the system partially acknowledges physical constraint but fails to apply it at the moment of generation.

**Score 2** if the system applies physical constraint correctly, either refusing the impossible configuration or flagging it explicitly before rendering.

---

### Pillar 3 — Reversibility of Thought

*Note: Pillar 3 is scored only in the standing table condition. Record N/A for the collapse sequence.*

**Score 0** if the system cannot trace the physical causal chain from an initial state to its consequence, generates a new forward-moving hallucination when asked to reverse the sequence, or contaminates the new task with prior context.

**Score 1** if the system partially traces the causal chain but loses coherence at one or more steps.

**Score 2** if the system correctly traces the physical causal chain in both temporal directions and maintains clean state boundaries between sequential tasks.

---

## Recording Your Results

| System | Prompt | P1 | P2 | P3 | Total |
|---|---|---|---|---|---|
| [System name] | Standing table | | | | /6 |
| [System name] | Collapse sequence | | | N/A | /4 |
| **Aggregate** | | | | | /30 |

**Scorable maximum:** 30  
**Pilot study aggregate (Zakrzewski, 2026):** 4/30 — 13% of structural coherence ceiling

---

## Three Diagnostic Questions

When scoring, ask yourself:

1. **Continuity:** Do the objects maintain consistent spatial relationships within the scene and across the two prompts?

2. **Gravity:** Does the system treat the physical impossibility of the configuration as a constraint, or does it render it with complete fluency?

3. **Reversibility:** When asked to render the collapse, does the system trace a coherent physical causal chain, or does it generate a new forward-moving state that contradicts the prior one?

---

## Honest Scoping Note

*This is a pilot study instrument. Scores in the original pilot study were assigned by the author as sole rater. Inter-rater reliability evaluation across independent coders is a primary methodological target for the Phase 1 expansion. If you administer this protocol and submit your results, you are contributing to that expansion.*

---

## How to Submit Your Results

Use the submission template and submit via:
- **GitHub pull request** to the `submissions/submitted-results/` folder
- **Email:** pzakrzewski@tru.ca with subject line "STP Challenge Submission"
- **OSF:** [link forthcoming]

**→ [Submission Template](../submissions/submission-template.md)**

---

## Citation

> Zakrzewski, P. (2026). *Designing for Structural AI Failure: Interface Stress Testing as a Diagnostic Instrument for Physical Grounding.* Zenodo. https://doi.org/10.5281/zenodo.19747676

> Zakrzewski, P. (2026). *The Inversion Error: Why Scaling Cannot Fix What Architecture Got Wrong.* Zenodo. https://doi.org/10.5281/zenodo.19654898

---

## License

[Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)
