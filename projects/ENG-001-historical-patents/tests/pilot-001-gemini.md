# Pilot 001 — Gemini Document Evaluation

## Run Details

- Project: ENG-001
- Task type: Single-document extraction and evidence assessment
- Test date: 2026-10-21
- Provider/interface: Google Gemini in Chrome side panel
- Mode shown: Auto
- Exact underlying model identifier: Not disclosed in captured interface
- Input document: 00446668.pdf — US patent 446,668
- New conversation: Yes — confirmed by researcher
- Only this PDF attached: Yes — confirmed by researcher
- Reference answers supplied beforehand: No — confirmed by researcher
- Web search: Prohibited by prompt; actual tool use not independently verified
- Additional interface context: Screenshot displayed Sharing "New Tab"
- Transcript provenance: Copied by the researcher into the mentoring conversation.
  The prompt and response below preserve that supplied text, with Markdown
  formatting normalized.

## Exact Submitted Prompt

Use only the attached patent document.

1. Identify the US patent number, invention title and inventor.
2. Give the application filing date and serial number.
3. Give the date attached to the US Letters Patent.
4. Extract the British patent number and associated date, preserving
   how the document describes that date.
5. Does this document alone independently establish the British
   patent's filing and publication dates? Explain briefly.

For each answer, identify the PDF page and supporting wording.
Distinguish explicit statements from inference. If a fact cannot be
established from this document, say so. Do not use web search.

## Complete Model Response

1. **US Patent Number, Invention Title, and Inventor**
   - **US Patent Number:** 446,668
   - **Invention Title:** Electric-Arc Light
   - **Inventor:** Thomas A. Edison
   - **PDF Page:** Page 2
   - **Supporting Wording:** "UNITED STATES PATENT OFFICE. THOMAS A. EDISON, OF MENLO PARK, NEW JERSEY... ELECTRIC-ARC LIGHT. SPECIFICATION forming part of Letters Patent No. 446,668..." (Explicit statement)

2. **Application Filing Date and Serial Number**
   - **Filing Date:** August 7, 1882
   - **Serial Number:** 68,651
   - **PDF Page:** Page 2
   - **Supporting Wording:** "Application filed August 7, 1882. Serial No. 68,651, (No model.)" (Explicit statement)

3. **Date Attached to the US Letters Patent**
   - **Date:** February 17, 1891
   - **PDF Page:** Page 2 (also found on page 1)
   - **Supporting Wording:** "...dated February 17, 1891." and "Patented Feb. 17, 1891." (Explicit statement)

4. **British Patent Number and Associated Date**
   - **British Patent Number:** 3,976
   - **Associated Date:** August 19, 1882 (described in the document as "dated August 19, 1882")
   - **PDF Page:** Page 2
   - **Supporting Wording:** "Patented in England August 19, 1882, No. 3,976" and "...for which I have obtained Letters Patent in Great Britain, No. 3,976, dated August 19, 1882..." (Explicit statement)

5. **Independent Establishment of British Patent Dates**
   - **Does this document alone independently establish the British patent's filing and publication dates?** No.
   - **Explanation:** While the document explicitly states the British patent number and an associated date ("August 19, 1882"), it merely lists these foreign patent details as a historical declaration by the patentee. It does not provide official British patent office records, filing receipts, or publication certificates to independently prove the legal filing and official publication events under British law. This is an explicit statement of foreign patent existence within the US text, requiring inference or external verification to confirm it as the official filing and publication timeline.

## Researcher Scoring — Rubric Version 1

Evaluator: Sharlyne Agini
Review assistance: AI mentoring assistant
Rubric: ../pilot-rubric.md

| Question | Score | Reason |
|---|---|---|
| Q1 | 2/2 | Correct patent number, title and inventor with page-2 support. |
| Q2 | 2/2 | Correct filing date and serial number with page-2 support. |
| Q3 | 2/2 | Correct Letters Patent date with page-2 support. |
| Q4 | 2/2 | Correct British reference and date; source wording preserved. |
| Q5 | 2/2 | Correctly identifies that British filing and publication dates are not separately established. |

Total: 10/10 — provisional.

## Qualitative Review

- No factual failure identified in the five core answers.
- The additional page-1 date attribution was visually checked against the source PDF and is supported.
- Supporting passages were assessed for factual support; character-for-character
  transcription fidelity has not been fully audited.
- For Q5, the decisive limitation is that the US passage does not separately
  identify British filing and publication events. Filing receipts or publication
  certificates are examples offered by the model, not mandatory evidence types.
- Actual web-tool use and exact underlying model version are unknown.
- No hidden reasoning or internal model processes were available for analysis.

## Methodological Limitations

- The rubric was created after this exploratory response and was informed by it.
- One response to one document does not establish general model performance.
- This run tests document extraction and evidence limits, not international
  archival research or web-source discovery.
- No overall ranking against another model is justified.
- The screenshot reviewed shows the prepared prompt and Auto mode, not the
  returned response. The result is preserved from researcher-supplied text.

## Evidence Status

- Source PDF page 2 visually reviewed by the mentoring assistant.
- Researcher confirmed a fresh conversation, one attached PDF and no
  reference answers supplied before the test.
- Source PDF and screenshot preservation in the repository remains to be checked.
- This revised file must be reviewed after saving before publication.
