# This stie is under constructing.
# sisp-ccadr-transcriptomic-analysis
# Introduction
This Github contributed Transcriptomic analysis of 15 human cholangiocarcinoma cell lines and 1 human bile duct immortalized cell line. The data were available as following: 
<GEO>, <SRA>.

# Site Structure 
This site is compose of folder: <br/>
- /1_cca :to retrieve data of RNA-seq from basepair and removed batch effect.
- /2_ccle_cca :  to retrieve data of RNA-seq from CCLE database and combined with our data. Then, normalization of both data set was done.
- /2_tsne : to re-plot tsne plot with the same setting and seed from /2_ccle_cca/code/2_ccle_cca.RMD
- /3_heatmap_by_ccle_organ : to compare our CCA (15 cell lines) vs CCLE by origin of cell lines (organ) by using correlation plot, then normalization with z-score.
- /4_fusion : to retrieve data of fusion genes from Basepair and analysis them <br/>

Each folder consist of 3 subfolder: "/code", "/input", and "/output". To re-run figure, place input data in "/input" folder, and run the code in "/code" folder. The results will be placed in "/output" folder. 

# Reference
<REF>
