# Bioinformatics Analysis of Helicobacter pylori Virulence Factors

## Project Overview
This project presents a small bioinformatics and data science analysis of *Helicobacter pylori* virulence genes, with a particular focus on the **CagA protein** and its **EPIYA phosphorylation motifs**, which are key determinants of pathogenicity and gastric disease severity.

The workflow integrates sequence analysis, motif detection, data structuring, and visualization using Python and standard UNIX tools.

---

## Objectives
- Translate *H. pylori* virulence gene sequences into protein sequences
- Identify and locate EPIYA motifs within the CagA protein
- Extract flanking amino acid contexts around EPIYA motifs
- Quantify gene and protein lengths
- Visualize virulence features using plots and heatmaps

---

## Tools & Technologies
- Python 3
- Biopython
- Pandas
- Matplotlib
- UNIX command-line tools (grep, sed, wc)
- macOS Terminal

---

## Dataset
- *Helicobacter pylori* virulence gene sequences (FASTA format)
- Focus gene: **cagA**

---

## Workflow Summary

### 1. Sequence Translation
- The *cagA* nucleotide sequence was translated into a protein sequence.
- Protein length: **1186 amino acids**

### 2. EPIYA Motif Detection
- Two EPIYA motifs were identified in the C-terminal region of CagA.
- Motif positions and surrounding amino acid contexts were extracted.

### 3. Feature Extraction
The following features were quantified:
- Nucleotide length
- Estimated protein length
- EPIYA motif count

### 4. Data Visualization
- Bar plot of protein lengths for virulence genes
- Heatmap of virulence-associated features

---
## Results & Visualizations

### Virulence Feature Heatmap
![Virulence feature heatmap](figures/virulence_feature_heatmap.png)
Figure 1. Heatmap of H. pylori virulence-associated features.
Normalized virulence features derived from gene and protein sequences are visualized using a heatmap. Differences in color intensity highlight variation in feature abundance, allowing comparative assessment of virulence determinants across the dataset.
### Gene Length Distribution
![Virulence gene lengths](figures/virulence_gene_lengths.png)
Figure 2. Length distribution of H. pylori virulence genes.
The figure depicts the nucleotide length distribution of identified virulence genes, revealing heterogeneity in gene size that may reflect functional and evolutionary differences among virulence factor
### Protein Length Bar Plot
![Protein length barplot](figures/protein_length_barplot.png)
Figure 3. Protein length of the H. pylori CagA virulence factor.
The translated CagA protein length is visualized, emphasizing its extended structure. Such length variability is biologically significant, as the C-terminal region contains EPIYA motifs involved in host-cell signaling and pathogenicity.
### Feature Correlation Heatmap
![Virulence correlation](figures/virulence_correlation.png)
Figure 4. Correlation matrix of virulence-associated features.
Pairwise correlations between quantified virulence features are shown. Strong correlations indicate interdependent biological properties, while weaker associations suggest distinct contributions to H. pylori pathogenicity.
## Key Results
- **CagA contains 2 EPIYA motifs**, consistent with highly virulent *H. pylori* strains.
- EPIYA motifs are clustered in the C-terminal region, supporting their role in host-cell signaling disruption.
- CagA is among the longest virulence-associated proteins analyzed.

---

## Output Files

### Figures (`figures/`)
- `protein_length_barplot.png`
- `virulence_feature_heatmap.png`
- `virulence_correlation.png`

### Tables (`tables/`)
- `virulence_numeric_matrix.tsv`
- `statistical_summary.tsv`

### Text Results (`results/`)
- `EPYIA_positions.txt`
- `EPYIA_context.txt`

---

## Biological Significance
EPIYA motifs in CagA undergo phosphorylation after host-cell entry, triggering aberrant signaling pathways linked to gastric inflammation, ulcers, and carcinoma. The number and positioning of EPIYA motifs are therefore critical virulence determinants.

---

## Conclusion
This project demonstrates how bioinformatics and data science techniques can be combined to extract biologically meaningful insights from bacterial genome sequences using lightweight computational workflows.

---

## Author
Dr Ali Ahmad
MBBS
MSc Clinical & Molecular Microbiology / Drug Discovery & Development  



