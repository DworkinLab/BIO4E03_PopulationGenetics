# Population Genetics using R

The `R` programming language has many libraries of great use, and increasingly so for both population genetic analysis and for learning and teaching population genetics.


So here is a brief list. As I am still compiling them, for the moment this is quite dis-organized.

## lists of lists
As always [CRAN Task views](https://cran.r-project.org/web/views/) is a good place to start for an overall view of libraries that are useful. In particular the Task view for [Genetics](https://cran.r-project.org/web/views/Genetics.html) and for [phylogenetics](https://cran.r-project.org/web/views/Phylogenetics.html). There are particular areas of overlap in these disciplines (i.e. simulating genealogies) which can be quite important.

Nescent also maintains a [list](http://popgen.nescent.org/PACKAGES.html). They also have some tutorials that are useful for practical data analysis [here](http://popgen.nescent.org/index.html).

## Special issue with R packages
There was also a nice special issue in the journal *Molecular Ecology Resources* on **Population Genomics with R**. The issue is [here](http://onlinelibrary.wiley.com/doi/10.1111/men.2017.17.issue-1/issuetoc). This has numerous papers describing a number of software tools in R. This [introduction](http://onlinelibrary.wiley.com/doi/10.1111/1755-0998.12636/full) summarizes lots of it if you want to take a look.


## Learning
[driftR](https://github.com/cjbattey/driftR)

## Where to start
There are some libraries that do many many things. `PopGenome` is an example of one. There are a few others as well.

[PopGenome](https://cran.r-project.org/web/packages/PopGenome/index.html). : An efficient Swiss Army knife for population Genomic Analyses in R. The vignette is [here](https://cran.r-project.org/web/packages/PopGenome/vignettes/An_introduction_to_the_PopGenome_package.pdf). Another tutorial on whole genome analysis is [here](https://cran.r-project.org/web/packages/PopGenome/vignettes/Whole_genome_analyses_using_VCF_files.pdf). Another tutorial is [here](https://github.com/tonig-evo/workshop-popgenome). The paper is [here](https://academic.oup.com/mbe/article/31/7/1929/2925788/PopGenome-An-Efficient-Swiss-Army-Knife-for).

## Data import, cleaning, transformations and export
[StrataG](https://cran.r-project.org/web/packages/strataG/index.html):An r package for manipulating, summarizing and analysing population genetic data.

[GENEPOPEDIT](https://github.com/rystanley/genepopedit): a simple and flexible tool for manipulating multilocus molecular data in R.

[apex](https://cran.r-project.org/web/packages/apex/index.html): phylogenetics with multiple genes. Toolkit for the analysis of multiple gene data. Apex implements the new S4 classes 'multidna', 'multiphyDat' and associated methods to handle aligned DNA sequences from multiple genes.

[seqinr](https://cran.r-project.org/web/packages/seqinr/index.html): Exploratory data analysis and data visualization for biological sequence (DNA and protein) data. Includes also utilities for sequence data management under the ACNUC system.

[SeqArray](http://corearray.sourceforge.net/tutorials/SeqArray/): r Big Data Management of Genome-Wide Sequencing Variants

## Data visualization
[POPHELPER](http://royfrancis.github.io/pophelper/): An R package and web app to analyze and visualize population structure.

[minotaur](https://github.com/NESCent/MINOTAUR):A platform for the analysis and visualization of multivariate results from genome scans with R Shiny.

## Genomic Data
[VCFR](https://cran.r-project.org/web/packages/vcfR/vignettes/intro_to_vcfR.html): A package to manipulate and visualize variant call format data in R.

# Detecting Selection and hybridization
[pcadapt](https://cran.r-project.org/package=pcadapt): an R package to perform genome scans for selection based on principal component analysis. Here is an [example tutorial](https://cran.r-project.org/web/packages/pcadapt/vignettes/pcadapt.html).

[parallelnewhybrid](https://github.com/bwringe/parallelnewhybrid): an R package for the parallelization of hybrid detection using newhybrids.

[rehh 2.0](https://cran.r-project.org/package=rehh): a reimplementation of the R package rehh to detect positive selection from haplotype structure. Here is a [tutorial](https://cran.r-project.org/web/packages/rehh/vignettes/rehh.pdf). Link to the new [paper]http://onlinelibrary.wiley.com/doi/10.1111/1755-0998.12634/abstract.

[pegas](https://cran.r-project.org/package=pegas): Population and Evolutionary Genetics Analysis System. Link to the [paper](https://academic.oup.com/bioinformatics/article-lookup/doi/10.1093/bioinformatics/btp696).

[OutFLANK](https://github.com/whitlock/OutFLANK):A procedure to find Fst outliers based on an inferred distribution of neutral Fst. See here for a quick [tutorial](http://popgen.nescent.org/2016-01-26-SNP-selection.html#section-3-outflank-httpsgithub.comwhitlockoutflank)

## Population Differentiation and divergence
[hierFstat](https://cran.r-project.org/package=hierfstat):Estimation and Tests of Hierarchical F-Statistics.
[mmod](https://cran.r-project.org/package=mmod): 	Modern Measures of Population Differentiation

## Simulation (both forward and reverse)
[scrm: Simulating the Evolution of Biological Sequences](https://cran.r-project.org/package=scrm):A coalescent simulator that allows the rapid simulation of biological sequences under neutral models of evolution. Different to other coalescent based simulations, it has an optional approximation parameter that allows for high accuracy while maintaining a linear run time cost for long sequences. It is optimized for simulating massive data sets as produced by Next- Generation Sequencing technologies for up to several thousand sequences. Link to the [vignette](https://cran.r-project.org/web/packages/scrm/vignettes/scrm-Arguments.html). Link to the [paper](https://academic.oup.com/bioinformatics/article-lookup/doi/10.1093/bioinformatics/btu861).

[coala](https://cran.r-project.org/package=coala):Coalescent simulators can rapidly simulate biological sequences evolving according to a given model of evolution. You can use this package to specify such models, to conduct the simulations and to calculate additional statistics from the results. It relies on existing simulators for doing the simulation, and currently supports the programs 'ms', 'msms' and 'scrm'. It also supports finite-sites mutation models by combining the simulators with the program 'seq-gen'.

[phyclust](https://cran.r-project.org/package=phyclust). Phylogenetic clustering (phyloclustering) is an evolutionary Continuous Time Markov Chain model-based approach to identify population structure from molecular data without assuming linkage equilibrium. The package phyclust (Chen 2011) provides a convenient implementation of phyloclustering for DNA and SNP data, capable of clustering individuals into subpopulations and identifying molecular sequences representative of those subpopulations. **Can do ms like simulations!!**. See the [website](https://snoweye.github.io/phyclust/) for more information including examples.

[skelesim](https://cran.r-project.org/package=skeleSim): an extensible, general framework for population genetic simulation in R (with shiny interface). I think this is mostly a front end (?)

[MetaPopGen](http://onlinelibrary.wiley.com/doi/10.1111/1755-0998.12371/abstract):an r package to simulate population genetics in large size metapopulations

[rmetasim](https://cran.r-project.org/package=rmetasim):rmetasim: An Individual-Based Population Genetic Simulation Environment.


## inference (estimating theta, demographic parameters, etc..)
[coalescentMCMC](https://cran.r-project.org/package=coalescentMCMC):MCMC Algorithms for the Coalescent. Flexible framework for coalescent analyses in R. It includes a main function running the MCMC algorithm, auxiliary functions for tree rearrangement, and some functions to compute population genetic parameters. Link to [vignette](https://cran.r-project.org/web/packages/coalescentMCMC/vignettes/Running_coalescentMCMC.pdf).


## Education
[population genetics in R](https://grunwaldlab.github.io/Population_Genetics_in_R/). A Primer on applied population genetics.
[evobiR](https://cran.r-project.org/web/packages/evobiR/index.html): Comparative and Population Genetic Analyses. Interactive simulations for teaching.

## Other
[ape](http://ape-package.ird.fr/): Analyses of Phylogenetics and Evolution. **Many packages depend on this**. [Link to Book](http://ape-package.ird.fr/APER.html). [link](http://ape-package.ird.fr/APER/APER2/APER2_Online_Material.tar.gz) to data and scripts associated with the book.  This has `DNAbin` class for DNA alignments.

[adegenet](https://cran.r-project.org/web/packages/adegenet/index.html): Exploratory Analysis of Genetic and Genomic Data. Tutorials are [here](https://github.com/thibautjombart/adegenet/wiki). Old sourceforge page (still has useful bits) is [here](http://adegenet.r-forge.r-project.org/)

[poppr](http://grunwaldlab.cgrb.oregonstate.edu/poppr-r-package-population-genetics): Genetic Analysis of Populations with Mixed Reproduction

## Data to use
[rsnps](https://cran.r-project.org/package=rsnps):Get 'SNP' ('Single-Nucleotide' 'Polymorphism') Data on the Web. A programmatic interface to various 'SNP' 'datasets' on the web: [OpenSNP](https://opensnp.org), []'NBCIs' 'dbSNP' database](https://www.ncbi.nlm.nih.gov/projects/SNP), and [Broad Institute 'SNP' Annotation and Proxy Search](http://archive.broadinstitute.org/mpg/snap/ldsearch.php). Functions are included for searching for 'SNPs' for the Broad Institute and 'NCBI'. For 'OpenSNP', functions are included for getting 'SNPs', and data for 'genotypes', 'phenotypes', annotations, and bulk downloads of data by user.

1000 genomes, Drosophila genomes...

## Phylogenetics
[phangorn](https://cran.r-project.org/web/packages/phangorn/index.html)

[RADami](https://cran.r-project.org/package=RADami): Phylogenetic Analysis of RADseq Data

[phylodyn](https://github.com/mdkarcher/phylodyn): an R package for phylodynamic simulation and inference

## Not R, but useful
[fastsimcoal2](http://cmpg.unibe.ch/software/fastsimcoal2/)

[SLiM](https://messerlab.org/slim/)

[angsd](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-014-0356-4). Computing pop gen summary stats. Assumes diploids, no pooling. Link to github page is [here](https://github.com/ANGSD/angsd)

Will add ms, msms, simcoal2,...
