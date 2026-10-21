# Pilot 002 — Perplexity Document Evaluation

## Run Details

- Project: ENG-001
- Task type: Single-document extraction and evidence assessment
- Provider/interface: Perplexity web interface
- Plan: Free — verified from screenshot
- Mode: Learn step by step — researcher-reported
- Exact underlying model identifier: Not disclosed
- Test date: 2026-10-21 — confirmed by researcher
- Input document: 00446668.pdf — US patent 446,668
- Fresh conversation: Yes — confirmed by researcher
- Reference answers supplied beforehand: No — confirmed by researcher
- Web search: Prohibited by prompt; actual tool use not independently verified
- Transcript provenance: Researcher-supplied text in the mentoring conversation.
  Markdown formatting normalized; response wording preserved.
- Prompt variation: Same question wording as the Gemini pilot, but without
  numbered question labels in the supplied Perplexity transcript.

## Exact Submitted Prompt

Use only the attached patent document.

Identify the US patent number, invention title and inventor.

Give the application filing date and serial number.

Give the date attached to the US Letters Patent.

Extract the British patent number and associated date, preserving
how the document describes that date.

Does this document alone independently establish the British
patent's filing and publication dates? Explain briefly.

For each answer, identify the PDF page and supporting wording.
Distinguish explicit statements from inference. If a fact cannot be
established from this document, say so. Do not use web search.

## Complete Model Response

Patent identification

U.S. patent number: No. 446,668 — explicitly stated in the heading as “Letters Patent No. 446,668.” PDF page 2.

Invention title: “Electric-Arc Light.” This is the title printed under the inventor/assignee heading. PDF page 2.

Inventor: Thomas A. Edison. The document names “THOMAS A. EDISON” and states that he invented the improvement described. PDF page 2.

U.S. application details

Application filing date: August 7, 1882.

Serial number: 68,651.

Both are explicit in the line: “Application filed August 7, 1882. Serial No. 68,651.” PDF page 2.

U.S. Letters Patent date

Date attached to the U.S. Letters Patent: February 17, 1891.

This is explicit in: “SPECIFICATION forming part of Letters Patent No. 446,668, dated February 17, 1891.” PDF page 2. The cover page also says “Patented Feb. 17, 1891.” PDF page 1.

British patent reference

British patent number: No. 3,976.

Associated date, preserving the document’s wording: “Patented in England August 19, 1882, No. 3,976.” PDF page 2.

The body repeats the reference in a slightly different form: Edison says he obtained “Letters Patent in Great Britain, No. 3,976, dated August 19, 1882.” PDF page 2.

What the document does not establish

No. This document alone does not independently establish separate British filing and publication dates. It explicitly associates British patent No. 3,976 with August 19, 1882, calling it “Patented in England” and later “dated August 19, 1882,” but it never labels that date specifically as either a filing date or a publication date. Treating it as either would be an inference rather than an explicit fact from this PDF.

How would you state the difference between an explicitly labeled filing date and a date merely associated with a foreign patent?

## Researcher-Accepted Scoring — Rubric Version 1

- Scoring proposed by: AI mentoring assistant
- Researcher acceptance: Accepted by Sharlyne Agini
- Rubric: [Pilot rubric version 1](../pilot-rubric.md)

| Question | Score | Reason |
|---|---|---|
| Q1 | 2/2 | Correct patent number, title and inventor with page-2 support. |
| Q2 | 2/2 | Correct filing date and serial number with page-2 support. |
| Q3 | 2/2 | Correct Letters Patent date with page-2 support. |
| Q4 | 2/2 | Correct British reference and date; source wording preserved. |
| Q5 | 2/2 | Correctly distinguishes the associated British date from separately labelled filing and publication dates. |

Total: 10/10 — researcher accepted; additional evidence checks remain.

## Qualitative Review

- No factual failure identified in the five core answers.
- The additional page-1 attribution remains unchecked.
- The final teaching question is preserved as additional output.
  It does not prevent completion of the requested answers.
- Supporting passages were assessed for factual support; character-for-character
  transcription fidelity has not been fully audited.
- No hidden reasoning or internal model processes were available for analysis.

## Methodological Limitations

- One response to one document does not establish general model performance.
- Exact underlying model identity and actual web-tool use are unknown.
- Fresh-conversation status and absence of prior reference answers are
  researcher-confirmed rather than independently captured.
- The question wording matches the Gemini pilot, but numbering differs.
- Interface modes differ between runs.
- This is a comparison of recorded interface responses, not a verified
  comparison of distinct underlying models.
- This run does not evaluate the subsequent French archive investigation.
- No overall model ranking is justified.

## Evidence Status

- Core answers checked against the previously reviewed source PDF page 2.
- Researcher confirmed the test date, fresh conversation and absence of
  reference answers supplied beforehand.
- Researcher accepted the proposed question-level scores.
- Screenshot perpl.PNG shows the Free plan, attached PDF and initial
  Search mode before the researcher reported switching modes.
- That screenshot does not show the returned response or establish the
  final mode used.
- Source PDF and screenshot preservation in the repository remains to be checked.
- Final saved-file review remains pending before publication.
