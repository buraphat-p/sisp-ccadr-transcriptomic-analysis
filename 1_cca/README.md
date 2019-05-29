# /1_cca
# Introduction
This objective of this module was to retrieve data of RNA-seq from basepair and removed batch effect. <br/>

# How to run this code
This folder consits of  "/input", "/code", and "/output". Place input as in "/input" folder, then run "/code/1_cca.RMD". Final result will be shown in "/output" folder.

# /input
This folder consist of two subfloder: "/_basepair" and "/_metadata". Folder /_basepair consist of data table of TPM/count of each cell lines. Folder "/_metadata" consist of meta data for this study.

File list consist of:
-	_basepair/SO_6831/SO_6831_D068.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_D131.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_D138.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_HUCCA1.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_HUCCT1.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_Huh28.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_K055.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_K100.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_K156.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_K213.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_K214.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_MCF7.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_MMNK1.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_RBE.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_SSP25.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_T47D.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_TFK1.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_YSCCC.hg19.counts_gene.txt
-	_basepair/SO_6831/SO_6831_ZR751.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D068.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D068_DAS.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D068_MEK.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D131.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D138.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D138_DAS.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_D138_MEK.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_HUCCA.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_HUCCT.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_HUH28.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K055.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K055_DAS.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K055_MEK.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K100.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K156.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K213.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K213_DAS.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K213_MEK.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_K214.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_MMNK1.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_RBE.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_SSP25.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_TFK1.hg19.counts_gene.txt
-	_basepair/SO_8069/SO_8069_YSCCC.hg19.counts_gene.txt
-	_metadata/metadata_basepair.xlsx
-	_metadata/metadata_cellline.xlsx
-	_metadata/metadata_master.xlsx

Note:<br/>
SO_6831 is batch1.<br/>
SO_8069 is batch2.<br/>

# /output
This folder is a result for /1_cca/code/1_cca.rmd script. There are three files here.<br/>
- Supplementary Figure Supl.fig before_after_combat_.pdf - PCA and tsne before vs after removal of batch effect.<br/>
- repl_fl_combat_ccadr_log2tpm_PB_.csv - pairewise gene expression of 15 CCA in bacth1 VS bacth2.<br/>
- median_log2tpm_combat_PB_.csv - gene expression of 15 CCA after batch effect removal (log2(TPM+1)). <br/>
