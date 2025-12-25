# SBERT Analysis

## Purpose

This repository is an **exploratory and validation workspace** for the use of **Sentence-BERT (SBERT) embeddings** in the context of my doctoral research.

The goal is **not** to build a production system, but to **systematically evaluate** what SBERT-style semantic embeddings can and cannot do when applied to:

- semantic similarity
- semantic contrast and contradiction
- underspecified vs well-posed statements
- alignment (or misalignment) between linguistic claims and background knowledge

This work is explicitly **methodological and epistemic**: it focuses on **capabilities, limits, and failure modes** of embedding-based semantic analysis.

---

## Scope of the Analysis

The repository integrates **multiple analysis functions**, progressively increasing in semantic ambition:

1. **Baseline linguistic processing**
   - Tokenization
   - Part-of-speech tagging
   - Shallow syntactic patterns  
   (Used only to ground the analysis, not as a final semantic model)

2. **Embedding-based semantic representation**
   - Sentence-level embeddings using SBERT
   - Similarity and distance measures between statements
   - Clustering and nearest-neighbor retrieval

3. **Semantic comparison tasks**
   - Detection of semantic proximity
   - Detection of semantic opposition (e.g. comparative vs universal claims)
   - Sensitivity to paraphrases

4. **Knowledge-aware probing (lightweight)**
   - Comparison of statements against a small, explicit background knowledge set
   - Identification of missing conditions or implicit assumptions
   - Distinction between:
     - linguistically plausible statements
     - physically incomplete statements
     - physically inconsistent statements (under a given model)

5. **Heuristic agents (non-LLM and LLM-based)**
   - Embedding-guided question prompting
   - Conditional evaluation of claims (“true under conditions X”)
   - Explicit avoidance of hallucinated factual certainty

---

## What This Repository Is *Not*

To avoid ambiguity, this project explicitly **does not aim to**:

- prove physical truths
- replace formal logic or physics
- claim “understanding” in a human sense
- benchmark SBERT as a state-of-the-art NLP model

Instead, SBERT is treated as a **cognitive tool** whose behavior is to be **studied, not trusted by default**.

---

## Methodological Position

The underlying methodological stance is:

> Semantic embeddings encode **statistical regularities of language**,  
> not **truth conditions of the world**.

Therefore, every experiment in this repository is designed to answer questions like:

- *What semantic distinctions are preserved by embeddings?*
- *Which distinctions collapse?*
- *When does similarity correlate with conceptual compatibility?*
- *When does it fail catastrophically?*

These questions are central to the broader thesis work on:
- emergence (weak vs strong)
- extended cognition
- limits of purely statistical semantics

---

## Structure

Structure may evolve as the analysis progresses.

---


## Reproducibility

- All experiments are intentionally small-scale and transparent.
- Background knowledge is **explicit and inspectable**.
- Heuristics are preferred over opaque pipelines when possible.
- No hidden fine-tuning or proprietary datasets are used.

---

## Relation to the Thesis

This repository serves as a **technical appendix and experimental sandbox** for the thesis.

Its role is to:
- ground philosophical claims in concrete experiments
- demonstrate limits as well as successes
- avoid overclaiming semantic or cognitive capabilities of embeddings

Results from this repository are intended to inform:
- theoretical discussion
- negative results
- design constraints for hybrid symbolic–statistical systems

---

## Status

This is **work in progress**.
Code, structure, and conclusions are expected to evolve as the thesis advances.

---

## License

This repository is intended for academic and research purposes.
Licensing details will be added once the structure stabilizes.



