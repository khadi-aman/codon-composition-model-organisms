# Comparative Analysis of Codon Composition in Orthologous Genes Across Model Organisms

## Project overview
This repository presents selected results from the 2020 master's dissertation *Comparative Analysis of Codon Composition in Orthologous Genes Across Model Organisms* (Xədicə Müşfiq qızı Bayramova, Institute of Genetic Resources, Azerbaijan National Academy of Sciences).

The dissertation compares codon profiles of 14 genes and their reported orthologs across multiple organisms. Analyses described in the thesis include relative synonymous codon usage (RSCU), pairwise codon-profile correlations, and comparisons of GC3% and AT3%.

## Included results
- `results/rscu_values_long.csv`: RSCU values recovered from the embedded data of the 14 RSCU charts in the Word dissertation.
- `results/correlation_*.csv`: correlation matrices transcribed from dissertation tables.
- `results/correlation_summary_by_gene.csv`: minimum, maximum and mean pairwise correlations calculated from the extracted correlation matrices.
- `figures/stat3_rscu_heatmap.png`: heatmap of STAT3 ortholog RSCU values from the dissertation chart.
- `figures/stat3_correlation_heatmap.png`: STAT3 codon-profile correlation matrix from the dissertation table.
- `figures/correlation_ranges_by_gene.png`: range summary calculated from the extracted pairwise correlations.

## Main findings reported in the dissertation
The dissertation's conclusion states that orthologs from genetically closer species generally showed higher codon-profile correlations, while more distant species showed lower or sometimes negative correlations. The thesis also reports that closely related species tended to show more similar RSCU patterns, and that most of the studied orthologs favored optimal codons with a higher GC content at the third codon position (GC3%) than AT content (AT3%).

These are summaries of the thesis's stated conclusions, not a new independent re-analysis of the underlying sequences.

## Methods and source
The dissertation reports sequence retrieval from NCBI/Ensembl, codon profile extraction, correlation analysis, RSCU calculation using CAIcal, and comparisons prepared in Excel. Correlation matrices and RSCU chart series in this repository were extracted from the supplied DOCX file.

## Important data limitations
- The supplied dissertation file contains embedded RSCU chart data and correlation tables, which are included here.
- A standalone table of numerical CAI results was not identified in the inspected document. CAI is described in the methods, but no CAI result file is included.
- A clearly documented, study-specific UPGMA tree/result was not identified in the inspected document. No tree is fabricated here.
- GC3%/AT3% conclusions are stated in the thesis, but a complete numerical GC3%/AT3% dataset was not identified in the extracted tables/charts. A corresponding numerical CSV/figure should be added only if the original values can be recovered from the dissertation's figures/appendices or source spreadsheets.
- Correlation coefficients are reported as present in the thesis tables; this repository does not independently verify the original sequence selection, orthology assignments, or statistical significance.

## Repository structure
```text
data/       # Source-data notes
results/    # Extracted numerical tables
figures/    # Visualizations from extracted thesis data
docs/       # Methods and provenance notes
```

## Reproducibility note
The figures were generated from values embedded in the supplied Word document. No raw FASTA sequences, full analysis scripts, or original Excel workbooks were included with this DOCX. Therefore, this is a transparent presentation of thesis results, not a fully reproducible end-to-end bioinformatics pipeline.
