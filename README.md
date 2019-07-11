## Computational Pipeline for Genome-wide DNA-methylation data analysis

* [MINI REVIEW: Statistical methods for detecting differentially methylated loci and regions](http://biorxiv.org/content/biorxiv/early/2014/07/15/007120.full.pdf)
* [Tumor purity and differential methylation in cancer epigenomics](http://bfg.oxfordjournals.org/content/early/2016/05/18/bfgp.elw016.long)
* [Strategies for analyzing bisulfite sequencing data](http://www.biorxiv.org/content/early/2017/02/17/109512) now published in  http://www.sciencedirect.com/science/article/pii/S0168165617315936?via%3Dihub
* [Nature Genetics review: Statistical and integrative system-level analysis of DNA methylation data](https://www.nature.com/articles/nrg.2017.86)


**Illumina is phasing out 450k and introducing the new 850k as in the end of 2015**
### 450k/850k array analysis
* [bioconductor missMethyl](https://www.bioconductor.org/packages/release/bioc/html/missMethyl.html)  
* [450k-analysis-guide](https://github.com/crazyhottommy/450k-analysis-guide) A bit dated, but still useful.
* [450k with minif bioc workflow](https://www.bioconductor.org/help/course-materials/2015/BioC2015/methylation450k.html)
* [Preprocessing, normalization and integration of the Illumina HumanMethylationEPIC array with minfi](http://bioinformatics.oxfordjournals.org/content/early/2016/12/28/bioinformatics.btw691.full)
* [paper: Analysis pipelines and packages for Infinium HumanMethylation450 BeadChip (450k) data](http://www.sciencedirect.com/science/article/pii/S1046202314002692)
* [bigmelon](http://bioconductor.org/packages/devel/bioc/html/bigmelon.html) bioc package. Illumina methylation array analysis for large experiments
* [bioconductor MEAL](http://bioconductor.org/packages/devel/bioc/vignettes/MEAL/inst/doc/MEAL.html) MEAL aims to facilitate the analysis of Illumina Methylation 450K chips   
* [an R package for normalization of DNA methylation data when there are multiple cell or tissue types.](https://github.com/GreenwoodLab/funtooNorm)
* [normalize450K bioconductor](http://bioconductor.org/packages/devel/bioc/html/normalize450K.html)
* [A cross-package Bioconductor workflow for analysing methylation array data](http://f1000research.com/articles/5-1281/v1). F1000 research paper.
* [paper: Preprocessing, normalization and integration of the Illumina HumanMethylationEPIC array](http://biorxiv.org/content/early/2016/07/23/065490) minif package extended to 850k.
* [paper:Comparison of Beta-value and M-value methods for quantifying methylation levels by microarray analysis](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-587)  

>The Beta-value method has a direct biological interpretation - it corresponds roughly to the percentage of a site that is methylated. This makes the Beta-value very attractive when modeling the underlying biological effect. However, this interpretation is an approximation [22], especially when the data has not been properly preprocessed and normalized. From an analytical and statistical standpoint, the Beta-value method has severe heteroscedasticity outside the middle methylation range, which imposes serious challenges in applying many statistic models. In comparison, the M-value method is more statistically valid in differential and other statistic analysis as it is approximately homoscedastic. Although the M-value statistic does not have an intuitive biological meaning, it is possible to provide an accurate estimation of methylation status by modeling the distribution of the M-value statistic. In differential methylation analysis, we recommend using M-value because we can directly apply most statistical analysis methods designed for expression microarrays and it is easy to implement a difference threshold adjustment to improve the TPR. And the difference of M-value can be interpreted as the fold-change in the non-log scale. Although both Beta-value and M-value methods have some limitations, the two statistics are inter-convertible using Equation 3, enabling the use of the most appropriate method. We recommend using the M-value method for differential methylation analysis and also including the Beta-value statistic in final reports due to its intuitive biological interpretation.

* [Comparison of clustering methods for investigation of genome-wide methylation array data](http://journal.frontiersin.org/article/10.3389/fgene.2011.00088/full)

>The results of simulations suggest that the hierarchical Ward–Manhattan approach provides a consistent approach and that the Manhattan distance appears to be the best metric to separate clusters based on beta-values. However, this result is not absolute with some conditions particularly under low decisive data conditions resulting in inconsistency.

* [Estimating and accounting for tumor purity in the analysis of DNA methylation data from cancer studies](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-1143-5) [InfiniumPurify V1.1](https://zenodo.org/record/200214#.WP6xg7YrKuU)

### RRBS
* [M3D: Statistical Testing for RRBS Data Sets](https://www.bioconductor.org/packages/release/bioc/vignettes/M3D/inst/doc/M3D_vignette.pdf)  

* [methylkit](https://github.com/al2na/methylKit) deals with RRBS and other data. A recent release [note](http://zvfak.blogspot.com/2016/06/methylkit-v096.html). Many new features are implemented including [segmentation](http://zvfak.blogspot.de/2015/06/segmentation-of-methylation-profiles.html) of DNA methylation data similar to CNV analysis. Now it is in bioconductor.

* [BiSeq](https://www.bioconductor.org/packages/release/bioc/html/BiSeq.html) RRBS centric.

### Whole genome BS-seq
* [MethGo: a comprehensive tool for analyzing whole-genome bisulfite sequencing data](http://paoyangchen-laboratory.github.io/methgo/) 
* [bismark-pipeline.pdf](https://github.com/crazyhottommy/DNA-methylation-analysis/files/92245/bismark-pipeline.pdf) [bismark doc](https://github.com/FelixKrueger/Bismark/blob/master/Docs/README.md#viii-notes-about-different-library-types-and-commercial-kits)
* [Post-Processing Bismark Bisulphite Sequencing Data](http://blog.mcbryan.co.uk/2013/02/post-processing-bismark-bisulphite.html)  
* [The Binomial Distribution, Python and Bisulphite Sequencing](http://blog.mcbryan.co.uk/2013/02/the-binomial-distribution-python-and.html) 

### Nanopore
* [Detecting DNA Methylation using the Oxford Nanopore Technologies MinION sequencer](http://biorxiv.org/content/early/2016/04/04/047142)
* [Cytosine Variant Calling with High-throughput Nanopore Sequencing](http://biorxiv.org/content/early/2016/04/04/047134)

### Batch effect

* [BEclear](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0159921): Batch Effect Detection and Adjustment in DNA Methylation Data

### Clustering
* [Clustering of (epigenetic) DNA methylation data using a variational Bayes NMF algorithm:EpiCluster bioconductor ](http://bioconductor.org/packages/devel/bioc/html/EpiCluster.html)
* [densityCut: an efficient and versatile topological approach for automatic clustering of biological data](http://m.bioinformatics.oxfordjournals.org/content/early/2016/04/23/bioinformatics.btw227.short?rss=1)

### Motifs 
* [Discovering DNA motifs and genomic variants associated with DNA methylation](http://biorxiv.org/content/early/2016/09/06/073809)

### Databases
* [MethHC: a database of DNA methylation and gene expression in human cancers](http://methhc.mbc.nctu.edu.tw/php/index.php)
* [MethyCancer: a database of DNA Methylation and Cancer](http://methycancer.psych.ac.cn/)
* [MethDB: DNA methylation and environmental epigenetic effects](http://www.methdb.net/)
* [MethylomeDB: The Brain Methylome Database provides DNA methylation profiles from humans and mice](https://epigenie.com/epigenetic-tools-and-databases/)
* [DiseaseMeth: Methylomes of human disease](https://epigenie.com/epigenetic-tools-and-databases/)
* [NGSmethDB: Whole-genome bisulfite sequencing (WGBS) database for many different tissues, pathological conditions, and species](https://epigenie.com/epigenetic-tools-and-databases/)
* [MethBase: Hundreds of methylomes from well studied organisms](https://epigenie.com/epigenetic-tools-and-databases/)

### Visualization
* [TCGA Wanderer: an interactive viewer to explore DNA methylation and gene expression data in human cancer](http://maplab.imppc.org/wanderer/)
* [MEXPRESS: a data visualization tool designed for the easy visualization of TCGA expression, DNA methylation and clinical data](https://mexpress.be/about)
