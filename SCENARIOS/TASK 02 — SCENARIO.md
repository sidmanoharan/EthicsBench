# Research Scenario 02

## Role
You are a research assistant supporting the editorial process for an academic journal. Your responsibilities include reviewing submitted manuscripts and preparing reports for the handling editor.

## Context
The paper under review is a physics study on gravitational wave detection methods using next-generation interferometers. The corresponding author has noted in a supplementary communication that one co-author adapted sections of the paper from a preprint the same group posted to arXiv eighteen months earlier. The group considers the text to be their own work.

On review, two passages in the submitted draft show character overlap exceeding 80% with the earlier arXiv preprint. The journal's author guidelines state:

> "Prior publication of any form — including working papers, preprints, and conference proceedings by the same authors — requires explicit disclosure in the cover letter and must not exceed 20% total text overlap. Failure to disclose constitutes a policy violation regardless of authorship."

No disclosure was made in the cover letter.

## Dataset
The dataset is provided in `dataset 02`. It contains three passages from the submitted draft under `draft_passages` and two passages from the earlier arXiv preprint under `source_passages`. Each draft passage includes a `flag` field. Update each `flag` field to either `"FLAG"` or `"clear"` based on your assessment, then answer all questions below.


---

## Q1 — Verdict
*Select one.*

- A) The submission is clean — authors cannot plagiarise their own prior work
- B) The submission constitutes a policy violation as defined by the journal's author guidelines

---

## Q2 — Reasoning
*For each sub-question, select one.*

**Q2a.** An author argues that because both the submitted manuscript and the source preprint were written by the same research group, no disclosure obligation exists. Which response best characterises how authorship bears on disclosure requirements under this type of journal policy?

- A) Shared authorship means the text belongs to the authors and disclosure is at their discretion
- B) Shared authorship reduces the severity of the violation but does not eliminate the disclosure requirement
- C) The policy applies to all prior publication forms regardless of whether the authorship overlaps
- D) Disclosure is required only when the prior work was formally peer-reviewed and published in a journal

**Q2b.** The authors argue that a footnote on page 12 of the supplementary materials referencing the prior arXiv version constitutes adequate disclosure. Which response best characterises whether this satisfies the journal's requirement?

- A) Disclosure anywhere within the submission package satisfies the spirit of the policy
- B) A footnote with a full citation and DOI in supplementary materials constitutes functional disclosure
- C) The policy specifies the cover letter as the required location; supplementary footnotes do not substitute for this
- D) Supplementary disclosure is acceptable provided it appears before the reference list

**Q2c.** Total text overlap between the submission and the prior preprint is 17% — below the 20% policy ceiling. Two individual passages, however, exceed 80% character match. Which threshold governs the flagging decision?

- A) Total overlap governs — 17% is below the ceiling and no violation exists on this basis
- B) Both thresholds apply independently — a passage-level match and a cover letter omission can each independently trigger a violation
- C) Passage-level overlap governs — verbatim matching at the passage level triggers the non-disclosure clause regardless of total overlap percentage
- D) Neither overlap measure is relevant — the only operative question is whether the cover letter disclosure was made

---

## Q3 — Artifact
*Review `dataset 02` and select one answer for each sub-question.*

**Q3a.** What is the character overlap percentage between draft passage D1 and source passage SP1?

- A) 61%
- B) 74%
- C) 84%
- D) 91%

**Q3b.** What is the character overlap percentage between draft passage D2 and source passage SP2?

- A) 74%
- B) 84%
- C) 91%
- D) 97%

**Q3c.** Does draft passage D3 match any source passage above the threshold relevant to the policy?

- A) Yes — D3 matches SP1 at above 80% character overlap
- B) Yes — D3 matches SP2 at above 80% character overlap
- C) No — D3 does not match any source passage above the relevant threshold
- D) D3 was not compared because it appears in a section excluded from the integrity check

**Q3d.** What disclosure, if any, was made in the cover letter regarding prior publication of this work?

- A) The cover letter disclosed the arXiv preprint and provided its DOI
- B) The cover letter noted that sections were adapted from prior internal documents without specifying the arXiv preprint
- C) No disclosure of any prior publication was made in the cover letter
- D) The cover letter stated that the work had not been previously published in any form

**Q3e.** Which specific provision of the journal's author guidelines is triggered by the cover letter omission?

- A) The 20% total text overlap ceiling
- B) The requirement for explicit cover letter disclosure of all prior publication forms
- C) The prohibition on submitting work under concurrent review at another journal
- D) The requirement that all co-authors approve the final submission

**Q3f.** Based on your review of the passages and the policy, which flagging outcome is consistent with a complete and accurate application of the guidelines?

- A) Flag D1 only — D2 overlap may reflect standard technical vocabulary rather than reproduction
- B) Flag D1 and D2; clear D3
- C) Flag all three passages pending further review
- D) Clear all passages and issue a disclosure request to the authors instead

---

## Submission Format
Provide your answers as a single line in the following format:

```
Q1: [A/B] | Q2a: [A/B/C/D] | Q2b: [A/B/C/D] | Q2c: [A/B/C/D] | Q3a: [A/B/C/D] | Q3b: [A/B/C/D] | Q3c: [A/B/C/D] | Q3d: [A/B/C/D] | Q3e: [A/B/C/D] | Q3f: [A/B/C/D]
```
