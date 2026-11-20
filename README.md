# Rigorous ceilings on phonon-mediated pairing: a map from Eliashberg theory to the Holstein model

Davis Rens  
SuperMatics Inc.  
[ORCID 0000-0001-5839-5197](https://orcid.org/0000-0001-5839-5197)

Paper DOI: [10.5281/zenodo.24406996](https://doi.org/10.5281/zenodo.24406996).  
Source repository: https://github.com/SuperMatics-Inc/phonon-pairing-ceiling-map

## Scope and evidence

The preprint collects released upper bounds on phonon-mediated pairing into one map and states the missing step as a conjecture. In linearized Eliashberg theory it records successive moment ceilings, with coefficients 0.2140146706, 0.19544330695, and then 0.1860593214 and 0.1887345454 on centered and causal branches of the stated finite-channel classes. For the spinful square-lattice Holstein model it records an implicit two-thirds-power clustering threshold in the phonon frequency and a frequency-uniform pair-temperature ceiling proportional to t squared over U for the on-site pair field, and takes the smaller of the two as a regime map. A low-frequency strip remains in which neither proved route supplies a linear-in-frequency ceiling. The remaining determinantal, gap-conditioned and defect-insertion routes are summarized with their own limits. The linear step is stated strictly as a conjecture.

Nothing here is a many-body transition temperature, a measurement, or a claim about a material. The paper makes no prediction about realized pair order and no claim about patentability.

## Contents and replay

- `paper/` contains the publication-metadata-filled manuscript source and its bibliography.
- `ADMITTED.sha256` records the raw-byte hashes of the admitted source set. Its `paper/main.pdf` entry names the reviewed build retained in release custody; that file is not included in this repository.
- `source-delta.diff` shows the admitted-to-release difference in `paper/main.tex` and `paper/refs.bib`. It adds the two companion citations requested by the manuscript review, the title-block macros and the date line that carry the article DOI and the repository URL. No theorem, constant, or scope sentence changed.
- `MANIFEST.sha256` pins each file in this repository except itself.

This paper ships no replay and has no supplement record. Every quantitative statement it uses is quoted from a companion record whose certificate or replay lives in that companion's repository, and its own printed numbers are closed-form values, so there is no new finite computation to replay. The printed decimals were recomputed independently during the manuscript review.

The manuscript can be built from `paper/` with Tectonic:

```sh
(cd paper && tectonic --keep-logs main.tex)
sha256sum -c MANIFEST.sha256
```

The GitHub Actions workflow checks the source manifest, builds the PDF with Tectonic, and checks the page count, the link targets, the authorship lines, and the disclosure text.

## Licenses and provenance

The manuscript text in `paper/` is distributed under CC-BY-4.0 through the paper record. The repository documentation uses Apache-2.0.

AI agents generated the proofs, code and drafts under D. Rens' direction. Separate AI agents did the independent reviews. This preprint has not been peer reviewed.
