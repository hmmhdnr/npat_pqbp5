# A custom code to confirm SNP/GWAS data and polyQ disease association dataset in our research paper entitled "PQBP5/NOL10 maintains and anchors the nucleolus under physiological and osmotic stress conditions".

## datasets
A source data file of this analysis is attached in this repository (named "Confirmation_of_SNP_GWAS_data_and_polyQ_disease_association_dataset.xlsx").
It consists of two sheets containing search results of SNPs of PQBP5 and related research papers as below:
* a list of SNPs in PQBP5/NOL10 acquired from dbSNP ( https://www.ncbi.nlm.nih.gov/snp/ )
* a list of research papers relating to SNPs and CAG repeats searched from PubMed ( https://pubmed.ncbi.nlm.nih.gov/ )

## custom codes
A custom function in Microsoft Excel was used to check wherther SNPs mentioned in research papers are included in a list of SNPs from dbSNP (see "query_and_result" datasheet in the atached Excel file).
```
=IF(COUNTIF(SNPs!A:A,A2) > 0, "yes", "no")
```
