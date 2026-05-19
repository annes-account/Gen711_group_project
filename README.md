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

Sources - 




