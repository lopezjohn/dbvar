# dbVar non-redundant structural variation datasets for Insertion variants

## Work in progress – Data subject to change

## Last updated:
06/22/18

## Link to FTP site:

[https://ftp.ncbi.nlm.nih.gov/pub/dbVar/sandbox/sv_datasets/nonredundant/insertions/](https://ftp.ncbi.nlm.nih.gov/pub/dbVar/sandbox/sv_datasets/nonredundant/insertions/#github)

# Introduction

The non-redundant structural variants, "NR SVs", of type "insertion" are in these
files on the FTP site:

&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_insertions.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_insertions.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_insertions.acmg_genes.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_insertions.acmg_genes.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_insertions.bed.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_insertions.bed.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_insertions.bedpe.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_insertions.bedpe.gz__  

The variant types in the NR "aggregated insertions" file are:

* alu_insertion
* insertion
* line1_insertion
* mobile_element_insertion
* novel_sequence_insertion
* sva_insertion

# Records in the aggregated_insertions files

Records in the aggregated_insertions files contain the following tab-separated fields.

| chr | outermost_start | outermost_stop | SV_count | variant_type | method | analysis | platform | study | SV |


## Example record 1:

chr | outermost_start | outermost_stop | SV_count | variant_type | method | analysis | platform | min_insertion_length | max_insertion_length | study | SV
----|-----------------|----------------|----------|--------------|--------|----------|----------|---|---|----|---
1 | 370037 | 370038 | 1 | insertion | Sequencing | Local_sequence_assembly | NA | 94 | 94 | Fan2017 | nssv14027289

### Explanation:

* The non-redundant coordinates for this record in dbVar are chr1, with
an outermost start of 370037 and outermost stop of 370038.

* The SV_count of 1 indicates there is only one SV with an exact match to the
given placement.  This count does not include SVs with a partial match.

* The variant_call_type is "insertion".

* The method of "Sequencing" and the analysis of "Local_sequence_assembly"
indicate how the variant was evaluated.

* 94 indicates the minimum insertion length, which is the same as the maximum insertion length since there is only one SV at this set of NR coordinates.

* NA indicates the no platform was specified for this variant.

* Fan2017 is the study name as found in dbVar.

* The dbVar variant_accession is "nssv14027289".

* URLs using the study name or variant_accession can be created to access the data
in dbVar, e.g.:
https://www.ncbi.nlm.nih.gov/dbvar/?term=Fan2017  
https://www.ncbi.nlm.nih.gov/dbvar/?term=nssv14027289

* From the latter page you may click on the "Variant Region ID" on the left to see
the variant's region in the NCBI Variation Viewer at:
https://www.ncbi.nlm.nih.gov/dbvar/variants/nsv3056167/

## Example record 2:

chr | outermost_start | outermost_stop | variant_count | variant_type | method | analysis | platform | min_insertion_length | max_insertion_length | study | variant
----|------------------|----------------|----------|--------------|--------|----------|----------|-------|--|--|---
1 | 5874241 | 5874241 | 2 | alu_insertion;insertion | Sequencing;Sequencing | Split_read_and_paired-end_mapping;de_novo_sequence_assembly | HiSeq 2000;Illumina HiSeq 2000 | 52 | 243 | Gardner2017;Besenbacher2014 | nssv14046119:essv16474703

### Explanation:

* This is a more complicated example insertion NR record containing multiple
variants with multiple types, methods, and analyses from multiple studies, using
platforms with different names, and having different insertion_lengths.

# Questions or feedback

* Please email dbvar@ncbi.nlm.nih.gov or create an issue on this GitHub page.

# Thanks!

Thanks for your interest in the dbVar human "non-redundant structural variations" (nr SVs)
data files from NCBI.

Please check back for updates soon.
