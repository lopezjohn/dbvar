# dbVar non-redundant structural variation datasets for Deletion variants

## Work in progress – Data subject to change

## Last updated:
06/22/18

## FTP Link:

[https://ftp.ncbi.nlm.nih.gov/pub/dbVar/sandbox/sv_datasets/nonredundant/deletions/](https://ftp.ncbi.nlm.nih.gov/pub/dbVar/sandbox/sv_datasets/nonredundant/deletions/#github)

# Introduction

The non-redundant structural variants, "NR SVs", of type "deletions" are in these  
files on the FTP site:

&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_deletions.tsv.gz__   
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_deletions.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_deletions.acmg_genes.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_deletions.acmg_genes.tsv.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_deletions.bed.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_deletions.bed.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh38.nr_deletions.bedpe.gz__  
&nbsp;&nbsp;&nbsp;&nbsp;__GRCh37.nr_deletions.bedpe.gz__  

The variant types in the NR "deletions" file are:

* alu_deletion
* copy_number_loss
* deletion
* herv_deletion
* line1_deletion
* sva_deletion

# Records in the aggregated_deletion_loss files

Records in the aggregated_deletion_loss files contain the following tab-separated fields.

| chr | outermost_start | outermost_stop | variant_count | variant_type | method | analysis | platform | study | variant | clinical_assertion | clinvar_accession


## Example record 1:
  
chr | outermost_start | outermost_stop | variant_count | variant_type | method | analysis | platform | study | variant | clinical_assertion | clinvar_accession  
----|-----------------|----------------|---------------|--------------|--------|----------|----------|-------|---------|--------------------|------------------  
X | 153293294 | 153296201 | 1 | deletion | Curated | Curated | NA | LSDB_submitted_variants | nssv7487065 | Pathogenic | SCV000222455

### Explanation:

* The non-redundant coordinates for this record in dbVar are chr1, with
an outermost start of 10001 and outermost stop of 1535693.

* The SV_count of 1 indicates there is only one SV with an exact match to the
given placement.  This count does not include SVs with a partial match.

* The variant_call_type is "deletion".

* The method and the analysis indicate how the one variant was evaluated.

* NA indicates the no platform was submitted for this variant.

* LSDB_submitted_variants is the study name as found in dbVar.

* The dbVar variant_accession is "nssv7487065".

* The clinical_significance is "Pathogenic"

* The variant has an accession in ClinVar of SCV000222455

* URLs using the study name accession or variant_accession can be created to access the data
in dbVar, e.g.:
https://www.ncbi.nlm.nih.gov/dbvar/studies/nstd103/  
https://www.ncbi.nlm.nih.gov/dbvar/?term=nssv7487065

* From the latter page you may click on the "Variant Region ID" on the left to see
the variant's region in the NCBI Variation Viewer at:
https://www.ncbi.nlm.nih.gov/dbvar/variants/nsv1197457/

* The SCV accession can be used to find the record in ClinVar by searching on ClinVar's home page:
https://www.ncbi.nlm.nih.gov/clinvar/

## Example record 2:

chr | outermost_start | outermost_stop | variant_count | variant_type | method | analysis | platform | study | variant | clinical_assertion | clinvar_accession  
----|-----------------|----------------|---------------|--------------|--------|----------|----------|-------|---------|--------------------|------------------
1 | 72300544 | 72346418 | 7 | copy_number_loss;deletion | Oligo_aCGH;Sequencing | Probe_signal_intensity;Read_depth | Agilent 24M aCGH;Illumina IIx | Park2010;Ju2010 | nssv1423530:nssv1425248:nssv1428032:nssv1428830:nssv1434173:nssv1439464:nssv1420391

### Explanation:

* This is a more complicated example deletion NR record containing multiple
variants with multiple types, methods, and analyses from multiple studies, using
multiple platforms.  This record does not contain clinical_significance or a 
ClinVar accession.

# Questions or feedback

* Please email dbvar@ncbi.nlm.nih.gov or create an issue on this GitHub page.

# Thanks!

Thanks for your interest in the dbVar human "non-redundant structural variations" (nr SVs)
data files from NCBI.

Please check back for updates soon.
