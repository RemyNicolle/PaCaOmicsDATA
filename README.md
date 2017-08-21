# PaCaOmicsDATA
Processed dataset of the PaCaOmics clinical trial (NCT01692873) study on pancreatic adenocarcinoma patient-derived xenografts.



All datasets are Tabulation Seperated Values (.tsv) file. Large files are also gzipped.

#### RNA

RNAseq-based transcriptome data is available for the human/tumor compartment as well as the murine/stromal compartment. SMAP (github.com/RemyNicolle/SMAP) was used to seperate specie-specific RNAseq reads.

Datasets are available as either raw counts, to be able to use any differential analysis method (Limma-Voom with Upper-Quartile normalization in the original study), or normalized counts.

Another dataset is available to be able to compare expression levels between human/tumor and murine/stroma.

- Human-Tumor_Transcriptome : Upper-Quartile normalized Human genes.
- Human-Tumor_rawcount_Transcriptome : Raw counts of Human genes
- Murine-Stroma_Transcriptome : Upper-Quartile normalized Murine genes.
- Murine-Stroma_rawcount_Transcriptome : Raw counts of Murine genes
- ComparableTumorStroma_Transcriptome : Concatenated quantile co-normalised Human and Murin reads after seperate RPKM normalization. 
- miRseq: Upper-Quartile normalized Human micro-RNA sequencing.



#### DNA

- Methylation : Illumina Infinium Human Methylation 450K BeadChip, normalized Beta-Value. Only SNP-clear probes value are shown and were used in the study.
- CopyNumber : Illumina Infinium HumanCode-24 BeadChip SNP arrays Copy Number values. 
- somaticMutations : Whole-Exome sequencing somatic non-synonymous mutations table.



#### Raw data

Genotype data from whole-exome sequencing has been deposited at the European Genome-phenome Archive (EGA,[ ](http://www.ebi.ac.uk/ega/)<http://www.ebi.ac.uk/ega/>), which is hosted by the EBI, under accession number EGAS00001001928. Other datasets are available on ArrayExpress (<http://www.ebi.ac.uk/arrayexpress>): SNP data is available under accession E-MTAB-5006, Methylation data is available under accession E-MTAB-5008, miRNA sequencing data is available through under accession E-MTAB-5018 and mRNA sequencing data is available under accession E-MTAB-5039. 