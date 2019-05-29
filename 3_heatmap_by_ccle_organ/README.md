# /2_tsne
# Introduction
This objective of this module was to compare our CCA (15 cell lines) vs CCLE by origin of cell lines (organ) by using correlation plot, then normalization with z-score.

# How to run this code
This folder consits of  "/input", "/code", and "/output". Place input as in "/input" folder, then run "/code/3_heatmap_by_ccle_organ.RMD". Final result will be shown in "/output" folder.

# /input
download CCLE-RNA-seq data from EMBL-EBI : 934 cell lines
from https://www.ebi.ac.uk/gxa/experiments/E-MTAB-2770/Results
at 20180427 <br/> 

934 cell lines 
Excluded OCI-Ly3 - https://web.expasy.org/cellosaurus/CVCL_8800
Cellosaurus OCI-Ly3 (CVCL_8800) <br/> 

However, cell line origin (annotation) was retrived from https://ocg.cancer.gov/programs/ctd2/data-portal at 20180428. <br/>

REF https://ocg.cancer.gov/ctd2-data-project/translational-genomics-research-institute-quantified-cancer-cell-line-encyclopedia#TGenCCLERNAseq <br/>

File list consist of:
-	_metadata/metadata_basepair.xlsx
-	_metadata/metadata_cellline.xlsx
-	_metadata/metadata_master.xlsx
-	cgHub_CCLE_RNA-seq_metadata_summary.txt: organ annotation from ctd2
-	EMBL_EBI_organ.csv: organ annotation from EMBL-EBI 
-	combine_metadat_edited.csv: final organ annotation of CCLE (combine from EMBL-EBI + ctd2 + mannual)

This module also require 15 cca gene expression and liver-pancreas annotation from folder: <br/>

/2_tsne/output <br/>
- /ccle_cca_expression_table_2019-05-29.csv: z-score nomalized expression of CCLE + our CCA

# /output
This folder consist of: <br/> 
- cca_ccle_corr_heatmap2019-05-29.pdf: z-score normalized correlation
- cca_ccle_corr_heatmap2019-05-29.png: z-score normalized correlation plot figure
