# /4_fusion
# Introduction
This objective of this module was to retrieve data of fusion genes from Basepair and analysis them.

# How to run this code
This folder consits of  "/input", "/code", and "/output". Place input as in "/input" folder, then run "/code/4.1_fusion_loaddata.RMD" first. Finally, run "/code/4.2_fusion_analysis_heatmap.RMD. Final result will be shown in "/output" folder.

# /input
Input consist of: <br/>
1. Fusion list from basepair (deFuse - McPherson et al., 2011)
-	_basepair/fusion_defuse/SO_6831/SO_6831_D068.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D068.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D068.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D131.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D131.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D131.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D138.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D138.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_D138.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_HUCCA1.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_HUCCA1.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_HUCCA1.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_HUCCT1.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_HUCCT1.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_HUCCT1.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_Huh28.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_Huh28.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_Huh28.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K055.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K055.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K055.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K100.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K100.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K100.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K156.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K156.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K156.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K213.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K213.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K213.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K214.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K214.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_K214.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_MCF7.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_MCF7.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_MCF7.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_MMNK1.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_MMNK1.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_MMNK1.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_RBE.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_RBE.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_RBE.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_SSP25.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_SSP25.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_SSP25.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_T47D.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_T47D.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_T47D.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_TFK1.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_TFK1.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_TFK1.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_YSCCC.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_YSCCC.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_YSCCC.results.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_ZR751.results.classify.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_ZR751.results.filtered.tsv
-	_basepair/fusion_defuse/SO_6831/SO_6831_ZR751.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D068.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D068.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D068.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D131.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D131.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D131.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D138.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D138.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_D138.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUCCA.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUCCA.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUCCA.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUCCT.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUCCT.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUCCT.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUH28.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUH28.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_HUH28.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K055.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K055.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K055.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K100.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K100.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K100.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K156.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K156.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K156.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K213.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K213.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K213.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K214.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K214.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_K214.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_MMNK1.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_MMNK1.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_MMNK1.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_RBE.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_RBE.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_RBE.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_SSP25.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_SSP25.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_SSP25.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_TFK1.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_TFK1.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_TFK1.results.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_YSCCC.results.classify.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_YSCCC.results.filtered.tsv
-	_basepair/fusion_defuse/SO_8069/SO_8069_YSCCC.results.tsv <br/>

Only concordance of fusion genes defined as fusion genes which found in both technical replicates were included for this study.

2. metadata
-	_metadata/metadata_basepair.xlsx
-	_metadata/metadata_cellline.xlsx
-	_metadata/metadata_master.xlsx

3. Known cancer-associated transcript fusions
-	pancanfus.txt
-	pancanfus.txt.gz <br/>

REF: Oncogene. 2015 September 10; 34(37): 4845-4854. <br/>
Download from http://www.tumorfusions.org/ at 20190214

# /output
This folder consist of: <br/> 

-	all_fusion_Oncogene.2015-all.fus_(with_MMNK1)_2019-06-01.csv : All fusion mapped with cancer-associated transcript fusions
-	gene_fusion_16celllines_Final_2019-06-01.csv : matrix from generated heatmap
-	gene_fusion_16celllines_mapped_with_tumorfusions_2019-06-01.csv : matrix from generated heatmap
-	Supplementary Figure Supl.fig_PB_2019-06-01.all.fus_(with_MMNK1).pdf : figure of fusion mapped with cancer-associated transcript fusions (with MMNK1 cell line)
-	Supplementary Figure Supl.fig_PB_2019-06-01.all.fus_(without_MMNK1).pdf : figure of fusion mapped with cancer-associated transcript fusions (without MMNK1 cell line)