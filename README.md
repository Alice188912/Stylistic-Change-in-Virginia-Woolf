# Stylistic Change in Virginia Woolf — Research Data

Curated corpus and stylometry outputs for the Virginia Woolf stylistic-change project. Only material directly relevant to the final essay is kept here: coursework handouts, the Conrad comparison corpus, and the essay draft itself have been removed.

## Contents

| Directory | Files | Description |
| --- | ---: | --- |
| `02-corpora/woolf/` | 14 | Plain-text editions of Virginia Woolf's novels and short stories (1915–1941) |
| `03-analysis-outputs/csv/` | 10 | Cluster-analysis edge and node lists generated with stylo (Classic Delta, consensus clustering, MDS) |
| `03-analysis-outputs/figures/` | 13 | Correspondence analysis, PCA and MDS plots, plus keyword word clouds |
| `03-analysis-outputs/tables/` | 10 | Frequency lists, keyword and KWIC results, distance tables, and the stylo configuration |

Total: 47 data files, plus this README and `.gitignore`.

## Curation notes

- The corpus contains Woolf texts only. The Conrad corpus, used for separate coursework experiments, was removed.
- Course manuals, assignments, reading lists and software handouts were removed.
- `Keyword_results.txt` was excluded: it reports keywords for Conrad's *Nostromo*, not for Woolf. The retained keyword and KWIC files all target Woolf texts.
- Two texts (`Monday or Tuesday 1921.txt` and `The-Waves 1931.txt`) appeared identically in both the course corpus and the essay materials, so one copy of each was kept.
- Original filenames are preserved for traceability, including embedded analysis parameters such as MFWs, culled value and clustering threshold.
- The essay draft is not included in this repository.
- The original source folder on the local machine was left untouched; this repository is a curated copy.

## Reproducing the analyses

The outputs were produced with R's **stylo** package and **AntConc**. Analysis parameters are recorded in the filenames and in `03-analysis-outputs/tables/stylo_config.txt`.
