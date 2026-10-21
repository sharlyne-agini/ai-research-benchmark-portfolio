# ENG-001 — Historical Patent Dates and AI Evidence Assessment

Author: Sharlyne Agini
Research date: 21 October 2026
Status: Research closed with documented limitations; publication preparation pending.
Independent research with AI-assisted mentoring and review.

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

## Verified Findings

| Record | Explicitly labelled information |
|---|---|
| US446668, PDF page 2 | Application filed 7 August 1882; serial 68,651 |
| US446668, PDF page 2 | US Letters Patent dated 17 February 1891 |
| US446668, PDF page 2 | French patent 148,852 cited as dated 16 April 1883 |
| INPI 1BB148852 | Initial patent filing date: 9 May 1882 |
| INPI 1BB148852_1 | Certificate of Addition filing date: 26 December 1882 |

INPI identifies the applicant as EDISON Thomas-Alva. Its initial record
concerns improvements to electric arc lighting and regulating mechanisms.
The first scanned image also contains the 9 May 1882 deposit reference.

## Main Conclusion

A date associated with a foreign patent in a US specification must not
automatically be classified as its filing date.

The French initial-patent filing date is explicitly recorded as
9 May 1882. The meaning of the US-cited 16 April 1883 date remains
unresolved. Different event dates do not by themselves demonstrate
contradictory records.

## AI Document-Evaluation Pilot

I supplied US446668 to Gemini in Chrome (Auto mode) and Perplexity
(Learn step by step mode), using five equivalent questions about
identifiers, dates and evidence limits.

Both supplied responses provisionally scored 10/10 under the pilot rubric.
No core factual failure was identified.

These runs tested single-document extraction and evidence assessment.
They did not test the subsequent French archive investigation.

## Limitations

- One document and one recorded response per interface.
- Exact underlying model versions were not disclosed.
- Web search was prohibited by the prompt; actual tool use was not verified.
- The rubric was developed after the Gemini response.
- Additional page-1 references in responses remain unchecked.
- Uploaded test-record files still contain transcript placeholders.
- The French publication date and meaning of 16 April 1883 remain unresolved.
- Identical technical or legal coverage across countries was not established.
- No independent second human verification was performed.
- This is not an official GAIA or SimpleQA contribution.
- No overall ranking of models or red-teaming success is claimed.

## Researcher Contribution

Source discovery, patent-data extraction, scan comparison, archive
navigation, identification of date-event ambiguity, and rubric-based
assessment, with AI assistance documented.

## Supporting Records

- [Rubric](pilot-rubric.md)
- [Gemini pilot](tests/pilot-001-gemini.md)
- [Perplexity pilot](tests/pilot-002-perplexity.md)

## Primary-Source Access

- US scan:
  https://edison.rutgers.edu/images/archive/patents/00446668.PDF
- INPI initial-patent archive reference: 1BB148852
- INPI addition archive reference: 1BB148852_1
- INPI historical collection:
  https://en-archives.inpi.fr/patents

Evidence reviewed includes the source PDF, INPI catalogue screenshots,
the initial-patent viewer screenshot and a saved INPI catalogue HTML page.
