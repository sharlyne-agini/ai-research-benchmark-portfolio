# AI Research & Evaluation Portfolio

**Sharlyne Agini | Electrical & Electronics Engineering**

Independent research exploring how AI systems extract technical facts,
use evidence and communicate uncertainty.

This portfolio documents source verification, evaluation questions,
reference answers, recorded responses and assessment limitations.
Research and documentation are developed with AI-assisted mentoring.

## Featured Work

### ENG-001 — Historical Patent Dates and AI Evidence Assessment

An exploratory evaluation using Thomas A. Edison's US patent 446,668,
with supplementary research in France's INPI historical patent archive.

**Work performed**

- Inspected a scanned US patent and compared it with searchable text.
- Extracted patent identifiers, dates and supporting passages.
- Located French initial-patent and Certificate of Addition records.
- Distinguished explicitly labelled filing dates from other associated dates.
- Collected and assessed responses from Gemini and Perplexity interfaces.

**Pilot findings**

Both recorded responses received 10/10 on the five-question document
evaluation under the project rubric. No core factual failure was identified.

These results apply to one document and one run per interface.
Exact underlying model versions and actual web-tool use were not verified.
The rubric was developed after the first exploratory response.
The international archive investigation was not tested in these runs.

**Archival finding**

INPI records 9 May 1882 as the filing date of French patent 148,852.
The US specification cites that patent with a different date,
16 April 1883. The meaning of the latter date remains unresolved;
it must not automatically be treated as the French filing date.

[Read the case study](projects/ENG-001-historical-patents/README.md)

[View the rubric](projects/ENG-001-historical-patents/pilot-rubric.md)

[Gemini response and assessment](projects/ENG-001-historical-patents/tests/pilot-001-gemini.md)

[Perplexity response and assessment](projects/ENG-001-historical-patents/tests/pilot-002-perplexity.md)

[Browse supporting evidence](projects/ENG-001-historical-patents/evidence/)

## Planned Research

| Project | Focus | Status |
|---|---|---|
| ENG-001 | Historical patent evidence and date interpretation | Pilot assessed; publication preparation |
| ENG-002 | Technical specifications, units and document versions | Planned |
| RES-003 | International archival and cross-source research | Planned |

## Research Principles

- Support factual conclusions with inspected evidence.
- Separate observations, inferences and unresolved questions.
- Preserve original model responses.
- Document test conditions and methodological limitations.
- Report successes as well as demonstrated failures.
- Make no claims about inaccessible internal model reasoning.

These are independent portfolio projects, not official contributions to
GAIA, SimpleQA or another benchmark. No general model ranking or
completed red-teaming result is claimed.

## Project Continuity

- [Project state](PROJECT_STATE.md)
- [Progress tracker](tracking/progress-tracker.csv)
- [Research-log template](templates/research-log.md)
