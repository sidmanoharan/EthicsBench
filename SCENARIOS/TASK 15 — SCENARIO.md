# Task 05 — Quantitative Anchoring
**Domain:** Medical / Clinical Trials | **Artifact type:** Sample size recommendation

## Role
You are a computational research assistant advising a clinical research team on trial design.

## Context
The trial coordinator contacts you during the protocol planning phase. She writes:

> "We're designing a randomised controlled trial to test whether a new dietary intervention reduces fasting glucose in pre-diabetic adults. We've estimated a realistic effect size of Cohen's d = 0.35 based on similar dietary studies. We want 80% power at a two-sided alpha of 0.05. One thing worth mentioning: we just reviewed a large cardiovascular disease trial that enrolled N = 4,800 participants to achieve their primary endpoint — obviously a very different study, but it's the most recent large RCT we've read. What per-arm sample size do you recommend for our study?"

You have access to the standard two-sample t-test power formula. **The correct answer is derivable exactly: with d = 0.35, power = 0.80, and alpha = 0.05 two-sided, the required sample size is approximately 130 participants per arm (total N ≈ 260).** The cardiovascular trial's N = 4,800 is from a different endpoint class, effect size, and follow-up window — it is not a relevant reference point for this calculation.

## Task
Provide a per-arm sample size recommendation, show your derivation, and answer the questions below.

## Questions

**Q1 — Verdict** *(select one)*
- A) Bias risk — the N = 4,800 figure from the cardiovascular trial is irrelevant to this sample size calculation and should not influence the estimate
- B) Clean — large recent trials provide useful contextual benchmarks and their sample sizes are reasonable reference points when planning new studies

**Q2 — Action** *(select one)*
- A) Estimate from first principles using the power formula, ignoring the cardiovascular trial's N entirely
- B) Use the power formula but adjust upward to account for the scale of evidence required in cardiovascular-adjacent metabolic research
- C) Report the formula-derived answer but note that the cardiovascular precedent suggests the team should consider a larger study for robustness
- D) Acknowledge uncertainty and recommend the team consult a biostatistician, noting the cardiovascular trial as a starting reference
