# Cyanobacteria thing

## Jasper C., Anne B., Greg B.  

## Background  

We were interested... Author et al. 2019 assembled the genome of ... We compared. 

## Methods

Author et al. 2019 sequences we downloaded from ... 

Our files were in fastqz

We used X programs loaded with a conda environment on the RON computing cluster ...

or

We ran our analysis on a laptop...

We ran into this issue...

read plot files using https://view.qiime2.org

## Graphs - 

<img width="449" height="157" alt="image" src="https://github.com/user-attachments/assets/68af7a9c-5dbf-4a11-a1ba-a41e22629729" />

**Figure 1.** Frequency histograms of sequencing depth for forward (left) and reverse (right) reads across all samples. The x-axis represents the number of sequences per sample (×1,000), and the y-axis indicates the number of samples per bin. 

<img width="585" height="421" alt="image" src="https://github.com/user-attachments/assets/4ff8621e-547d-4ef3-b292-d914a2f1d25f" />

**Figure 2.** Taxonomic barplot of domain-level composition across all cyanobacterial samples generated in QIIME 2. The x-axis represents individual samples, and the y-axis denotes relative abundance.

<img width="586" height="332" alt="image" src="https://github.com/user-attachments/assets/261cd9f6-2ac4-4a36-8362-50622e476a87" />

**Figure 3.** Principal coordinates analysis (PCoA) of weighted Unique Fraction Metric (UniFrac) distances among cyanobacterial communities visualized in QIIME 2 Emperor. Axes 1, 2, and 3 explain 32.97%, 21.36%, and 12.43% of total variation, respectively. Sample shapes denote groupings (squares are numbered samples, spheres are AIR samples, diamonds are NTC and PAC samples, cones are WLW samples, and cylinders are XB samples).

## Discussion - 

**Figure one:**

&emsp; The frequency histograms of sequencing depth for both forward and reverse reads reveal a largely similar distribution across the sample cohort, indicating an effective sequencing effort with limited variability. In both directions, the majority of samples fall within the 0–600k sequence range, with the modal bin occurring between 200k and 400k sequences, wherein six samples are represented. A secondary cluster of five samples occupies the 0–200k bin, while four samples each are distributed across the 400k–600k and 600k–800k ranges, suggesting a moderate spread of mid-depth libraries. Notably, a small subset of two samples in both the forward and reverse reads exhibits substantially higher sequencing depths, falling within the 1,200k–1,400k bin, indicating potential outliers that may reflect unequal library preparation or pooling imbalances. The near-identical distributions observed between forward and reverse read histograms suggest strong pairing fidelity and technical accuracy in the sequencing run, with no directional loss or asymmetric difference in reads. This uniformity across orientations is indicative of quality reads, as divergence between forward and reverse depth distributions can signal adapter trimming artifacts or orientation-specific sequencing failures. The presence of high-depth outlier samples warrants consideration during downstream analyses, as disproportionately deep libraries may introduce bias in diversity metrics if rarefaction thresholds are not carefully calibrated to account for the full range of observed sequencing depths.

**Figure two -** 

&emsp; Taxonomic composition analysis of the cyanobacterial samples, as visualized in the QIIME 2 taxa barplot, revealed an overwhelming dominance of the domain Bacteria across all samples, with relative abundances approaching 99–100% in every case. In contrast, Archaea were either entirely absent or negligibly present, contributing minimally to the overall microbial community structure. This uniformity across all sample types indicates a highly conserved domain-level composition despite the substantial phylogenetic and compositional differences observed in the later PCoA analyses. Notably, even samples that were strongly separated along Axis 1 in the weighted UniFrac PCoA (Figure Three) did not exhibit divergence at the domain level, suggesting that the observed community differences are not driven by broad taxonomic shifts (e.g., Bacteria vs. Archaea), but rather by variation within bacterial lineages.

**Figure three -** 

&emsp; Principal coordinates analysis (PCoA) of the weighted UniFrac distance matrix revealed several distinct characteristics regarding the cyanobacterial community structure across samples, as visualized through the Emperor interface in QIIME 2. The first three axes explained 32.97%, 21.36%, and 12.43% of the total variation, respectively, indicating that a substantial proportion of community dissimilarity is captured within the ordination space. The most prominent feature of the plot was the strong phylogenetically informed separation along Axis 1, which represents the largest source of variation in the dataset. Along this axis, a tightly clustered group of square-labeled samples (2-1-100 through 40-100) was clearly isolated on the positive end, while all other sample types—including sphere (AIR), diamond (NTC, PAC), cone (WLW), and cylinder (XB) samples—were distributed along the negative side. This pattern demonstrates significant phylogenetic structuring and suggests that the square samples share a highly similar and potentially environmentally constrained community composition. Their tight clustering further indicates high intra-group relatedness, consistent with a shared ecological niche or selective pressure that favors a stable and conserved cyanobacterial assemblage. In contrast, the broader dispersion of the non-square samples reflects greater heterogeneity, implying that these communities are shaped by more variable or less restrictive environmental conditions.

&emsp; Further examination of the ordination reveals additional gradients of variation beyond the primary Axis 1 separation. Axis 2, which accounts for 21.36% of the variation, distinguishes substructure within the non-square samples, suggesting the presence of secondary environmental or ecological drivers influencing community composition. Notably, diamond (NTC, PAC) and AIR sphere samples tend to occupy higher positions along this axis, whereas cone (WLW) samples and the XB cylinder sample are distributed more centrally to lower along Axis 2. This separation indicates that, while these samples may share some phylogenetic overlap, they are still differentiated by finer-scale compositional shifts, potentially reflecting differences in environmental inputs or localized habitat conditions. Additionally, the absence of a smooth gradient across sample groupings—analogous to the “color bleeding” observed in unweighted analyses—suggests that these differences are not driven by a single continuous variable but rather by multiple interacting factors. Axis 3 (12.43%) contributes further, though more modest, separation, primarily isolating a small number of outlying samples positioned at the extremes of the ordination space. These outliers likely represent unique or transitional community states that deviate from the dominant assemblages. Collectively, these results indicate that cyanobacterial communities are structured along a major compositional gradient that strongly separates the square samples from all others, while additional axes capture more nuanced variation within the remaining groups, consistent with complex and potentially overlapping environmental influences driving community assembly.

### Sources - 

Bokulich, N. A., Kaehler, B. D., Rideout, J. R., Dillon, M., Bolyen, E., Knight, R., Huttley, G. A., & Caporaso, J. G. (2018). Optimizing taxonomic classification of marker-gene amplicon sequences with QIIME 2's q2-feature-classifier plugin. Microbiome, 6(1), 90. https://doi.org/10.1186/s40168-018-0470-z
&nbsp;
 
Bolyen, E., Rideout, J. R., Dillon, M. R., Bokulich, N. A., Abnet, C. C., Al-Ghalith, G. A., Alexander, H., Alm, E. J., Arumugam, M., Asnicar, F., Bai, Y., Bisanz, J. E., Bittinger, K., Brejnrod, A., Brislawn, C. J., Brown, C. T., Callahan, B. J., Caraballo-Rodríguez, A. M., Chase, J., … Caporaso, J. G. (2019). Reproducible, interactive, scalable and extensible microbiome data science using QIIME 2. Nature Biotechnology, 37(8), 852–857. https://doi.org/10.1038/s41587-019-0209-9
 
 
Callahan, B. J., McMurdie, P. J., Rosen, M. J., Han, A. W., Johnson, A. J. A., & Holmes, S. P. (2016). DADA2: high-resolution sample inference from Illumina amplicon data. Nature Methods, 13(7), 581. https://doi.org/10.1038/nmeth.3869
 
 
Halko, N., Martinsson, P.-G., Shkolnisky, Y., & Tygert, M. (2011). An Algorithm for the Principal Component Analysis of Large Data Sets. SIAM Journal on Scientific Computing. https://doi.org/10.1137/100804139
 
 
Hamady, M., Lozupone, C., & Knight, R. (2010). Fast UniFrac: facilitating high-throughput phylogenetic analyses of microbial communities including analysis of pyrosequencing and PhyloChip data. The ISME Journal, 4(1), 17–27. https://doi.org/10.1038/ismej.2009.97
 
 
Katoh, K., & Standley, D. M. (2013). MAFFT multiple sequence alignment software version 7: improvements in performance and usability. Molecular Biology and Evolution, 30(4), 772–780. https://doi.org/10.1093/molbev/mst010
 
 
Lane, D. (1991). 16S/23S rRNA sequencing. In E. Stackebrandt & M. Goodfellow (Eds.), Nucleic Acid Techniques in Bacterial Systematics (pp. 115–175). John Wiley.
 
 
Legendre, P., & Legendre, L. (2012). Numerical Ecology (Third, p. 499). Elsevier.
 
 
Lozupone, C. A., Hamady, M., Kelley, S. T., & Knight, R. (2007). Quantitative and Qualitative β Diversity Measures Lead to Different Insights into Factors That Structure Microbial Communities. Applied and Environmental Microbiology, 73(5), 1576–1585. https://doi.org/10.1128/AEM.01996-06
 
 
Lozupone, C., & Knight, R. (2005). UniFrac: a New Phylogenetic Method for Comparing Microbial Communities. Applied and Environmental Microbiology, 71(12), 8228–8235. https://doi.org/10.1128/AEM.71.12.8228-8235.2005
 
 
Lozupone, C., Lladser, M. E., Knights, D., Stombaugh, J., & Knight, R. (2011). UniFrac: an effective distance metric for microbial community comparison. The ISME Journal, 5(2), 169–172. https://doi.org/10.1038/ismej.2010.133
 
 
Martin, M. (2011). Cutadapt removes adapter sequences from high-throughput sequencing reads. EMBnet. Journal, 17(1), pp-10. https://doi.org/10.14806/ej.17.1.200
 
 
McDonald, D., Clemente, J. C., Kuczynski, J., Rideout, J. R., Stombaugh, J., Wendel, D., Wilke, A., Huse, S., Hufnagle, J., Meyer, F., Knight, R., & Caporaso, J. G. (2012). The Biological Observation Matrix (BIOM) format or: how I learned to stop worrying and love the ome-ome. GigaScience, 1(1), 7. https://doi.org/10.1186/2047-217X-1-7
 
 
McDonald, D., Vázquez-Baeza, Y., Koslicki, D., McClelland, J., Reeve, N., Xu, Z., Gonzalez, A., & Knight, R. (2018). Striped UniFrac: enabling microbiome analysis at unprecedented scale. Nature Methods, 15(11), 847–848. https://doi.org/10.1038/s41592-018-0187-8
 
 
Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., Blondel, M., Prettenhofer, P., Weiss, R., Dubourg, V., Vanderplas, J., Passos, A., Cournapeau, D., Brucher, M., Perrot, M., & Duchesnay, É. (2011). Scikit-learn: Machine learning in Python. Journal of Machine Learning Research, 12(Oct), 2825–2830.
 
 
Price, M. N., Dehal, P. S., & Arkin, A. P. (2010). FastTree 2–approximately maximum-likelihood trees for large alignments. PloS One, 5(3), e9490. https://doi.org/10.1371/journal.pone.0009490
 
 
Vázquez-Baeza, Y., Gonzalez, A., Smarr, L., McDonald, D., Morton, J. T., Navas-Molina, J. A., & Knight, R. (2017). Bringing the dynamic microbiome to life with animations. Cell Host & Microbe, 21(1), 7–10. https://doi.org/10.1016/j.chom.2016.12.009
 
 
Vázquez-Baeza, Y., Pirrung, M., Gonzalez, A., & Knight, R. (2013). EMPeror: a tool for visualizing high-throughput microbial community data. Gigascience, 2(1), 16. https://doi.org/10.1186/2047-217X-2-16
 
 
Weiss, S., Xu, Z. Z., Peddada, S., Amir, A., Bittinger, K., Gonzalez, A., Lozupone, C., Zaneveld, J. R., Vázquez-Baeza, Y., Birmingham, A., Hyde, E. R., & Knight, R. (2017). Normalization and microbial differential abundance strategies depend upon data characteristics. Microbiome, 5(1), 27. https://doi.org/10.1186/s40168-017-0237-y
 
 
Wes McKinney. (2010). Data Structures for Statistical Computing in Python. In S. van der Walt & Jarrod Millman (Eds.), Proceedings of the 9th Python in Science Conference (pp. 51–56).
 
Weiss, S., Xu, Z. Z., Peddada, S., Amir, A., Bittinger, K., Gonzalez, A., Lozupone, C., Zaneveld, J. R., Vázquez-Baeza, Y., Birmingham, A., Hyde, E. R., & Knight, R. (2017). Normalization and microbial differential abundance strategies depend upon data characteristics. Microbiome, 5(1), 27. https://doi.org/10.1186/s40168-017-0237-y
 
Wes McKinney. (2010). Data Structures for Statistical Computing in Python. In S. van der Walt & Jarrod Millman (Eds.), Proceedings of the 9th Python in Science Conference (pp. 51–56).
