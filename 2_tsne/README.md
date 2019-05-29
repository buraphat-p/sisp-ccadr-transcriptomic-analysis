# /2_tsne
# Introduction
This objective of this module was to re-plot tsne plot base on output from /2_ccle_cca/code/2_ccle_cca.RMD

# How to run this code
This folder consits of  "/input", "/code", and "/output". Place input as in "/input" folder, then run "/code/2_ccle_cca.RMD". Final result will be shown in "/output" folder.

# /input
download CCLE-RNA-seq data from EMBL-EBI : 934 cell lines
from https://www.ebi.ac.uk/gxa/experiments/E-MTAB-2770/Results
at 20180427 <br/> 

934 cell lines 
Excluded OCI-Ly3 - https://web.expasy.org/cellosaurus/CVCL_8800
Cellosaurus OCI-Ly3 (CVCL_8800) <br/> 

"Caution: A cell line, now termed GNE-587170 (CVCL_AT69), was mistakenly distributed by OCI to a number of groups under the designation OCI-Ly-3, the origin of that cell line is now known." <br/> 
"Problematic cell line: Misidentified. This cell line was mistakenly distributed by OCI to a number of groups as being OCI-Ly-3 (CVCL_8800). The real identity of this cell line is not known. From personal communication of Neve R." <br/> 

File list consist of:
- "/_metadata": folder for metadata
-	_metadata/metadata_basepair.xlsx
-	_metadata/metadata_cellline.xlsx
-	_metadata/metadata_master.xlsx
-	E-MTAB-2770-query-results.tpms.tsv : serve as metadata for cell line cancer origin (by organ)
-	EMBL_EBI_organ.csv: serve as raw TPM of CCLE

This module also require 15 cca gene expression and liver-pancreas annotation from folder: <br/>
/1_cca/output <br/>
filename: 
- median_log2tpm_combat_PB_.csv

/2_ccle_cca/output <br/>
- result.cca2019-05-25.csv - annotation liver-pancreas like

# /output
This folder consist of: <br/> 
-	ccle_cca_expression_table_2019-05-29.csv - expression of ccle + our 15 our cca + 3 our breast cancer + 1 MMNK-1 with batch effect removal and z-score normalization, annotation of organ, origin, cell name, and database.
-	tsne_ccle_2019-05-29.pdf - tsne plot
-	tsne_ccle_2019-05-29.png - tsne plot
-	tsne_coordination_cca_ccle_2019-05-29.csv - co-ordination (xy) of tsne (tsne1 - tsne2). 
