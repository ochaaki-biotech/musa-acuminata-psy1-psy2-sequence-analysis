# musa-acuminata-psy1-psy2-sequence-analysis
Comparative bioinformatics analysis of PSY1 and PSY2 phytoene synthase gene sequences in Musa acuminata using NCBI Nucleotide database retrieval, sequence metadata analysis and BLAST nucleotide alignment.
# Comparative Sequence Analysis of PSY1 and PSY2 in *Musa acuminata*

[![Course](https://img.shields.io/badge/Course-Recombinant%20DNA%20Technologies-blue)](https://kab.ac.ug/)
[![Field](https://img.shields.io/badge/Field-Bioinformatics-green)]()
[![Organism](https://img.shields.io/badge/Organism-Musa%20acuminata-orange)]()
[![Project](https://img.shields.io/badge/Project-Academic%20Practical-lightgrey)]()

## 1. Project Overview

This repository documents a comparative bioinformatics analysis of two phytoene synthase gene sequences, **PSY1 and PSY2**, from *Musa acuminata* (banana).

The practical was conducted as part of the **Recombinant DNA Technologies** course at Kabale University. It introduces fundamental bioinformatics procedures used to retrieve nucleotide sequences, examine sequence annotations, identify coding regions, and investigate sequence similarity using the Basic Local Alignment Search Tool (BLAST).

The analysis focuses on understanding the sequence characteristics and similarity relationships of PSY1 and PSY2 using publicly available nucleotide sequence records from the National Center for Biotechnology Information (NCBI).

## 2. Aim

To retrieve, examine, and comparatively analyse PSY1 and PSY2 nucleotide sequences from *Musa acuminata* using NCBI sequence databases and BLAST.

## 3. Specific Objectives

- Retrieve PSY1 and PSY2 nucleotide sequences from the NCBI database.
- Examine sequence metadata, including accession numbers, sequence lengths, and annotations.
- Identify and interpret coding sequence (CDS) information.
- Perform BLAST sequence similarity searches.
- Interpret BLAST results using percentage identity, query coverage, alignment length, gaps, and E-values.
- Compare the sequence characteristics and similarity patterns observed for the two sequences.

## 4. Biological Background

Phytoene synthase (PSY) is an important enzyme involved in the carotenoid biosynthesis pathway. It catalyses the formation of phytoene, an early intermediate in carotenoid production.

Carotenoids are pigments that contribute to the yellow, orange, and red coloration of plant tissues and participate in important biological processes.

Studying PSY gene sequences provides an opportunity to understand gene sequence variation, annotation, and similarity between related nucleotide records.

This practical examines two sequences identified as PSY1 and PSY2 in *Musa acuminata*.

## 5. Tools and Resources

| Tool / Resource | Purpose |
|---|---|
| NCBI Nucleotide | Retrieval of nucleotide sequences |
| NCBI BLASTn | Comparison of nucleotide sequences |
| NCBI RefSeq | Access to curated reference sequence records |
| FASTA format | Storage and representation of nucleotide sequences |
| Web browser | Accessing bioinformatics databases and tools |

## 6. Sequence Information

The two nucleotide records used in the practical are summarised below.

| Feature | PSY1 | PSY2 |
|---|---|---|
| Organism | *Musa acuminata* AAA Group | *Musa acuminata* |
| Gene identifier | PSY1 | PSY2 |
| Sequence type | mRNA | mRNA, partial CDS |
| Accession supplied | XM009388150 | JX195670.1 |
| Sequence length | 1,817 bp | 600 bp |
| CDS information | Positions 352–1644 in the earlier record | `<1..600` |
| Database | NCBI | NCBI |

**Data verification note:** The PSY1 accession information supplied during the practical requires verification. An earlier record was identified as `XM_009388150.3`, while the supplied accession/version was recorded as `XM009388150` / `009388150.1`. The record description also contained a product-name and gene-qualifier inconsistency. These details should be checked against the original NCBI record before treating the accession as final.

## 7. Bioinformatics Workflow

The practical followed these major stages:

1. **Sequence retrieval:** PSY1 and PSY2 nucleotide records were obtained from the NCBI Nucleotide database.
2. **Sequence examination:** The records were examined for accession numbers, sequence lengths, organism information, and annotations.
3. **CDS examination:** Coding sequence information was identified and interpreted from the available annotations.
4. **FASTA preparation:** Nucleotide sequences were used as input for sequence similarity analysis.
5. **BLAST analysis:** BLASTn searches were conducted to identify similar nucleotide sequences in the database.
6. **Result interpretation:** Sequence identity, query coverage, alignment length, gaps, and E-values were examined.
7. **Comparative discussion:** The findings were interpreted in relation to the two sequence records.

## 8. Summary of BLAST Results

### PSY1

The PSY1 analysis identified three high-scoring segment pairs (HSPs) against one predicted *Musa acuminata* AAA Group phytoene synthase 2 chloroplastic-like mRNA record, `XM_065160940.1`.

The reported alignment segments showed approximately 99% sequence identity, with E-values of 0.0, 0.0, and 7e-117, respectively.

These are three alignment segments against one subject sequence, rather than three independent BLAST subject records.

### PSY2

The PSY2 query sequence was 600 bp long. The reported BLAST results included:

| Subject accession | Identity | Query coverage | E-value |
|---|---:|---:|---:|
| JX195670.1 | 100% | 100% | 0.0 |
| XM_065082466.1 | 99% | 100% | 0.0 |
| XM_065125103.1 | 99% | 100% | 0.0 |

The first result represents an exact self-match to the query accession. The other two results are predicted *Musa acuminata* phytoene synthase 2 chloroplastic-like records.

An E-value displayed as 0.0 represents an extremely small value below the displayed precision; it does not mean that the mathematical value is exactly zero.

## 9. Key Bioinformatics Concepts Demonstrated

This practical provides experience with the following concepts:

- **Nucleotide sequence:** An ordered arrangement of DNA or RNA bases.
- **Accession number:** A unique identifier assigned to a sequence record in a biological database.
- **FASTA format:** A standard text format used to represent biological sequences.
- **CDS:** The coding sequence region that is translated into a protein.
- **BLAST:** A tool for identifying regions of similarity between biological sequences.
- **Percentage identity:** The proportion of aligned positions containing identical nucleotides.
- **Query coverage:** The proportion of the query sequence included in an alignment.
- **E-value:** An estimate of the number of alignments of similar quality expected by chance in a database search.
- **HSP:** A high-scoring segment pair representing a locally aligned region between two sequences.

## 10. Repository Structure

The repository is organised to make the practical easy to understand, reproduce, and review.

```text
PSY1-PSY2-Comparative-Sequence-Analysis/
│
├── README.md
│
├── report/
│   └── PSY1_PSY2_Comparative_Sequence_Analysis_Report.pdf
│
├── sequences/
│   ├── PSY1.fasta
│   └── PSY2.fasta
│
├── blast-results/
│   ├── PSY1_BLAST_results.txt
│   └── PSY2_BLAST_results.txt
│
└── references/
    └── database_accessions.txt
```

*Note: This is a suggested directory structure. Add the files as they become available and update the names to match the actual repository contents.*

## 11. Limitations and Considerations

- The PSY1 accession and version information needs confirmation against the original NCBI record.
- The PSY2 sequence is described as a partial CDS; conclusions should therefore be limited to the available 600 bp sequence.
- A high BLAST percentage identity indicates sequence similarity but does not, by itself, establish identical biological function.
- The PSY1 HSPs represent separate local alignment regions and should not be interpreted as independent subject records.
- The analysis is based on the sequence records and BLAST outputs available during the practical.

## 12. Conclusion

This practical demonstrates how publicly available nucleotide databases and sequence alignment tools can be used to investigate plant gene sequences.

Through the retrieval, annotation examination, and BLAST comparison of PSY1 and PSY2 sequences from *Musa acuminata*, the exercise develops foundational skills in bioinformatics, sequence interpretation, and comparative molecular analysis.

The project also highlights the importance of accurate accession verification and careful interpretation of sequence similarity results.

## 13. References and Data Sources

1. National Center for Biotechnology Information (NCBI). Nucleotide Database. https://www.ncbi.nlm.nih.gov/nuccore/
2. National Center for Biotechnology Information (NCBI). BLAST: Basic Local Alignment Search Tool. https://blast.ncbi.nlm.nih.gov/Blast.cgi
3. National Center for Biotechnology Information (NCBI). Reference Sequence Database (RefSeq). https://www.ncbi.nlm.nih.gov/refseq/

## 14. Academic Information

**Institution:** Kabale University  
**Course:** Recombinant DNA Technologies  
**Programme:** Bachelor of Science in Biotechnology  
**Academic Level:** Year Two  
**Project Type:** Bioinformatics Practical  
**Student:** Ochaaki Nyarwa Absolom

---

*This repository is an academic learning project documenting practical experience in nucleotide sequence retrieval, annotation, and comparative bioinformatics analysis.*
