# ENG-001 — Historical Patent Dates and AI Evidence Assessment

- **Author:** Sharlyne Agini
- **Research date:** 21 October 2026
- **Version:** 1.0 — publication draft
- **Scope:** Exploratory document-evaluation pilot with supplementary US–France archival research

- **[Read or download the research report](ENG-001_Research_Report.pdf)**

## Overview

This case study examines accurate extraction of historical patent information
and the distinction between explicitly labelled filing dates and other
dates associated with a patent.

Two AI-interface responses answered a five-question document task correctly
under the pilot rubric. Subsequent archival research identified a French
filing date that differs from the date cited in the US specification.
The meaning of the US-cited French date remains unresolved.

## Research Question

Can historical electrical-lighting patent references be checked across
national records without confusing filing dates with other patent dates?

## Sources and Method

I inspected US patent 446,668, Electric-Arc Light, by Thomas A. Edison,
using a Rutgers-hosted scan. I extracted identifiers and dates from PDF
page 2 and compared searchable text with scanned printing.

The US specification references foreign patents, including French patent
148,852, dated 16 April 1883.

After unsuccessful searches for the British reference, I searched INPI's
historical patent archive by French patent number. I located the initial
patent record and a separate Certificate of Addition.

Verification consisted of researcher inspection and AI-assisted review
of supplied documents and screenshots. No independent second human
verification was performed.

## Verified Findings

| Record | Explicitly labelled information | Evidence |
|---|---|---|
| US446668, PDF page 2 | Application filed 7 August 1882; serial 68,651 | [US patent scan](evidence/00446668.pdf) |
| US446668, PDF page 2 | US Letters Patent dated 17 February 1891 | [US patent scan](evidence/00446668.pdf) |
| US446668, PDF page 2 | French patent 148,852 cited as dated 16 April 1883 | [US patent scan](evidence/00446668.pdf) |
| INPI 1BB148852 | Initial patent filing date: 9 May 1882 | [Initial record screenshot](evidence/inpi_initial_patent.PNG) |
| INPI 1BB148852_1 | Certificate of Addition filing date: 26 December 1882 | [Addition record screenshot](evidence/inpi_addition.PNG) |

[View US patent](https://github.com/sharlyne-agini/ai-research-benchmark-portfolio/blob/main/projects/ENG-001-historical-patents/evidence/00446668.pdf) · [Download PDF](https://github.com/sharlyne-agini/ai-research-benchmark-portfolio/raw/refs/heads/main/projects/ENG-001-historical-patents/evidence/00446668.pdf)

If GitHub cannot display the preview, use Download PDF.
INPI identifies the applicant as EDISON Thomas-Alva. Its initial record
concerns improvements to electric arc lighting and regulating mechanisms.

The [first scanned image](evidence/french_patent_first_page.PNG)
also contains a 9 May 1882 deposit reference, corroborating the
catalogue's filing-date entry.

The initial patent and its addition share a patent number but have
different archive references and filing dates. They must be distinguished
during extraction.

## Main Conclusion

A date associated with a foreign patent in a US specification must not
automatically be classified as its filing date.

The French initial-patent filing date is explicitly recorded as
9 May 1882. The meaning of the US-cited 16 April 1883 date remains
unresolved. Different event dates do not by themselves demonstrate
contradictory records or an error in either source.

This research establishes a cross-source date-label distinction.
It does not establish identical technical or legal coverage across countries.

## AI Document-Evaluation Pilot

### Task

Using only US446668, each system was asked to:

1. Identify the US patent number, title and inventor.
2. Extract the application filing date and serial number.
3. Extract the date attached to the US Letters Patent.
4. Extract the British reference while preserving its date wording.
5. Assess whether the document independently establishes separate
   British filing and publication dates.

The instructions requested PDF pages and supporting wording,
distinguished explicit statements from inference, and prohibited web search.

### Test Conditions

| Field | Gemini run | Perplexity run |
|---|---|---|
| Date | 21 October 2026 | 21 October 2026 |
| Interface | Gemini in Chrome side panel | Perplexity web interface |
| Mode | Auto | Learn step by step |
| Exact underlying model | Not disclosed | Not disclosed |
| Fresh conversation | Researcher-confirmed | Researcher-confirmed |
| Reference answers supplied beforehand | No — researcher-confirmed | No — researcher-confirmed |
| Actual web-tool use | Not independently verified | Not independently verified |

Question wording was equivalent, but the supplied Perplexity prompt
omitted question numbering. Interface configurations also differed.

### Results

| Question | Gemini | Perplexity |
|---|---|---|
| Patent identification | 2/2 | 2/2 |
| Filing date and serial number | 2/2 | 2/2 |
| US Letters Patent date | 2/2 | 2/2 |
| British reference and date wording | 2/2 | 2/2 |
| Evidence limits | 2/2 | 2/2 |
| **Total** | **10/10** | **10/10** |

Scores were accepted by the researcher with AI-assisted review.
Additional evidence checks remain, as documented below.

No core factual failure was identified. Both responses distinguished
the British associated date from separately established filing and
publication dates.

These runs tested single-document extraction and evidence assessment.
They did not test discovery or interpretation of the French archive records.

## Evaluation Method

The [pilot rubric](pilot-rubric.md) assigns 0–2 points per question,
considering correctness, completeness, supporting wording, page reference
and whether conclusions stay within the evidence.

The rubric was created after the Gemini response and before the
Perplexity run. The first run is therefore exploratory, and the rubric
was informed by its response.

Scores describe these recorded responses, not general model capabilities.

## Limitations

- One document and one recorded response per interface.
- Exact underlying model versions were not disclosed.
- Web search was prohibited by the prompt; actual tool use was not verified.
- Prompt numbering and interface modes differed.
- The rubric was developed after the Gemini response.
- Additional page-1 references in responses remain unchecked.
- Character-for-character quotation fidelity has not been fully audited.
- Transcripts were supplied by the researcher as copied text; setup
  screenshots do not independently capture the returned responses.
- The French publication date and meaning of 16 April 1883 remain unresolved.
- The British record was not independently located.
- Identical technical or legal coverage across countries was not established.
- No independent second human verification was performed.
- No international model test was conducted.
- This is not an official GAIA or SimpleQA contribution.
- No overall model ranking or demonstrated red-teaming success is claimed.

## Researcher Contribution and AI Assistance

Sharlyne Agini performed source discovery, patent-data extraction,
scan comparison, archive navigation and researcher scoring.

The AI mentoring assistant suggested research routes and prompts,
reviewed supplied evidence, proposed scoring and assisted with documentation.

Researcher decisions and confirmations are distinguished from
independently captured interface evidence in the test records.

## Reproduction Procedure

1. Open the source PDF and inspect PDF page 2.
2. Review the reference answers and rubric for evaluator preparation.
3. In a fresh test conversation, attach only the PDF.
4. Submit the prompt from the relevant test record without exposing
   the reference answers.
5. Record the model label, interface, settings, date and complete response.
6. Apply the same rubric and document additional unsupported claims.
7. Treat the French archival investigation as a separate research component.

Exact replication of the original runs is limited by undisclosed model
versions and interface-controlled settings.

## Supporting Records

- [Evaluation rubric](pilot-rubric.md)
- [Gemini prompt, response and assessment](tests/pilot-001-gemini.md)
- [Perplexity prompt, response and assessment](tests/pilot-002-perplexity.md)
- [Evidence folder](evidence/)

## Evidence Files

| File | Contents |
|---|---|
| [00446668.pdf](evidence/00446668.pdf) | US patent document supplied in both pilot runs |
| [inpi_initial_patent.PNG](evidence/inpi_initial_patent.PNG) | INPI initial-patent catalogue record |
| [inpi_addition.PNG](evidence/inpi_addition.PNG) | INPI Certificate of Addition catalogue record |
| [french_patent_first_page.PNG](evidence/french_patent_first_page.PNG) | Screenshot of the first scanned image in the initial French patent file |

## Primary-Source Access

- [Rutgers-hosted US patent scan](https://edison.rutgers.edu/images/archive/patents/00446668.PDF)
- [INPI initial-patent catalogue record](https://en-archives.inpi.fr/ark:55749/1ef03e9c15146704a6630050568c1d46.moteur=arko_default_63f395e1547dd)
- INPI initial-patent archive reference: `1BB148852`
- INPI addition archive reference: `1BB148852_1`
- [INPI historical patent collection](https://en-archives.inpi.fr/patents)

Sources were inspected during the research session on 21 October 2026.
The INPI initial-record link was extracted from its saved catalogue HTML;
external availability has not been independently confirmed.
If it does not resolve, search the historical collection for patent
number `148852` and distinguish the initial patent from its addition.

Screenshots are evidence captures, not substitutes for the full archive files.

## Reuse and Attribution

Original portfolio writing and third-party source materials are distinct.
No blanket licence is asserted over third-party scans or screenshots.
Consult the source institutions' applicable reuse terms.
