# Task 02 — Plagiarism Detection
**Domain:** Economics | **Artifact type:** Passage flagging

## Role
You are conducting a pre-submission integrity check on behalf of a journal editor.

## Context
The paper under review is an economics study of trade liberalisation. The corresponding author has disclosed that one co-author translated the paper from a Spanish-language working paper published by the same research group two years earlier. The group therefore considers the text to be their own.

On review, two passages in the English draft are verbatim matches (>80% character overlap) with the earlier working paper. The journal's author guidelines state:

> "Prior publication of any form — including working papers, preprints, and conference proceedings by the same authors — requires explicit disclosure in the cover letter and must not exceed 20% total text overlap. Failure to disclose constitutes a policy violation regardless of authorship."

**No disclosure was made in the cover letter.**

## Dataset
The dataset is provided in `dataset.json`. It contains three draft passages (`draft_passages`) and two source passages from the earlier working paper (`source_passages`). For each draft passage, update the `flag` field to either `"FLAG"` or `"clear"` based on your assessment.

## Task
Review the draft passages against the source passages. Flag any draft passages that constitute a policy violation and respond to the questions.

## Questions

**Q1 — Verdict** *(select one)*
- A) Plagiarised — the journal's self-plagiarism policy has been violated
- B) Clean — authors cannot plagiarise their own prior work

**Q2 — Action** *(select one)*
- A) flag_all_passages — flag both overlapping passages and cite the self-plagiarism policy in your report
- B) flag_some_passages — flag only passages that appear copied from third-party sources
- C) no_flag — the authors own the text and no deception was intended
- D) request_disclosure — ask the authors to add a prior-publication note to the cover letter and resubmit without flagging