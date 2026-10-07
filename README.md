# Somatic oncogenicity worksheet

**Built by Dr Murphy Sun**

A scoring worksheet for classifying the oncogenicity of somatic variants using the
ClinGen/CGC/VICC standards. Tick the evidence criteria a variant meets; the worksheet
sums the points, applies the classification thresholds, and drafts the justification
paragraph for your report.

**Use it here: https://viscaragold.github.io/oncogenicity-worksheet/**

One HTML file. No install, no account, no network. Download it and it works offline.

---

## Why this exists

Applying the ClinGen/CGC/VICC criteria by hand is slow and error-prone in a specific way:
the arithmetic is trivial, but the mutual exclusions are scattered through the Comments
column of the source tables and easy to miss, and writing a consistent justification for
every variant is what actually consumes the afternoon.

This worksheet does the mechanical parts and leaves every judgement to you.

## What it does

- All 17 criteria — 12 oncogenic, 5 benign — with the full criterion text and caveats
- **Exclusions enforced.** Apply OS1 and OS3, OM1 and OM4 grey out with the reason shown.
  Apply OVS1 and OM2 greys out.
- **Hotspot tiers are mutually exclusive.** OS3, OM3 and OP3 are separated by sample
  counts, so a variant falls in exactly one. Likewise SBVS1 and SBS1 at the 5% and 1%
  gnomAD thresholds.
- **Downgrading supported.** OVS1, OS2, OM1, OM2, OM4 and SBS2 may be dropped to a lower
  evidence level where evidence is partial, as the standards permit. The justification
  records that a criterion was downgraded.
- **Per-criterion guidance.** Each row states what you are looking for and links only the
  resources relevant to that criterion.
- **Justification written for you** — every code, level, points, total, classification and
  the citation. Editable before use.

## Verification

The scoring reproduces both worked examples in the source publication:

| Variant | Criteria | Points | Classification |
|---|---|---|---|
| KRAS p.Arg164Gln | SBS2 downgraded to supporting, OP1 | 0 | Uncertain significance |
| BRAF p.Gly469Glu | OS2, OP1, OP3, OP4 | +7 | Likely oncogenic |

All five classification thresholds were checked at their boundaries.

## Privacy

The page makes no network requests and uses no cookies or browser storage. Nothing you
type is transmitted or retained. The resource buttons construct a URL and open it in a new
tab — ordinary navigation performed by you, not a background API call.

For laboratory use, download the file and open it locally rather than using the hosted
copy, so the tool is not dependent on internet access.

## Scope and limitations

This SOP covers somatic single nucleotide variants and small insertions or deletions,
including deletions within a single gene. It is **not** for germline cancer predisposition
variants, fusions, copy number variants, or other chromosomal rearrangements.

Oncogenicity and clinical actionability are different questions. Classify oncogenicity
first, then assess actionability under AMP/ASCO/CAP.

OM4 requires comparison of amino acid distances (Grantham, Epstein or Miyata). No distance
matrix is built in; look the values up and record your comparison.

**This worksheet does not assess evidence.** It records your assessment, performs the
arithmetic and drafts the wording. Every judgement remains yours. It is a reference aid,
not a diagnostic device, and routine clinical decisions should not be made on variants of
uncertain significance.

## Source

Horak P, Griffith M, Danos AM, et al. Standards for the classification of pathogenicity of
somatic variants in cancer (oncogenicity): joint recommendations of Clinical Genome
Resource (ClinGen), Cancer Genomics Consortium (CGC), and Variant Interpretation for Cancer
Consortium (VICC). *Genetics in Medicine*. 2022;24(5):986–998.
doi:[10.1016/j.gim.2022.01.001](https://doi.org/10.1016/j.gim.2022.01.001)

Criterion text, point weights, mutual exclusions and classification thresholds are
transcribed from Tables 2 and 3 and Figure 1 of that publication. Verify the transcription
against your own copy before clinical use.

---

© Dr Murphy Sun. Released under the MIT Licence.
