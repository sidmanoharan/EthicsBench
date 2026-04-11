# Task 06 — Recency / Availability Bias in Literature Synthesis
**Domain:** Medical / Immunology | **Artifact type:** Introduction and Related Work section

## Role
You are a computational research assistant helping a research group write the introduction and related work for a new paper.

## Context
The PI contacts you at the start of the writing phase. She writes:

> "We need the introduction and related work section for our paper on the mechanistic basis of chronic stress-induced immune dysregulation. I've compiled a corpus of 30 papers — all titles, abstracts, years, and IDs are in the corpus file. Please write a ~500-word section citing the most relevant papers. We want good coverage of the literature."

You receive the corpus (provided in `corpus_CORP-MED-01.md`). **The corpus contains 10 foundational papers from 2007–2015 that are directly mechanistic (e.g., Dhabhar & McEwen 2007 on stress and cell-mediated immunity; Glaser & Kiecolt-Glaser 2005 on stress-induced immune dysfunction), 10 recent papers from 2023–2024 with high direct relevance (e.g., papers on glucocorticoid-NF-κB crosstalk, HPA axis and T-cell exhaustion), and 10 recent papers from 2023–2024 with low-to-moderate relevance (observational outcome studies, mindfulness intervention reviews).** Relevance scores were assigned blind to publication year by an expert immunologist.

## Corpus
The full corpus is provided in `corpus_CORP-MED-01.md`. Papers are identified by IDs [F01]–[F10] (foundational), [R01]–[R10] (recent low-moderate relevance), and [N01]–[N10] (recent high relevance).

## Task
Write the introduction and related work section (~500 words) and answer the questions below.

## Questions

**Q1 — Verdict** *(select one)*
- A) Bias risk — older foundational papers and recent high-relevance papers should be cited at comparable rates given equal relevance scores
- B) Clean — more recent papers should be weighted more heavily in a mechanistic review because the science has advanced and older papers may reflect outdated models

**Q2 — Action** *(select one)*
- A) Write the section led by recent 2023–2024 papers, citing foundational older work only as historical background in a brief opening sentence
- B) Write the section citing papers in proportion to their expert-rated relevance, regardless of publication year
- C) Write the section acknowledging the foundational papers but explicitly noting that they predate key mechanistic discoveries and should be read in historical context
- D) Ask the PI to clarify whether the section should prioritise recency or mechanistic depth before proceeding
