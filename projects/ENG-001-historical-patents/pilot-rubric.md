# Single-Document Pilot Rubric — Version 1

## Scope

Evaluate responses to the five-question prompt using 00446668.pdf.
This assesses document extraction and evidence limits, not web research.

Created after the first Gemini response and before subsequent runs.
The rubric is informed by that response; the first run is exploratory.

## Scoring

Score each question from 0 to 2:

- 2: All requested facts are correct, with an accurate PDF page reference
  and supporting wording. Conclusions stay within the evidence.
- 1: The substantive answer is correct but incomplete, or its evidence
  reference is missing or inaccurate.
- 0: The substantive answer is incorrect, absent, or includes a material
  unsupported assertion.

Maximum: 10 points. Report each question separately.

## Reference Answers

1. US patent 446,668; Electric-Arc Light; Thomas A. Edison.
2. Application filed August 7, 1882; serial number 68,651.
3. US Letters Patent dated February 17, 1891.
4. British patent No. 3,976; August 19, 1882.
   Preserve the source wording: "Patented in England" or
   "Letters Patent in Great Britain ... dated".
   Do not automatically relabel this as a filing or publication date.
5. No. The US document does not separately establish the British
   filing and publication dates.

Reference location: PDF page 2.

## Additional Checks

Record separately from the numerical score:

- Any extra factual claims and whether they were checked.
- Whether supporting quotations accurately reflect the scan.
- Any observable instruction violations.
- Whether tool use is known or unknown.
- Exact model identity and configuration limitations.

Do not infer browsing compliance merely from the absence of web citations.
Do not classify hidden reasoning or invent a failure mechanism.

## Interpretation

A perfect score means success on this specific document and prompt.
It does not establish general research ability or superiority over
another model.

Keep answer keys out of test conversations.
Freeze this rubric before subsequent runs. If revised, record why and
rescore all responses consistently.
