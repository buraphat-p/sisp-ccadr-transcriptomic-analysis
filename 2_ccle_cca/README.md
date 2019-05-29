# /2_ccle
# Introduction
This objective of this module was to retrieve data of RNA-seq from CCLE database and combined with our data. Then, normalization of both data set was done.

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

This folder consist of: <br/> 
- "EMBL_EBI_organ.tsv": serve as metadata for cell line cancer origin (by organ) <br/>
- "E-MTAB-2770-query-results.tpms.tsv": serve as raw TPM of CCLE <br/>

File list consist of:
- "/_metadata": folder for metadata
-	_metadata/metadata_basepair.xlsx
-	_metadata/metadata_cellline.xlsx
-	_metadata/metadata_master.xlsx
-	E-MTAB-2770-query-results.tpms.tsv
-	EMBL_EBI_organ.csv

# /output
This folder consist of: <br/> 
- "cca.predict2019-05-25.csv":result of kkn prediction score for our CCA.<br/> 
- "result.cca2019-05-25.csv":result of kkn prediction score for our CCA.<br/> 
- "tsne_ccle_2019-05-25.pdf": result of tsne figure.<br/> 
- "tsne_ccle_2019-05-25.png": result of tsne figure.<br/> 
- "tsne_coordination_cca_ccle_2019-05-25.csv": coordination for tsne plot
